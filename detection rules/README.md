# Detection Rules

This directory contains custom SIEM detection rules developed using the Elastic (ELK) Stack to identify high-risk security activities and generate alerts for security monitoring.

## Detection Rules Included

### 1. Brute Force Detection Rule
Detects repeated authentication failures and suspicious login attempts that may indicate credential-based attacks.

**Monitored Activities:**
- Multiple failed login attempts
- Password guessing attacks
- Repeated authentication failures

### 2. Privilege Escalation Detection Rule
Identifies activities where users attempt to gain elevated permissions or unauthorized access to sensitive resources.

**Monitored Activities:**
- Unauthorized role changes
- Admin access grants
- Privilege abuse attempts
- Permission modification events

### 3. Data Exfiltration Detection Rule
Detects suspicious data transfer activities that may indicate information theft or unauthorized data movement.

**Monitored Activities:**
- Large file transfers
- Sensitive data uploads
- External data transfers
- Unusual network transfer activity

## Detection Methodology

Each rule was created using Kibana Detection Rules and configured with:
- Custom KQL queries
- Severity classification
- Risk scoring
- Automated alert generation
- Continuous monitoring

## Outcome

The implemented detection rules successfully generated alerts for simulated security events, demonstrating the effectiveness of the ELK Stack for threat detection and security monitoring.
