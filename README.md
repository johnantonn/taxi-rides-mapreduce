# Taxi rides analytics

Java projects from **Big Data Analytics Programming** (KU Leuven MAI): processing taxi GPS track data at scale.

> **Status:** Personal / university coursework archive — **not actively maintained**. Hadoop / Spark versions in the POMs reflect the course era.

## How to run

Use **Java 8** and **Maven**. Build and run **MapReduce** from the repository root (see [README-ride-revenue.md](README-ride-revenue.md)). For **Spark**, `cd trip-length/` and use that module’s `pom.xml` and instructions. Each sub-project is independent.

## Layout

| Path | Stack | Description |
|------|--------|-------------|
| Repository root (`pom.xml`, `src/`) | **Apache Hadoop MapReduce** | Total ride revenue from GPS segments — see [README-ride-revenue.md](README-ride-revenue.md) |
| [`trip-length/`](trip-length/) | **Apache Spark** | Trip length / distance computation (`TripLength.java`) |

Build and run each part from its own directory (each has its own `pom.xml`).

## Requirements

- **Ride revenue**: Java 8, Hadoop (see [README-ride-revenue.md](README-ride-revenue.md))
- **Trip length**: Java 8, Apache Spark (see `trip-length/pom.xml`)
