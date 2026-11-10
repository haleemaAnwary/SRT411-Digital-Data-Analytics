# Lab 06 — Centralized Logging and DNS Traffic Analytics with ELK

**Course:** SRT411 — Digital Data Analytics  
**Technologies:** Elasticsearch, Logstash, Kibana, Grok, Mutate filters  
**Evidence:** Academic Lab 06 report (PDF available below)

## Original lab report

[View Lab 06 report (PDF)](<Lab%2006%20Manual.pdf>) — original academic lab documentation and screenshots.

## Overview
This lab extends ELK-based logging by ingesting application and MySQL logs, extracting structured event fields, exploring records in Kibana, and creating visualizations of benign browser DNS traffic and malicious DNS-tunneling datasets.

## Tasks completed

### 1. Centralized application and database logging
- Ran an application stack and collected application and MySQL logs.
- Configured a **MySQL Logstash pipeline** to identify query entries, extract an ID with Grok, tag events as `mysql_log`, and index matching records in Elasticsearch as `mysql_logs`.
- Configured an **application Logstash pipeline** to parse critical API access entries, extract fields including **email, ID and name**, tag them as `criticalapi`, and index matching records in `app_logs`.
- Used **Kibana Discover** to inspect ingested events and the fields extracted from log messages.

### 2. Logging and investigation concepts
- Compared application, system and security logs and reviewed attributes of actionable log messages.
- Discussed using HTTP status codes, API paths, timestamps, user details and SQL commands to investigate application and database activity.
- Identified the importance of structure, consistency, context and avoiding unnecessary sensitive content in logs.

### 3. DNS data ingestion, analysis and visualization
Ingested and visualized four labeled DNS traffic datasets in the ELK Stack:

| Dataset | Label in the lab |
|---|---|
| Chrome | Benign |
| Firefox | Benign |
| dnscat2 | Malicious / DNS tunneling |
| iodine | Malicious / DNS tunneling |

The report documents Logstash pipelines, indexed data, Kibana exploration and visualizations for these datasets.

## Skills demonstrated
**ELK Stack · Logstash Pipelines · Grok Parsing · Mutate Filters · Elasticsearch Indexing · Kibana Discover · Dashboard Visualizations · Application Logs · MySQL Logs · DNS Traffic Analysis · Security Data Analytics**

## Documentation
The original report includes screenshots and explanations of the pipeline configurations, indexed records and visualizations. Upload the PDF to this folder, then add a link here.

## Scope and limitations
This is an academic log analytics exercise. It includes benign and malicious traffic **datasets**, but it does not establish a production-ready DNS tunneling detection system, measured detection accuracy, or live incident response. Original complete service configurations, datasets and executable source files are not included in this portfolio.
