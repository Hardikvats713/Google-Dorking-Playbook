# Bug Bounty Reconnaissance Dorks

## Overview

Google Dorking is an effective passive reconnaissance technique used by bug bounty hunters and security researchers to discover publicly indexed assets belonging to an organization.

This document focuses on safe, authorized, and publicly available information that can help researchers:

* Understand an organization's attack surface
* Discover public-facing assets
* Locate documentation
* Identify APIs and developer resources
* Find technology-related information
* Map infrastructure components

> Important: Always ensure your activities comply with the target's bug bounty policy, scope, and applicable laws. Only test assets that are explicitly authorized.

---

# What Is Passive Reconnaissance?

Passive reconnaissance is the process of collecting information without directly interacting with target systems in a way that could impact them.

Examples include:

* Search engine research
* Documentation review
* Public asset discovery
* Technology stack identification
* Public repository analysis

Benefits:

* Low risk
* Non-intrusive
* Helps prioritize further investigation
* Builds a complete understanding of the target

---

# Recon Workflow

A typical bug bounty reconnaissance workflow:

```text
Target Selection
        ↓
Domain Discovery
        ↓
Subdomain Discovery
        ↓
Documentation Discovery
        ↓
API Discovery
        ↓
Technology Identification
        ↓
Attack Surface Mapping
```

---

# Domain Discovery

## Objective

Identify pages indexed under the target domain.

### Query

```text
site:target.com
```

### Purpose

Provides an overview of:

* Public webpages
* Service portals
* Support sections
* Documentation

### Example

```text
site:example.com
```

### What You Learn

* Website structure
* Public content
* Important business services

---

# Subdomain Discovery

Organizations often host services on multiple subdomains.

### Query

```text
site:*.target.com
```

### Purpose

Discover indexed subdomains.

### Example Results

```text
blog.target.com
docs.target.com
support.target.com
api.target.com
```

### Why Important

Subdomains frequently host:

* APIs
* Documentation
* Developer portals
* Customer services

---

# Documentation Discovery

Documentation reveals how systems are intended to operate.

### Query

```text
site:target.com docs
```

### Purpose

Find technical documentation.

### Possible Findings

* User guides
* Developer documentation
* Product manuals

### Why Useful

Documentation often provides valuable context about application functionality.

---

# Developer Portal Discovery

Many organizations maintain dedicated developer resources.

### Query

```text
site:target.com developer
```

### Purpose

Locate:

* Developer portals
* Integration guides
* SDK resources
* API documentation

### Example

```text
site:example.com developer
```

---

# API Discovery

APIs are often documented publicly.

### Query

```text
site:target.com api
```

### Purpose

Discover:

* API references
* Integration documentation
* Endpoint descriptions

### Example

```text
site:example.com api
```

---

# Swagger Discovery

Swagger/OpenAPI documentation is commonly indexed.

### Query

```text
site:target.com swagger
```

### Purpose

Locate API documentation systems.

### Example Findings

```text
Swagger UI
OpenAPI Documentation
API Explorer
```

### Research Value

Helps understand:

* Available endpoints
* Request formats
* Authentication mechanisms

---

# GraphQL Discovery

GraphQL services are increasingly common.

### Query

```text
site:target.com graphql
```

### Purpose

Find GraphQL-related resources.

### Example Findings

```text
GraphQL Documentation
GraphQL Guides
Developer References
```

---

# Support Portal Discovery

Support systems often expose useful product information.

### Query

```text
site:target.com support
```

### Purpose

Discover:

* Help centers
* Knowledge bases
* Support documentation

### Why Useful

Support resources frequently describe application features in detail.

---

# Knowledge Base Discovery

### Query

```text
site:target.com "knowledge base"
```

### Purpose

Locate product knowledge repositories.

### Potential Findings

* Product explanations
* Configuration guides
* Troubleshooting information

---

# Blog Discovery

Technical blogs often reveal implementation details.

### Query

```text
site:target.com blog
```

### Purpose

Discover engineering and product content.

### Potential Findings

* Architecture discussions
* Product announcements
* Technology stack insights

---

# Technology Research

Organizations frequently discuss technologies they use.

### Query

```text
site:target.com "engineering"
```

### Query

```text
site:target.com "architecture"
```

### Purpose

Understand:

* Infrastructure approaches
* Development practices
* Technology choices

---

# Public Asset Discovery

Search for publicly available assets.

### Query

```text
site:target.com assets
```

### Query

```text
site:target.com resources
```

### Purpose

Identify:

* Static resources
* Product assets
* Publicly available files

---

# Mobile Application Research

Organizations often publish mobile-related resources.

### Query

```text
site:target.com android
```

### Query

```text
site:target.com ios
```

### Purpose

Find:

* Mobile documentation
* Application guides
* Platform-specific resources

---

# Public PDF Discovery

PDF documents often contain valuable information.

### Query

```text
site:target.com filetype:pdf
```

### Possible Findings

* Whitepapers
* User manuals
* Product guides
* Technical documentation

### Research Value

Documents frequently provide deeper technical details than websites.

---

# Public Presentation Discovery

### Query

```text
site:target.com filetype:ppt
```

### Purpose

Locate presentations and conference materials.

### Potential Findings

* Product overviews
* Technical talks
* Training materials

---

# Job Posting Analysis

Job descriptions can reveal technologies in use.

### Query

```text
site:target.com careers
```

### Query

```text
site:target.com jobs
```

### Potential Findings

* Programming languages
* Cloud providers
* Security tools
* Infrastructure technologies

---

# Authentication Documentation Discovery

### Query

```text
site:target.com authentication
```

### Query

```text
site:target.com oauth
```

### Purpose

Find documentation describing:

* Login workflows
* Identity systems
* Authorization processes

---

# Version Discovery

Organizations often maintain multiple product versions.

### Query

```text
site:target.com "v1"
```

### Query

```text
site:target.com "v2"
```

### Query

```text
site:target.com "version"
```

### Purpose

Understand application evolution and supported releases.

---

# Recon Combination Examples

## API Documentation

```text
site:target.com api docs
```

### Goal

Locate API documentation quickly.

---

## Developer Resources

```text
site:target.com developer api
```

### Goal

Discover integration-related content.

---

## Technical Documentation

```text
site:target.com filetype:pdf documentation
```

### Goal

Find detailed technical documents.

---

## Engineering Content

```text
site:target.com engineering blog
```

### Goal

Research implementation details.

---

# Common Findings During Recon

Researchers often discover:

* Documentation portals
* Support centers
* Developer platforms
* Public APIs
* Product resources
* Technical blogs
* Knowledge bases
* Public documents

These findings help build an understanding of the target before conducting any authorized testing.

---

# Best Practices

## Always Verify Scope

Ensure discovered assets are included within the bug bounty program.

## Document Findings

Maintain notes regarding:

* Domains
* Subdomains
* Documentation
* APIs
* Technologies

## Remain Passive Initially

Start with public information gathering before any active testing.

## Respect Program Rules

Follow:

* Scope limitations
* Rate limits
* Responsible disclosure requirements

---

# Summary

Google Dorking is a valuable passive reconnaissance technique for bug bounty hunting. By using search operators such as `site:`, `inurl:`, `intitle:`, and `filetype:`, researchers can efficiently discover public assets, documentation, APIs, developer portals, and technical resources.

Effective reconnaissance improves understanding of the target environment and helps researchers focus their efforts on authorized, high-value areas of investigation while remaining compliant with program policies and applicable laws.
