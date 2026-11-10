# Lab 05 — ELK Stack Deployment, NGINX Log Ingestion & Elasticsearch Queries

**Course:** SRT411 — Digital Data Analytics  
**Submitted:** June 9, 2024  
**Platform:** Ubuntu Linux  
**Tools:** Elasticsearch, Logstash, Kibana, NGINX access logs  
**Evidence:** 16-page academic lab report (PDF available below)

## Original lab report

[View Lab 05 report (PDF)](<Lab%2005%20Manual.pdf>) — original academic lab documentation and screenshots.

## Overview

This lab explores centralized log management and search analytics through the **ELK Stack** (Elasticsearch, Logstash, Kibana). It documents installation and configuration, log ingestion from an NGINX `access.log` file, dashboard visualizations, and basic index/document operations in Elasticsearch.

## Tasks completed

### 1. ELK Stack setup
- Installed and configured Elasticsearch on Ubuntu, including editing `elasticsearch.yml` and JVM heap settings.
- Installed and verified Kibana, and installed and started Logstash.
- Documented the environment and installation verification through terminal and interface screenshots.

### 2. NGINX access log ingestion
- Prepared an NGINX `access.log` sample file.
- Used a Logstash configuration to ingest and process the log records.
- Ran Logstash with the configured pipeline, then inspected indexed events in **Kibana Discover**.
- Created Kibana dashboard visualizations using the ingested records.

### 3. Elasticsearch indexing and queries
- Inspected the cluster's indices and queried documents.
- Created an index named `mydata` and added sample JSON documents.
- Retrieved a document by ID, deleted another by ID, and verified the deletion.

### 4. Elasticsearch concepts
Explained clusters and nodes, master versus data-node responsibilities, document indexing and storage, JSON representations, and differences between search-oriented Elasticsearch and relational databases.

## Skills demonstrated
**Ubuntu Linux · Elasticsearch · Logstash · Kibana · ELK Stack · Centralized Logging · Log Ingestion · NGINX Access Logs · Data Indexing · JSON Documents · Elasticsearch Queries · Dashboard Visualization**

## Evidence in the report
- **Pages 3–7:** ELK installation and configuration
- **Pages 8–10:** NGINX log pipeline, Kibana Discover and dashboard screenshots
- **Pages 11–14:** Elasticsearch index and document operations
- **Pages 15–16:** Conceptual reflections and setup notes

The original report is linked above.

## Scope and limitations
This is an academic logging and analytics lab. The report demonstrates ingestion and visualization of **NGINX access logs**, not a production security operations centre or a validated threat-detection system. The report says the Logstash pipeline code was obtained with chatbot assistance. Original executable pipeline files and datasets are not included in this repository.
