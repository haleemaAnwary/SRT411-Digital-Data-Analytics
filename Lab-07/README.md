# Lab 07 — Threat Intelligence Integration and Linux Audit Monitoring

**Course:** SRT411 — Digital Data Analytics  
**Tools:** Filebeat, Elasticsearch, Kibana, auditd, Kali Linux, Nmap  
**Evidence:** 19-page academic lab report (PDF to be uploaded separately)

## Overview

This lab explores open-source threat intelligence ingestion and Linux security-event monitoring in the Elastic Stack. It documents the Filebeat threat-intelligence module with abuse.ch sources, collection of auditd records, controlled activity from a Kali Linux virtual machine, and security-oriented Kibana visualizations.

## Tasks completed

### 1. Open-source threat intelligence feeds
- Enabled Filebeat's **threatintel** module and configured the **abuseurl** and **abusemalware** filesets for abuse.ch malicious URL and malware hash feeds.
- Inspected ingested records in **Kibana Discover**.
- Created separate **AbuseURL** and **AbuseMalware** dashboards to explore indicators and visualize distributions.

### 2. Linux audit logging and controlled activity
- Prepared an **Elastic Stack VM** and a separate **Kali Linux VM** for controlled lab exercises.
- Installed and enabled **auditd**, configured audit rules, and enabled Filebeat's auditd module to collect audit events.
- Performed an **SSH login** and an **Nmap scan** from Kali, and ran a test script to generate system activity.
- Investigated resulting events in Kibana Discover, including process-related records and remote file-deletion activity.
- Created a Kibana dashboard summarizing **executables, audit keys, and users**.

### 3. Threat-hunting and detection concepts
The written analysis compares attack-based and data-based threat hunting and discusses threat intelligence, automated collection and response, severity classification, and Elastic Security integrations. These are **conceptual topics**, not evidence of a deployed AI/ML autonomous hunting or incident-response platform.

## Skills demonstrated

**Filebeat · Open-Source Threat Intelligence · abuse.ch Feeds · Elasticsearch · Kibana · Linux auditd · Security Event Collection · Log Investigation · Nmap · Kali Linux · Dashboard Visualization · Threat Hunting Fundamentals**

## Report evidence
- **Pages 3–6:** Filebeat threat intelligence configuration, Discover records, and feed dashboards.
- **Pages 7–14:** Virtual lab, auditd configuration, controlled testing, event inspection, and audit-event dashboard.
- **Pages 15–18:** Written threat detection and threat hunting concepts.

Upload `Lab 07 Manual.pdf` to this folder separately and link it here.

## Scope and limitations

This is an **academic lab** demonstrating ingestion and analysis of threat-intelligence feeds and audit events. The report does not verify that the lab automatically matched indicators to host activity, blocked attacks, or delivered end-to-end automated threat response. Screenshots and described tests are lab observations, not production detection-performance metrics. Original VM images, scripts, configuration files and datasets are not provided in this repository.
