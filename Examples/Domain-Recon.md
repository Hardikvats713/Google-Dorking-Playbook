# Domain Reconnaissance Workflow

## Overview

Domain reconnaissance is the process of collecting information about a domain and its associated assets using publicly available sources.

A domain often acts as the central point for:

* Websites
* Applications
* APIs
* Documentation
* Support Platforms
* Developer Portals
* Cloud Resources
* Business Services

By performing structured reconnaissance, researchers can build an inventory of publicly visible assets and gain a better understanding of how an organization operates online.

This guide demonstrates a complete domain reconnaissance workflow using search operators and publicly available information.

> This guide is intended for educational, research, and authorized security assessment purposes only.

---

# Objective

Given a domain:

```text
example.com
```

Build a complete inventory of:

* Public Websites
* Subdomains
* Documentation
* APIs
* Developer Resources
* Support Platforms
* Cloud References
* Public Files
* Technology Information

---

# Domain Recon Methodology

```text
Domain Identification
          ↓
Asset Discovery
          ↓
Subdomain Discovery
          ↓
Documentation Discovery
          ↓
API Discovery
          ↓
Authentication Discovery
          ↓
Technology Research
          ↓
Cloud Research
          ↓
File Discovery
          ↓
Asset Inventory
```

---

# Phase 1 — Initial Domain Discovery

## Goal

Understand what search engines already know about the domain.

### Query

```text
site:example.com
```

### Purpose

Retrieve indexed pages belonging to the domain.

### Possible Findings

```text
www.example.com
about.example.com
support.example.com
blog.example.com
docs.example.com
```

### Why Important

Provides an initial overview of the organization's public footprint.

---

# Phase 2 — Website Structure Mapping

## Query

```text
site:example.com
```

Review discovered pages and categorize them.

### Example Asset Categories

| Asset                                     | Category        |
| ----------------------------------------- | --------------- |
| [www.example.com](http://www.example.com) | Main Website    |
| blog.example.com                          | Blog            |
| docs.example.com                          | Documentation   |
| support.example.com                       | Support         |
| status.example.com                        | Status Platform |

### Goal

Understand how services are organized.

---

# Phase 3 — Subdomain Discovery

Subdomains often reveal separate applications and services.

### Query

```text
site:*.example.com
```

### Purpose

Discover indexed subdomains.

### Possible Findings

```text
api.example.com
docs.example.com
support.example.com
status.example.com
careers.example.com
developer.example.com
```

### Why Important

Different subdomains frequently represent different business functions.

---

# Phase 4 — Documentation Discovery

Documentation often contains valuable technical information.

### Query

```text
site:example.com docs
```

### Purpose

Locate documentation resources.

### Possible Findings

```text
Product Documentation
User Guides
API References
Developer Documentation
```

---

## Alternative Query

```text
site:example.com documentation
```

### Purpose

Expand documentation coverage.

---

# Phase 5 — File Discovery

Search engines index many publicly available documents.

## PDF Discovery

### Query

```text
site:example.com filetype:pdf
```

### Possible Findings

```text
Whitepapers
Technical Guides
User Manuals
Case Studies
```

### Why Useful

Documents often contain more detailed information than webpages.

---

## Presentation Discovery

### Query

```text
site:example.com filetype:ppt
```

### Possible Findings

```text
Conference Presentations
Training Material
Technical Talks
```

---

## Spreadsheet Discovery

### Query

```text
site:example.com filetype:xlsx
```

### Possible Findings

```text
Public Reports
Datasets
Business Information
```

---

# Phase 6 — API Discovery

Many organizations expose public APIs.

## Query

```text
site:example.com api
```

### Purpose

Locate API-related resources.

### Possible Findings

```text
API Documentation
Developer Guides
Integration References
```

---

## Swagger Discovery

### Query

```text
site:example.com swagger
```

### Purpose

Find OpenAPI/Swagger documentation.

### Possible Findings

```text
API Explorer
Developer Documentation
OpenAPI Specifications
```

---

## GraphQL Discovery

### Query

```text
site:example.com graphql
```

### Purpose

Locate GraphQL resources.

---

# Phase 7 — Developer Portal Discovery

Developer platforms often contain valuable information.

### Query

```text
site:example.com developer
```

### Possible Findings

```text
Developer Portals
SDK Documentation
Integration Platforms
```

### Why Important

Developer resources often explain how products and services work.

---

# Phase 8 — Authentication Discovery

Authentication systems reveal major application components.

## Login Discovery

### Query

```text
site:example.com login
```

### Possible Findings

```text
Customer Login
Partner Login
Account Portal
```

---

## Portal Discovery

### Query

```text
site:example.com portal
```

### Possible Findings

```text
Customer Portals
Business Dashboards
Service Platforms
```

---

## Dashboard Discovery

### Query

```text
site:example.com dashboard
```

### Purpose

Identify application interfaces.

---

# Phase 9 — Support Ecosystem Discovery

Support systems frequently reveal business processes.

### Query

```text
site:example.com support
```

### Possible Findings

```text
Knowledge Base
Help Center
Support Portal
FAQs
```

---

## Knowledge Base Discovery

### Query

```text
site:example.com "knowledge base"
```

### Purpose

Locate detailed product information.

---

# Phase 10 — Blog Discovery

Blogs often reveal business and technical information.

### Query

```text
site:example.com blog
```

### Possible Findings

```text
Product Updates
Engineering Articles
Business Announcements
```

### Why Useful

Provides insight into organizational priorities and technologies.

---

# Phase 11 — Technology Research

Organizations frequently discuss technologies publicly.

## Engineering Research

### Query

```text
site:example.com engineering
```

### Possible Findings

```text
Architecture Discussions
Infrastructure Articles
Development Practices
```

---

## Architecture Discovery

### Query

```text
site:example.com architecture
```

### Purpose

Locate technical design information.

---

# Phase 12 — Cloud Research

Cloud technologies often appear in documentation and blogs.

## Cloud Discovery

### Query

```text
site:example.com cloud
```

### Possible Findings

```text
Cloud Infrastructure
Migration Projects
Cloud-Native Applications
```

---

## Kubernetes Discovery

### Query

```text
site:example.com kubernetes
```

### Possible Findings

```text
Container Platforms
Infrastructure Discussions
```

---

## DevOps Discovery

### Query

```text
site:example.com DevOps
```

### Purpose

Research deployment and operational practices.

---

# Phase 13 — Career Intelligence

Job listings often reveal technologies.

### Query

```text
site:example.com careers
```

### Possible Findings

```text
Engineering Roles
Cloud Roles
Security Roles
```

---

## Technology Research Through Careers

### Query

```text
site:example.com jobs AWS
```

### Query

```text
site:example.com jobs Kubernetes
```

### Query

```text
site:example.com jobs Python
```

### Purpose

Identify technologies currently used by the organization.

---

# Phase 14 — Public Report Discovery

Reports provide valuable organizational insight.

## Annual Reports

### Query

```text
site:example.com "annual report"
```

### Possible Findings

```text
Business Reports
Financial Information
Corporate Strategy
```

---

## Whitepaper Discovery

### Query

```text
site:example.com whitepaper
```

### Purpose

Locate technical and business publications.

---

# Asset Inventory Creation

After reconnaissance, document findings.

## Example Asset Inventory

| Asset                                     | Category         |
| ----------------------------------------- | ---------------- |
| [www.example.com](http://www.example.com) | Main Website     |
| api.example.com                           | API              |
| docs.example.com                          | Documentation    |
| support.example.com                       | Support          |
| blog.example.com                          | Blog             |
| developer.example.com                     | Developer Portal |
| status.example.com                        | Status Platform  |

---

# Recon Notes Template

```text
Target Domain:
example.com

Subdomains:
- api.example.com
- docs.example.com
- support.example.com

Documentation:
- User Guides
- API References

Developer Resources:
- Developer Portal
- SDK Documentation

Authentication:
- Login Portal
- Customer Dashboard

Technology Indicators:
- Cloud
- Kubernetes
- DevOps

Files:
- Whitepapers
- Technical Reports
```

---

# Common Findings

Domain reconnaissance frequently uncovers:

* Public Websites
* APIs
* Documentation
* Developer Platforms
* Support Systems
* Blogs
* Technical Reports
* Cloud References
* Authentication Portals
* Business Resources

---

# Best Practices

## Start Broad

Begin with general searches before narrowing scope.

## Organize Findings

Categorize discovered assets by function.

## Verify Information

Cross-reference findings with official sources.

## Focus on Public Information

Use only publicly accessible resources.

## Maintain Documentation

Create inventories and notes for future analysis.

---

# Domain Recon Cheat Sheet

| Objective                | Query                         |
| ------------------------ | ----------------------------- |
| Discover Assets          | site:example.com              |
| Find Subdomains          | site:*.example.com            |
| Find Documentation       | site:example.com docs         |
| Find APIs                | site:example.com api          |
| Find Developer Portals   | site:example.com developer    |
| Find Login Pages         | site:example.com login        |
| Find Support Systems     | site:example.com support      |
| Find PDFs                | site:example.com filetype:pdf |
| Find Cloud References    | site:example.com cloud        |
| Find Engineering Content | site:example.com engineering  |

---

# Summary

Domain reconnaissance is the foundation of OSINT, company research, and authorized security assessments. By systematically exploring a domain through search operators, researchers can discover websites, subdomains, documentation, APIs, support systems, developer resources, public documents, and technology indicators.

A structured workflow transforms scattered search results into a complete understanding of an organization's public digital footprint while remaining ethical, lawful, and evidence-based.
