# Lab 08 — Data Preparation, Elasticsearch Mapping & Kibana Analytics

**Course:** SRT411 — Digital Data Analytics  
**Tools:** Python, Logstash, Elasticsearch, Kibana, Excel/CSV  
**Evidence:** 20-page academic lab report (PDF to be uploaded separately)

## Overview

This lab documents an end-to-end analytics exercise using a public **liquor sales** dataset from Kaggle, described in the report as containing more than 100,000 rows and over 10 columns. Work included developing research questions, cleaning the data with Python, converting and ingesting data through Logstash, managing Elasticsearch index mappings and templates, querying records, and creating Kibana visualizations and a dashboard.

## Tasks completed

### 1. Data story and research questions
- Examined transaction fields describing sales amounts, product information, volumes, prices, dates, and store locations.
- Developed research questions about **geographic sales differences**, **product performance**, **time-based trends**, and **pricing versus sales**.
- Identified relevant quantitative and categorical fields for the analysis.

### 2. Cleaning and ingestion
- Documented a **Python data-cleaning script** for preparing the dataset.
- Configured a **Logstash pipeline** for importing and transforming CSV records into Elasticsearch.
- Reviewed Elasticsearch **index structure, settings, mappings, and an index template**.

### 3. Elasticsearch queries
- Queried documents with an item-description match for **"Vodka"**.
- Used a numerical range query to find sales records between **$50 and $100**.

### 4. Kibana visualizations and dashboard
Created a dashboard named **LIQUOR SALES**, documenting:
- Sales totals by vendor and by country.
- Bottles sold by city.
- Items ranked by median sales.
- Interactive filtering by **city** and by sales amount (for example, **$1,000–$5,000**).

### 5. Descriptive statistics
Reported and discussed **mean, mode, median, standard deviation, and variance** for sales-related fields, with an explanation of how each measure helps interpret the distribution. The report also discusses potential business insights and follow-up uses; these proposed insights should not be mistaken for independently validated causal relationships.

## Skills demonstrated

**Python Data Cleaning · CSV Processing · Logstash · Elasticsearch · Index Mapping · Index Templates · Query DSL · Kibana · Data Visualization · Dashboard Design · Filtering · Descriptive Statistics · Exploratory Data Analysis**

## Report evidence
- **Pages 3–6:** Dataset selection, variables, research questions and Python cleaning.
- **Pages 7–10:** Logstash data conversion, Elasticsearch index mapping and index templates.
- **Pages 11–12:** Elasticsearch searches.
- **Pages 12–17:** Visualizations, LIQUOR SALES dashboard and filters.
- **Pages 18–20:** Descriptive statistics and interpretation.

Upload `Lab 08 Manual.pdf` to this folder separately, and link it here.

## Scope and limitations

This is an **academic data analytics project**, not a production sales analytics platform or cybersecurity detection solution. The original Python script, source dataset and complete Logstash configuration are only shown in report screenshots and are not represented here as independently runnable files. The report’s exploratory business conclusions are presented as interpretations, not verified predictive results.
