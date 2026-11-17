# Secure Cloud Computing – Alzheimer's screening from handwriting

Project work for the **Secure Cloud Computing** course, University of Salerno, A.Y. 2026/2027 – Group 3.

## Description

The project delivers a web platform, provided as SaaS on a secure cloud infrastructure, that discriminates healthy subjects from patients with Alzheimer's disease based on the features of their handwriting.

The system receives the features extracted from the handwriting tasks performed by the patient and returns a prediction. Validated cases are used to periodically retrain the model.

## Users

- **Patient**: performs the handwriting tasks and can access only their own data.
- **Neurologist**: views, validates and delivers the results to their patients, and is the only one who knows their identity.
- **Administrator**: manages the service, sees only the features and retrains the model when needed.

## Service Level Agreement

| Requirement | Value |
|---|---|
| Service window | Monday–Friday, 08:00–18:00 |
| Availability | ≥ 99.5% of the uptime |
| Outage | At most 30 minutes per event, 3 minutes on average |
| Reliability | ≥ 99.5% of requests served correctly |
| Response time | ≤ 1 second at the 99th percentile |
| Peak load | Up to 5,000 requests per minute |

## Repository structure

```
Secure-Cloud-Computing/
├── model/          # WP1 – model training
├── app/            # WP2 – web app and inference API
├── docker/         # WP3 – containerization
├── k8s/            # WP4 – Kubernetes manifests
├── nginx/          # WP4 – NGINX configuration
├── stress-test/    # WP5 – load scenarios with wrk
├── docs/           # WP0, WP6 – documentation, planning, presentation
└── README.md
```

## Getting started

Instructions for running the application will be added at the end of development.

## Team

- **Gregorio Barberio** — [@gregbar2](https://github.com/gregbar2)
- **Simone Grimaldi** — [@simonegrimaldi](https://github.com/simonegrimaldi)
- **Davide Quaranta** — [@davidequaranta8](https://github.com/davidequaranta8)
