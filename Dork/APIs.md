# API Discovery Dorks

## Overview

Application Programming Interfaces (APIs) are the backbone of modern applications. They allow different systems, applications, and services to communicate with one another.

Organizations commonly expose APIs for:

* Mobile Applications
* Web Applications
* Developer Platforms
* SaaS Products
* Internal Integrations
* Third-Party Services

Many APIs are publicly documented and indexed by search engines. Discovering these APIs can help researchers, developers, and security professionals better understand how an application functions.

This guide focuses on identifying publicly indexed API-related resources through search engines.

---

# Understanding API Discovery

API Discovery is the process of identifying:

* API Documentation
* Developer Portals
* Swagger/OpenAPI Specifications
* GraphQL Endpoints
* API References
* SDK Documentation
* Public API Gateways

## Why API Discovery Matters

API discovery can help:

### Developers

* Learn integration methods
* Find official documentation
* Understand endpoint structures

### Security Researchers

* Map application attack surfaces
* Understand application architecture
* Identify publicly documented services

### OSINT Analysts

* Discover exposed infrastructure
* Understand technology ecosystems
* Identify publicly available resources

---

# Common Search Operators

## site

Restricts results to a specific domain.

### Example

```text
site:example.com
```

### Purpose

Search only within a target domain.

---

## inurl

Searches for keywords within URLs.

### Example

```text
inurl:api
```

### Purpose

Find pages that contain API-related paths.

---

## intitle

Searches page titles.

### Example

```text
intitle:"API"
```

### Purpose

Locate API documentation pages.

---

## filetype

Searches for specific document formats.

### Example

```text
filetype:json
```

### Purpose

Find publicly available machine-readable files.

---

# API Documentation Discovery

Documentation is usually the first step in understanding an API.

## Example 1

```text
site:example.com inurl:docs
```

### What It Finds

Pages containing documentation resources.

### Possible Results

* User Guides
* API References
* Developer Documentation

### Example URL

```text
https://docs.example.com
```

---

## Example 2

```text
site:example.com intitle:"API Documentation"
```

### What It Finds

Pages whose titles explicitly reference API documentation.

### Why Useful

Provides direct access to developer resources.

---

# Developer Portal Discovery

Developer portals often contain:

* API Guides
* SDK Downloads
* Authentication Documentation
* Rate Limits
* Integration Examples

## Example

```text
site:example.com developer
```

### Possible Results

* Developer Portals
* Integration Hubs
* API Reference Centers

---

# Swagger Discovery

Swagger is one of the most widely used API documentation frameworks.

## Example

```text
site:example.com swagger
```

### Possible Findings

* Swagger UI
* OpenAPI Documentation
* Interactive API References

---

## Example

```text
site:example.com inurl:swagger
```

### Possible Findings

```text
/swagger
/swagger-ui
/swagger/index.html
```

---

# OpenAPI Discovery

OpenAPI specifications describe API structures.

## Example

```text
site:example.com "openapi"
```

### What It Finds

Pages referencing OpenAPI specifications.

---

## Example

```text
site:example.com filetype:json "openapi"
```

### What It Finds

Public JSON files containing OpenAPI definitions.

---

# GraphQL Discovery

GraphQL APIs are increasingly common.

## Example

```text
site:example.com graphql
```

### What It Finds

GraphQL documentation and references.

---

## Example

```text
site:example.com inurl:graphql
```

### Common Results

```text
/graphql
/graphql-api
/graphql/docs
```

---

# API Reference Discovery

Many organizations maintain dedicated API reference sections.

## Example

```text
site:example.com "API Reference"
```

### Purpose

Locate official endpoint documentation.

---

## Example

```text
site:example.com "REST API"
```

### Purpose

Identify REST API documentation.

---

# SDK Discovery

Software Development Kits often accompany APIs.

## Example

```text
site:example.com SDK
```

### Possible Findings

* Java SDK
* Python SDK
* Go SDK
* JavaScript SDK

---

# Authentication Documentation Discovery

Authentication documentation helps explain how APIs are accessed.

## Example

```text
site:example.com authentication api
```

### Possible Findings

* OAuth Documentation
* JWT Guides
* API Key Usage
* Access Control Information

---

# Postman Collection Discovery

Organizations frequently publish Postman collections.

## Example

```text
site:example.com postman
```

### Possible Findings

* Public API Collections
* Integration Examples
* Testing Resources

---

# Versioned API Discovery

Many APIs use versioning.

## Example

```text
site:example.com "v1"
```

## Example

```text
site:example.com "v2"
```

## Example

```text
site:example.com "v3"
```

### Purpose

Identify different API generations.

---

# API Search Combinations

## Documentation + API

```text
site:example.com inurl:docs api
```

### Use Case

Locate API documentation quickly.

---

## Swagger + API

```text
site:example.com swagger api
```

### Use Case

Locate Swagger-based documentation.

---

## Developer Portal + API

```text
site:example.com developer api
```

### Use Case

Discover official integration resources.

---

# Practical Workflow

## Step 1

Find Documentation

```text
site:example.com docs
```

## Step 2

Find Developer Resources

```text
site:example.com developer
```

## Step 3

Find API References

```text
site:example.com "API Reference"
```

## Step 4

Find Swagger/OpenAPI Resources

```text
site:example.com swagger
```

## Step 5

Find GraphQL Resources

```text
site:example.com graphql
```

---

# Common API Technologies

| Technology | Description                            |
| ---------- | -------------------------------------- |
| REST       | Resource-based APIs using HTTP         |
| GraphQL    | Query language for APIs                |
| SOAP       | XML-based API architecture             |
| OpenAPI    | API specification standard             |
| Swagger    | Interactive API documentation          |
| Postman    | API testing and collaboration platform |

---

# Best Practices

* Use search operators responsibly.
* Respect robots.txt and platform policies.
* Follow bug bounty program scopes.
* Validate findings through official documentation.
* Focus on publicly available resources.
* Never attempt unauthorized access.

---

# Summary

API discovery using search operators is a valuable technique for developers, researchers, and security professionals. By combining operators such as site:, inurl:, intitle:, and filetype:, users can efficiently locate documentation, developer portals, OpenAPI specifications, GraphQL references, and other publicly indexed API resources.

The goal of API discovery is understanding systems and improving visibility—not bypassing security controls or accessing unauthorized information.
