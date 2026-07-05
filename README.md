# Enterprise Banking Data Platform — an explorable model

*Work-derived model, fully generalized · 2025–2026*

**[Explore the live model →](https://halkhoori2000.github.io/Data-Platform-Confluent-Kafka/)**

This is an interactive model of a real enterprise banking data platform — the kind that turns dozens of source systems, event streams, and years of files into governed, queryable data products. It reads like a real reference architecture: individual pieces — source systems, connectors, Kafka, ADF, the Databricks lakehouse with its medallion layers, serving and BI tools — connected by the actual data-flow arrows, with security and governance running underneath. Level buttons (L0–L4) choose the depth: the executive overview, the full estate, then inside any clicked piece — down to Kafka's commit log and Delta Lake's transaction log.

Technically, the model covers a lakehouse platform built on Confluent Kafka (CDC streaming with Kafka Connect and Schema Registry), Azure Data Factory (control-table-driven batch with watermark incrementality), and Databricks on ADLS Gen2 + Delta Lake (Auto Loader, Delta Live Tables, Spark + Photon, Workflows), organized as Bronze → Silver → Gold, served through Databricks SQL and Delta Sharing, consumed via Power BI + Copilot and AI/BI Genie, and governed end-to-end by Unity Catalog with Entra ID, Key Vault, and private networking as the security rail. Clicking a piece opens its detail panel; three live demos run inside it — a Kafka partition's append-only log with replication and consumer offsets, Delta's transaction log with time travel, and a Spark job executing as stages, shuffles, and tasks. Four "journeys" show the platform at work — including the [Historic Data Loading](https://halkhoori2000.github.io/Historic-Data-Loading/) delivery, which ran on this platform.

## Use Cases

- **Explaining a modern data platform** — one diagram from source system to dashboard, at whatever depth the audience picks: executives stay at L0, engineers go to L4
- **Learning the streaming + lakehouse stack** — Kafka, CDC, Schema Registry, Delta Lake, medallion architecture, and lakehouse governance, each explained where it sits in the whole
- **Architecture reference** — the patterns (metadata-driven ingestion, watermark incrementality, deterministic quality rules, IaC-provisioned environments) are industry-standard and reusable
- **Portfolio deep-dive** — the journeys connect the model to real, documented deliveries

## Challenges

- **Depth without drowning** — the same page has to work for someone who wants five boxes and someone who wants offsets and ISR mechanics; explicit levels (L0–L4) plus a per-piece detail panel are the answer
- **Honesty at every level** — tool internals are public engineering knowledge, but delivery claims appear only in the journey pages, where they're backed by their own case studies
- **Confidentiality by construction** — the model generalizes an actual estate: no institution names, no internal system names, no configurations, no data appear anywhere
- **A model that stays true** — the architecture shown follows the real build: incremental batches directly into a governed gold layer, control-table watermarks, and one conformed table per source system

## Repository structure

```
index.html   ← the entire explorable model (GitHub Pages) — no build step, no dependencies
```
