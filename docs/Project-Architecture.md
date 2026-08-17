# Project Architecture

## Overview

The project implements a custom SIEM dashboard using the ELK Stack to collect, analyze, detect, and visualize critical security events.

## Architecture Components

### Elasticsearch

Elasticsearch serves as the central repository for storing and indexing security events. It enables fast searching and aggregation of event data.

### Kibana

Kibana provides visualization and dashboard capabilities for monitoring security events, alerts, and trends.

### Elastic Security

Elastic Security was used to create custom detection rules and generate alerts for identified threats.

## Workflow

Security Events
↓
Elasticsearch Index
↓
Data View Creation
↓
Detection Rules
↓
Alert Generation
↓
Kibana Dashboard
↓
Security Monitoring

## Security Use Cases

- Brute-Force Attack Detection
- Privilege Escalation Detection
- Data Exfiltration Detection

The architecture supports centralized monitoring and rapid identification of suspicious security activities.
