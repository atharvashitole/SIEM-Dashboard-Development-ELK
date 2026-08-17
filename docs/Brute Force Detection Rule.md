# Brute Force Detection Rule

## Overview

This detection rule was created to identify brute-force authentication attempts within the SIEM environment. The rule monitors security events containing the event type "Brute Force" and generates alerts whenever matching activities are detected.

## Rule Configuration

- Rule Name: Brute Force Detection Rule
- Rule Type: Query Rule
- Severity: High
- Risk Score: 75
- Data View: security-events
- Query:

```kql
event_type:"Brute Force"
```

## Detection Logic

The rule continuously searches indexed security events for indicators of repeated authentication failures and suspicious login activity associated with brute-force attacks.

## Validation

Sample brute-force events were ingested into Elasticsearch and successfully detected by Elastic Security. Generated alerts confirmed that the rule was functioning as expected.
