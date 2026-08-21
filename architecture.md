# System Architecture

## Overview

The platform follows a BI-first architecture.

The primary focus is on reliable data, governed business metrics,
data modeling, and decision-support reporting.

AI is introduced as an augmentation layer rather than as the foundation
of the platform.

---

## High-Level Architecture

```text
                    Public Data Sources
                           |
             +-------------+-------------+
             |             |             |
           ERCOT          EIA          NOAA
             |             |             |
             +-------------+-------------+
                           |
                           v
                  Data Ingestion Layer
                    Python / SQL
                           |
                           v
                     Raw Data Layer
                           |
                           v
                 Data Quality Checks
                           |
                           v
                 Transformation Layer
                           |
                           v
                  Analytical Data Model
                           |
                           v
                  BI Semantic Layer
                           |
             +-------------+-------------+
             |             |             |
             v             v             v
        Portfolio BI   Customer BI   BI Operations
             |             |             |
             +-------------+-------------+
                           |
                           v
                    AI-Assisted BI
                           |
                           v
                  Decision Support
                           |
                           v
                     BI Dashboard
