# Analytical Data Model

## Overview

The analytical data model follows a dimensional modeling approach.

The model separates descriptive dimensions from measurable business facts
to support reusable BI analysis and reporting.

The primary design objective is to provide a consistent analytical grain,
clear relationships, and reusable business metrics.

---

## Conceptual Model

```text
                  Dim Date
                     |
                     |
Dim Customer ---- Fact Usage ---- Dim Product
                     |
                     |
                Dim Location
                     |
                     |
               Dim Market
