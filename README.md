# RED Pipeline

> **Coming soon.** The complete code, configuration, and reproducibility instructions for the pipeline will be released here after the repository has been organized and documented.

This repository will host the open-source pipeline accompanying our paper on endpoint-level microservice anomaly detection and root-cause localization.

## Pipeline overview

The pipeline is designed around the Train-Ticket microservice system and endpoint-scoped fault injection. Each collection run combines:

- concurrent transaction workloads for realistic endpoint traffic;
- endpoint- or service-level fault injection with millisecond-resolution intervals;
- client-side response records, including status code, round-trip latency, response length, and response-body hashes;
- SkyWalking traces for server-side request rate, error rate, and duration metrics;
- pod logs and Prometheus metrics for auxiliary analysis;
- endpoint normalization and fusion into 15-second per-endpoint windows.

The resulting representation combines server-side RED metrics with client-observed response semantics and latency, enabling evaluation of anomaly detection and root-cause localization under richer observability conditions.

## Status

The implementation and documentation are being prepared. **Coming soon:**

- collection and orchestration scripts;
- fault-injection configurations;
- preprocessing and feature-fusion code;
- dataset schema and download instructions;
- reproduction instructions for the paper's experiments.

## Reference

The accompanying dataset is available at Zenodo: [10.5281/zenodo.24097673](https://doi.org/10.5281/zenodo.24097673).

## License

License information will be added with the first complete release.
