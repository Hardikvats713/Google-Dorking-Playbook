# Bug Bounty Reconnaissance Workflow

## Overview

One of the most important skills in bug bounty hunting is reconnaissance.

Many successful findings originate not from advanced exploitation techniques but from a thorough understanding of the target's attack surface.

This document demonstrates how publicly available information and search operators can be used during an authorized bug bounty engagement to discover assets, documentation, technologies, APIs, and application components.

> This guide is intended for educational purposes and authorized security assessments only. Always ensure that your activities remain within the scope of the bug bounty program.

---

# Scenario

Assume a bug bounty program includes:

```text
example.com
*.example.com
```

Objective:

Build a complete inventory of publicly visible assets before performing any testing.

---

# Reconnaissance Methodology

```text
Scope Review
      ↓
Domain Discovery
      ↓
Subdomain Discovery
      ↓
Documentation Discovery
      ↓
Developer Portal Discovery
      ↓
API Discovery
      ↓
Technology Research
      ↓
Asset Mapping
      ↓
Prioritization
```

---

# Phase 1 — Scope Review

Before performing any reconnaissance:

## Verify

* Program rules
* Allowed targets
* Out-of-scope assets
* Reporting requirements

## Example

```text
In Scope:
example.com
*.example.com

Out of Scope:
Third-party services
Customer systems
```

---

# Phase 2 — Domain Discovery

## Goal

Understand what Google already knows about the target.

### Query

```text
site:example.com
```

### What This Reveals

Potentially:

```text
www.example.com
blog.example.com
support.example.com
docs.example.com
```

### Why Important

Provides an initial overview of public assets.

---

# Phase 3 — Subdomain Discovery

## Goal

Identify indexed subdomains.

### Query

```text
site:*.example.com
```

### Possible Results

```text
api.example.com
docs.example.com
support.example.com
careers.example.com
status.example.com
```

### Findings Table

| Asset               | Purpose        |
| ------------------- | -------------- |
| api.example.com     | APIs           |
| docs.example.com    | Documentation  |
| support.example.com | Support Portal |
| status.example.com  | Service Status |
| careers.example.com | Recruitment    |

### Why Important

Different subdomains often represent different applications.

---

# Phase 4 — Documentation Discovery

Documentation frequently reveals how systems work.

### Query

```text
site:example.com docs
```

### Possible Findings

```text
Developer Documentation
User Guides
Integration Guides
API References
```

---

## Alternative Query

```text
site:example.com filetype:pdf
```

### Possible Findings

```text
Architecture Documents
Technical Guides
Whitepapers
Product Manuals
```

### Why Important

Documentation often provides valuable context about application functionality and public interfaces.

---

# Phase 5 — Developer Portal Discovery

Many modern organizations provide developer resources.

### Query

```text
site:example.com developer
```

### Example Findings

```text
developers.example.com
developer.example.com
```

### Potential Information

* SDK Documentation
* Integration Guides
* Developer Dashboards
* API References

---

# Phase 6 — API Discovery

APIs are a critical component of modern applications.

## Query

```text
site:example.com api
```

### Example Findings

```text
api.example.com
developers.example.com/api
```

### Why Useful

Helps researchers understand:

* Application structure
* Public integrations
* Service architecture

---

## Swagger Discovery

### Query

```text
site:example.com swagger
```

### Possible Findings

```text
API Documentation
OpenAPI References
Developer Resources
```

---

## GraphQL Discovery

### Query

```text
site:example.com graphql
```

### Possible Findings

```text
GraphQL Documentation
Developer Guides
```

---

# Phase 7 — Authentication Surface Discovery

Authentication portals often indicate major application components.

## Query

```text
site:example.com login
```

### Possible Findings

```text
Customer Login
Admin Portal
Support Dashboard
Developer Access Portal
```

---

## Portal Discovery

### Query

```text
site:example.com portal
```

### Possible Findings

```text
Customer Portal
Partner Portal
Account Dashboard
```

---

# Phase 8 — Support Resource Discovery

Support portals frequently reveal application capabilities.

### Query

```text
site:example.com support
```

### Findings

```text
Knowledge Base
Help Center
Support Dashboard
```

### Why Useful

Support articles often explain workflows and features.

---

# Phase 9 — Technology Research

Organizations frequently discuss technologies publicly.

## Engineering Blog Discovery

### Query

```text
site:example.com engineering
```

### Potential Findings

```text
Infrastructure Articles
Technology Decisions
Architecture Discussions
```

---

## Cloud Research

### Query

```text
site:example.com cloud
```

### Potential Findings

```text
Cloud Migration Projects
Cloud Architecture Articles
Infrastructure Blogs
```

---

## Kubernetes Research

### Query

```text
site:example.com kubernetes
```

### Potential Findings

```text
Container Platforms
Cloud Native Systems
Deployment Discussions
```

---

# Phase 10 — File Discovery

Documents often contain valuable information.

## PDF Discovery

### Query

```text
site:example.com filetype:pdf
```

### Possible Findings

```text
Whitepapers
Reports
Guides
Documentation
```

---

## Presentation Discovery

### Query

```text
site:example.com filetype:ppt
```

### Possible Findings

```text
Technical Presentations
Conference Talks
Training Materials
```

---

# Phase 11 — GitHub Research

Many organizations maintain open-source projects.

## Query

```text
example organization github
```

### Possible Findings

```text
Open Source Projects
Developer Tools
SDKs
Libraries
```

### Why Useful

Public repositories can provide insight into:

* Development Practices
* Architecture Patterns
* Technology Choices

---

# Asset Inventory Creation

At this stage, findings should be documented.

## Example Inventory

| Asset                                     | Category         |
| ----------------------------------------- | ---------------- |
| [www.example.com](http://www.example.com) | Main Website     |
| api.example.com                           | API              |
| docs.example.com                          | Documentation    |
| support.example.com                       | Support          |
| status.example.com                        | Status Platform  |
| developer.example.com                     | Developer Portal |

---

# Prioritization

Not all assets deserve equal attention.

### High Priority

* APIs
* Developer Platforms
* Public Documentation
* Customer Applications

### Medium Priority

* Blogs
* Support Systems
* Status Pages

### Low Priority

* Marketing Pages
* Static Content

---

# Recon Notes Template

```text
Target:
example.com

Subdomains:
- api.example.com
- docs.example.com
- support.example.com

Documentation:
- API Docs
- User Guides

Developer Resources:
- SDK Documentation
- Integration Guides

Technologies:
- Cloud Platform
- Kubernetes
- API Gateway

Interesting Assets:
- Developer Portal
- Public API
- Support Dashboard
```

---

# Common Recon Findings

During authorized bug bounty reconnaissance, researchers frequently discover:

* APIs
* Developer Portals
* Documentation Sites
* Knowledge Bases
* Cloud Resources
* Support Systems
* Public Reports
* Open Source Projects

These findings help researchers better understand the target environment and identify areas for further authorized investigation.

---

# Best Practices

## Stay Within Scope

Only investigate assets explicitly included within the program.

## Remain Passive Initially

Begin with information gathering before any active testing.

## Document Everything

Maintain organized notes and inventories.

## Validate Findings

Verify information using official sources.

## Respect Program Rules

Follow all bug bounty policies and disclosure requirements.

---

# Summary

Successful bug bounty hunting begins with reconnaissance. Search engines, public documentation, developer resources, support portals, APIs, and technical content can provide valuable insight into an organization's publicly visible attack surface.

A structured reconnaissance process helps researchers build comprehensive asset inventories, understand application ecosystems, and prioritize authorized testing efforts more effectively.
