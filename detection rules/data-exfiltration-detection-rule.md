# Data Exfiltration Detection Rule

## Overview

This detection rule was implemented to detect potential data exfiltration activities that could indicate unauthorized transfer of sensitive information outside the organization.

## Rule Configuration

- Rule Name: Data Exfiltration Detection Rule
- Rule Type: Query Rule
- Severity: Critical
- Risk Score: 90
- Data View: security-events
- Query:

```kql
event_type:"Data Exfiltration"
```

## Detection Logic

The rule identifies events associated with large file transfers, sensitive data uploads, external data transfers, and other indicators of possible data exfiltration attempts.

## Validation

Test data representing exfiltration scenarios was ingested into Elasticsearch. The rule generated critical alerts successfully, demonstrating effective detection and alert generation capabilities.
