# Instant Payments Platform

> 🚧 Work in progress. Follow the progress in the [milestones](https://github.com/MathSMB/instant-payments-platform/milestones).

An event-driven instant payments platform, inspired by Brazil's Pix. It receives payment orders, moves money in a double-entry ledger, detects fraud in real time and reconciles statements in batch.

**This is a study and portfolio project.** It simulates an instant payment flow and does not connect to the Central Bank of Brazil or any real payment network. All data is fictitious.

## What this project demonstrates

- Consistency in distributed systems: idempotency keys, transactional outbox, saga with compensation
- Messaging with retry, dead-letter queues and reprocessing (Kafka)
- Real-time fraud detection with Kafka Streams, Avro and Schema Registry
- Batch reconciliation with Spring Batch
- Security (OAuth2), observability (OpenTelemetry, Grafana) and load testing (k6)
- Documented decisions: system design and ADRs in [`docs/`](docs/)

## Planned stack

Java 25 · Spring Boot 4.1 · PostgreSQL · Kafka · Redis · Keycloak · Testcontainers · OpenTelemetry · Grafana · k6 · Docker · Kubernetes (Helm) · Terraform

## Roadmap

| # | Milestone |
|---|---|
| 01 | Foundation: repository, CI and payment-api |
| 02 | Ledger and idempotency |
| 03 | Kafka, outbox and notifications |
| 04 | Saga, retry and DLQ |
| 05 | Security and API |
| 06 | Observability, load testing and documentation |
| 07 | Fraud detection with Kafka Streams |
| 08 | Reconciliation with Spring Batch |
| 09 | Performance, Kubernetes and Terraform |
