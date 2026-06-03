# OSINT Dorks

## Overview

Open Source Intelligence (OSINT) is the process of collecting, analyzing, and correlating information from publicly available sources.

OSINT is widely used by:

* Security Researchers
* Bug Bounty Hunters
* Threat Intelligence Analysts
* Investigators
* Journalists
* Developers
* System Administrators
* Researchers

Google Dorking is one of the most powerful OSINT techniques because search engines index enormous amounts of publicly accessible information across websites, documents, cloud resources, developer platforms, and organizational assets.

This guide focuses on using search operators to gather intelligence from publicly available sources in a lawful and ethical manner.

---

# What is OSINT?

OSINT stands for Open Source Intelligence.

It involves gathering information from sources such as:

* Websites
* Search Engines
* Documentation
* Public Reports
* Government Records
* Academic Research
* Social Media
* Developer Platforms
* Public Repositories
* Cloud Resources

OSINT does not involve unauthorized access.

The objective is to analyze information that is already publicly available.

---

# Why OSINT Matters

OSINT helps organizations and researchers:

## Security Research

* Understand attack surfaces
* Discover assets
* Map technologies

## Business Research

* Analyze competitors
* Study industries
* Understand markets

## Journalism

* Verify information
* Investigate events
* Gather evidence

## Academic Research

* Locate publications
* Find reports
* Access datasets

---

# OSINT Methodology

A structured OSINT investigation typically follows:

```text
Target Identification
          ↓
Information Collection
          ↓
Data Validation
          ↓
Correlation
          ↓
Analysis
          ↓
Reporting
```

---

# Core Search Operators

## site

Search within a specific domain.

### Example

```text
site:example.com
```

### Purpose

Restrict results to a target website.

---

## filetype

Search for specific file formats.

### Example

```text
filetype:pdf
```

### Purpose

Locate documents and reports.

---

## intitle

Search page titles.

### Example

```text
intitle:"report"
```

### Purpose

Find pages focused on specific topics.

---

## inurl

Search URL structures.

### Example

```text
inurl:blog
```

### Purpose

Locate specific content categories.

---

## before

Search content published before a date.

### Example

```text
site:example.com before:2025-01-01
```

### Purpose

Historical research.

---

## after

Search content published after a date.

### Example

```text
site:example.com after:2025-01-01
```

### Purpose

Recent information gathering.

---

# Organization Intelligence

Understanding an organization is often the first step.

## Basic Domain Research

### Query

```text
site:company.com
```

### Purpose

Discover publicly indexed assets.

### Potential Findings

* Products
* Services
* Portals
* Documentation

---

# Company Documentation Discovery

### Query

```text
site:company.com filetype:pdf
```

### Purpose

Find organizational documents.

### Possible Findings

* Whitepapers
* Reports
* Manuals
* Product Documentation

---

# Press Release Discovery

### Query

```text
site:company.com press release
```

### Purpose

Locate official announcements.

### Potential Findings

* Product Launches
* Acquisitions
* Partnerships
* Business Updates

---

# Annual Report Discovery

### Query

```text
site:company.com "annual report"
```

### Purpose

Understand company performance and strategy.

---

# Technology Intelligence

Organizations often reveal technology choices through public content.

## Engineering Blog Discovery

### Query

```text
site:company.com engineering
```

### Purpose

Research technical implementations.

### Potential Findings

* Architecture Discussions
* Infrastructure Design
* Development Practices

---

## Architecture Research

### Query

```text
site:company.com architecture
```

### Purpose

Discover infrastructure-related information.

---

## Cloud Technology Research

### Query

```text
site:company.com cloud
```

### Purpose

Identify cloud-related technologies.

---

# API Intelligence

Many organizations publish developer resources.

## API Discovery

### Query

```text
site:company.com api
```

### Purpose

Locate API documentation.

---

## Developer Portal Discovery

### Query

```text
site:company.com developer
```

### Purpose

Find developer resources.

---

## Swagger Documentation Discovery

### Query

```text
site:company.com swagger
```

### Purpose

Identify API documentation platforms.

---

# Domain Intelligence

Domains often reveal organizational structure.

## Subdomain Research

### Query

```text
site:*.company.com
```

### Purpose

Discover indexed subdomains.

### Possible Findings

* Blog Platforms
* Documentation Sites
* Support Systems
* Developer Portals

---

# Login Portal Discovery

### Query

```text
site:company.com login
```

### Purpose

Identify authentication-related assets.

### Possible Findings

* Customer Portals
* Account Dashboards
* Service Platforms

---

# Documentation Intelligence

Documents often provide deep insights.

## PDF Discovery

### Query

```text
site:company.com filetype:pdf
```

### Purpose

Locate publicly available documentation.

---

## Presentation Discovery

### Query

```text
site:company.com filetype:ppt
```

### Purpose

Find presentations and conference materials.

---

## Spreadsheet Discovery

### Query

```text
site:company.com filetype:xlsx
```

### Purpose

Locate public datasets and reports.

---

# Academic Intelligence

Universities publish vast amounts of information.

## Research Papers

### Query

```text
site:edu filetype:pdf research
```

### Purpose

Locate academic publications.

---

## Lecture Materials

### Query

```text
site:edu filetype:ppt
```

### Purpose

Find educational resources.

---

# Government Intelligence

Government websites contain public information.

## Government Reports

### Query

```text
site:gov filetype:pdf
```

### Purpose

Locate government publications.

---

## Regulations

### Query

```text
site:gov regulation
```

### Purpose

Find policy documents.

---

# News Intelligence

Search engines can assist with media research.

## Company News

### Query

```text
site:company.com news
```

### Purpose

Discover recent developments.

---

## Industry News

### Query

```text
industry keyword news
```

### Purpose

Track trends and developments.

---

# GitHub Intelligence

GitHub is a valuable OSINT source.

## Project Discovery

### Query

```text
filename:package.json
```

### Purpose

Find JavaScript projects.

---

## Infrastructure Research

### Query

```text
filename:Dockerfile
```

### Purpose

Study deployment methods.

---

## CI/CD Research

### Query

```text
path:.github/workflows
```

### Purpose

Analyze automation workflows.

---

# Cloud Intelligence

Cloud-related content reveals infrastructure trends.

## Cloud Discovery

### Query

```text
site:company.com cloud
```

### Purpose

Identify cloud adoption.

---

## Kubernetes Research

### Query

```text
site:company.com Kubernetes
```

### Purpose

Find cloud-native infrastructure references.

---

# Competitive Intelligence

Organizations often publish useful information.

## Product Research

### Query

```text
site:company.com product
```

### Purpose

Understand offerings and capabilities.

---

## Partner Discovery

### Query

```text
site:company.com partner
```

### Purpose

Identify strategic relationships.

---

# Historical Intelligence

Search operators can support timeline research.

## Historical Content

### Query

```text
site:company.com before:2022-01-01
```

### Purpose

View older indexed content.

---

## Recent Content

### Query

```text
site:company.com after:2025-01-01
```

### Purpose

Find recent publications.

---

# Complete OSINT Workflow

## Phase 1 — Domain Discovery

```text
site:company.com
```

---

## Phase 2 — Asset Mapping

```text
site:*.company.com
```

---

## Phase 3 — Documentation Collection

```text
site:company.com filetype:pdf
```

---

## Phase 4 — Technology Research

```text
site:company.com engineering
```

---

## Phase 5 — API Discovery

```text
site:company.com api
```

---

## Phase 6 — Reporting

Document:

* Domains
* Technologies
* Documentation
* Public Assets
* Findings

---

# Common OSINT Findings

Researchers frequently discover:

* Public Documentation
* Whitepapers
* Engineering Blogs
* Developer Portals
* APIs
* Product Information
* Cloud Technologies
* Public Reports
* Academic Resources
* Government Publications

---

# Best Practices

## Verify Information

Cross-reference findings with multiple sources.

## Maintain Documentation

Keep organized records of findings.

## Respect Privacy

Focus on publicly available information.

## Stay Ethical

Use OSINT techniques responsibly and lawfully.

## Validate Sources

Prefer official and authoritative sources whenever possible.

---

# OSINT Cheat Sheet

| Objective               | Query                          |
| ----------------------- | ------------------------------ |
| Find Domain Assets      | site:company.com               |
| Find PDFs               | site:company.com filetype:pdf  |
| Find APIs               | site:company.com api           |
| Find Docs               | site:company.com docs          |
| Find Login Pages        | site:company.com login         |
| Find Developer Portals  | site:company.com developer     |
| Find Engineering Blogs  | site:company.com engineering   |
| Find Cloud References   | site:company.com cloud         |
| Find Research Papers    | site:edu filetype:pdf research |
| Find Government Reports | site:gov filetype:pdf          |

---

# Summary

OSINT is the discipline of collecting and analyzing publicly available information to generate actionable intelligence. Search operators provide a powerful method for discovering websites, documents, reports, technologies, APIs, cloud resources, developer portals, and organizational assets.

By combining structured methodologies with advanced search operators, researchers can efficiently gather information, validate findings, and build a comprehensive understanding of a target while remaining within legal and ethical boundaries.
