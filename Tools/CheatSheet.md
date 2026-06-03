# GOOGLE DORKING PLAYBOOK

## Quick Reference Cheat Sheet

Version 1.0

---

# Table of Contents

1. Introduction
2. Core Search Operators
3. Operator Combinations
4. File Discovery
5. API Discovery
6. Login Page Discovery
7. Cloud Asset Discovery
8. GitHub Discovery
9. OSINT Workflow
10. Bug Bounty Recon Workflow
11. Quick Reference Tables
12. Best Practices

---

# What is Google Dorking?

Google Dorking is the use of advanced search operators to locate specific publicly indexed information.

Applications:

* OSINT
* Research
* Bug Bounty Reconnaissance
* Documentation Discovery
* Asset Discovery
* Competitive Analysis
* Academic Research

---

# Core Search Operators

## site:

Search within a specific website.

### Syntax

```text
site:example.com
```

### Example

```text
site:example.com
```

### Purpose

Find all indexed pages belonging to a domain.

---

## filetype:

Search for specific file formats.

### Syntax

```text
filetype:pdf
```

### Example

```text
site:example.com filetype:pdf
```

### Purpose

Locate documents and reports.

---

## intitle:

Search page titles.

### Example

```text
intitle:"documentation"
```

### Purpose

Find pages with specific titles.

---

## inurl:

Search URL structures.

### Example

```text
inurl:docs
```

### Purpose

Locate pages containing specific keywords in URLs.

---

## before:

Search older content.

### Example

```text
site:example.com before:2024-01-01
```

---

## after:

Search recent content.

### Example

```text
site:example.com after:2024-01-01
```

---

# Operator Combination Examples

## Documentation

```text
site:example.com docs
```

---

## APIs

```text
site:example.com api
```

---

## Developer Portals

```text
site:example.com developer
```

---

## Support Systems

```text
site:example.com support
```

---

## Login Pages

```text
site:example.com login
```

---

# File Discovery

## PDF Files

```text
site:example.com filetype:pdf
```

Find:

* Whitepapers
* Manuals
* Reports
* Technical Documentation

---

## Presentations

```text
site:example.com filetype:ppt
```

Find:

* Training Material
* Conference Talks
* Product Demonstrations

---

## Spreadsheets

```text
site:example.com filetype:xlsx
```

Find:

* Public Reports
* Datasets
* Business Information

---

# API Discovery

## General API Search

```text
site:example.com api
```

---

## Swagger

```text
site:example.com swagger
```

---

## GraphQL

```text
site:example.com graphql
```

---

## Developer Resources

```text
site:example.com developer
```

---

# Login Page Discovery

## Login Pages

```text
site:example.com login
```

---

## Sign In Pages

```text
site:example.com intitle:"sign in"
```

---

## Portals

```text
site:example.com portal
```

---

## Dashboards

```text
site:example.com dashboard
```

---

# Cloud Asset Discovery

## Cloud References

```text
site:example.com cloud
```

---

## AWS References

```text
site:example.com AWS
```

---

## Azure References

```text
site:example.com Azure
```

---

## Kubernetes References

```text
site:example.com kubernetes
```

---

## DevOps References

```text
site:example.com DevOps
```

---

# GitHub Dorks

## Node.js Projects

```text
filename:package.json
```

---

## Python Projects

```text
filename:requirements.txt
```

---

## Docker Projects

```text
filename:Dockerfile
```

---

## Docker Compose

```text
filename:docker-compose.yml
```

---

## Terraform

```text
extension:tf
```

---

## Kubernetes

```text
filename:deployment.yaml
```

---

## GitHub Actions

```text
path:.github/workflows
```

---

# OSINT Workflow

```text
Target
   ↓
Domain Discovery
   ↓
Subdomain Discovery
   ↓
Documentation Discovery
   ↓
API Discovery
   ↓
Technology Research
   ↓
Asset Mapping
   ↓
Reporting
```

---

# Domain Recon Workflow

## Step 1

```text
site:example.com
```

Discover assets.

---

## Step 2

```text
site:*.example.com
```

Discover subdomains.

---

## Step 3

```text
site:example.com docs
```

Find documentation.

---

## Step 4

```text
site:example.com api
```

Find APIs.

---

## Step 5

```text
site:example.com login
```

Identify authentication portals.

---

# Company Recon Workflow

## Research Products

```text
site:example.com product
```

---

## Research Services

```text
site:example.com services
```

---

## Research Technologies

```text
site:example.com engineering
```

---

## Research Cloud

```text
site:example.com cloud
```

---

## Research Careers

```text
site:example.com careers
```

---

# Bug Bounty Recon Workflow

## Phase 1

Discover Assets

```text
site:target.com
```

---

## Phase 2

Find Subdomains

```text
site:*.target.com
```

---

## Phase 3

Find Documentation

```text
site:target.com docs
```

---

## Phase 4

Find APIs

```text
site:target.com api
```

---

## Phase 5

Build Asset Inventory

---

# Quick Reference Table

| Objective              | Query                         |
| ---------------------- | ----------------------------- |
| Find Assets            | site:example.com              |
| Find Subdomains        | site:*.example.com            |
| Find Docs              | site:example.com docs         |
| Find PDFs              | site:example.com filetype:pdf |
| Find APIs              | site:example.com api          |
| Find Swagger           | site:example.com swagger      |
| Find GraphQL           | site:example.com graphql      |
| Find Login Pages       | site:example.com login        |
| Find Dashboards        | site:example.com dashboard    |
| Find Support           | site:example.com support      |
| Find Developer Portals | site:example.com developer    |
| Find Cloud References  | site:example.com cloud        |
| Find AWS References    | site:example.com AWS          |
| Find Kubernetes        | site:example.com kubernetes   |
| Find GitHub Actions    | path:.github/workflows        |

---

# Best Practices

✓ Verify findings using official sources

✓ Document discoveries systematically

✓ Focus on publicly available information

✓ Respect program scope and policies

✓ Use findings for education, research, and authorized assessments

✓ Cross-reference information whenever possible

---

# Common Mistakes

✗ Assuming indexed information is current

✗ Relying on a single source

✗ Ignoring documentation

✗ Failing to organize findings

✗ Performing activities outside authorized scope

---

# Notes Section

Target:

---

Assets:

---

Documentation:

---

APIs:

---

Technologies:

---

Interesting Findings:

---

---

Google Dorking Playbook
Quick Reference Guide
Version 1.0
