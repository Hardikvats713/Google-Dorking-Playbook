# Cloud Assets Discovery Dorks

## Overview

Modern organizations heavily rely on cloud infrastructure to host applications, store files, deliver content, and provide services at scale.

Cloud assets may include:

* Cloud-hosted applications
* Storage services
* Content Delivery Networks (CDNs)
* API Gateways
* Static websites
* Documentation portals
* Developer resources
* Public cloud infrastructure

Many cloud-related resources are publicly documented or indexed by search engines. Understanding these assets helps security researchers, bug bounty hunters, developers, and OSINT analysts map an organization's technology ecosystem.

This guide focuses on identifying publicly indexed cloud resources using search operators.

---

# What Are Cloud Assets?

Cloud assets are resources hosted on cloud platforms such as:

| Provider        | Common Services                           |
| --------------- | ----------------------------------------- |
| AWS             | EC2, S3, CloudFront, API Gateway          |
| Microsoft Azure | Virtual Machines, Blob Storage, Azure CDN |
| Google Cloud    | Compute Engine, Cloud Storage, Cloud Run  |
| Cloudflare      | CDN, DNS, WAF                             |
| DigitalOcean    | Droplets, Spaces                          |
| Oracle Cloud    | Compute, Storage                          |
| IBM Cloud       | Virtual Servers, Storage                  |

---

# Why Cloud Asset Discovery Matters

Cloud asset discovery helps researchers:

* Understand application architecture
* Identify hosting providers
* Locate documentation
* Discover developer resources
* Map infrastructure components
* Improve attack surface visibility

Benefits include:

* Better reconnaissance
* Technology stack awareness
* Infrastructure understanding
* Asset inventory creation

---

# Search Operators Used

## site

Restricts results to a specific domain.

### Example

```text id="a1k39m"
site:example.com
```

### Purpose

Search only within a target organization.

---

## inurl

Search for keywords within URLs.

### Example

```text id="d7h2vn"
inurl:cloud
```

### Purpose

Locate cloud-related pages.

---

## intitle

Search page titles.

### Example

```text id="f9c8za"
intitle:"cloud"
```

### Purpose

Find cloud-focused resources.

---

## filetype

Search for specific document types.

### Example

```text id="k5q4tx"
filetype:pdf
```

### Purpose

Discover cloud architecture documents and guides.

---

# Cloud Infrastructure Discovery

## Example

```text id="m4rzj7"
site:target.com cloud
```

### Purpose

Locate cloud-related references.

### Possible Findings

* Cloud migration pages
* Infrastructure documentation
* Cloud service descriptions

### Why Useful

Provides insight into an organization's cloud strategy.

---

# Cloud Documentation Discovery

## Example

```text id="v8nyh1"
site:target.com cloud documentation
```

### Purpose

Find official cloud documentation.

### Possible Results

* Architecture guides
* Deployment instructions
* Technical references

---

# AWS Discovery

Amazon Web Services is one of the most widely used cloud providers.

## Example

```text id="n2qy4u"
site:target.com AWS
```

### What It Finds

Pages referencing AWS technologies.

### Potential Findings

* AWS migration stories
* Infrastructure blogs
* Technical documentation

---

## Example

```text id="p6kc0r"
site:target.com "Amazon Web Services"
```

### Purpose

Locate explicit AWS references.

---

# Azure Discovery

Microsoft Azure powers many enterprise environments.

## Example

```text id="g7yw3e"
site:target.com Azure
```

### Potential Findings

* Azure architecture references
* Deployment documentation
* Cloud migration content

---

## Example

```text id="j4tm8n"
site:target.com "Microsoft Azure"
```

### Purpose

Identify Azure-related infrastructure information.

---

# Google Cloud Discovery

## Example

```text id="l9ar5s"
site:target.com "Google Cloud"
```

### Purpose

Locate Google Cloud references.

### Possible Findings

* Cloud deployments
* Infrastructure discussions
* Engineering documentation

---

# Cloudflare Discovery

Cloudflare is commonly used for CDN and security services.

## Example

```text id="t3vk2f"
site:target.com Cloudflare
```

### Possible Findings

* Performance optimization content
* Security documentation
* Network architecture discussions

---

# CDN Discovery

Content Delivery Networks improve application performance.

## Example

```text id="u7ze6k"
site:target.com CDN
```

### Purpose

Find references to content delivery infrastructure.

### Potential Findings

* Performance guides
* Edge delivery systems
* Network architecture discussions

---

# Cloud Storage Research

Many organizations document cloud storage solutions.

## Example

```text id="x2hn8q"
site:target.com storage
```

### Possible Findings

* Storage architecture
* Backup documentation
* File hosting information

---

# Static Website Discovery

Organizations frequently host static websites in cloud environments.

## Example

```text id="b6pq4y"
site:target.com static site
```

### Purpose

Find references to cloud-hosted static resources.

---

# Cloud Migration Discovery

Organizations often publish migration case studies.

## Example

```text id="r4vj0c"
site:target.com migration
```

### Potential Findings

* Infrastructure transformation projects
* Cloud adoption journeys
* Technical architecture discussions

---

# DevOps Discovery

Cloud environments are closely connected with DevOps practices.

## Example

```text id="c5tm1w"
site:target.com DevOps
```

### Purpose

Discover operational and deployment-related information.

### Possible Findings

* CI/CD pipelines
* Automation discussions
* Infrastructure-as-Code references

---

# Kubernetes Discovery

Many cloud-native applications run on Kubernetes.

## Example

```text id="z9ev6n"
site:target.com Kubernetes
```

### Potential Findings

* Container orchestration guides
* Engineering blogs
* Architecture discussions

---

## Example

```text id="q8aw3f"
site:target.com k8s
```

### Purpose

Locate Kubernetes shorthand references.

---

# Container Technology Discovery

## Example

```text id="y1rc7j"
site:target.com Docker
```

### Purpose

Discover container-related resources.

### Potential Findings

* Deployment documentation
* Containerized architecture discussions

---

# Cloud Security Documentation

## Example

```text id="m0fj8k"
site:target.com cloud security
```

### Purpose

Locate security-focused cloud resources.

### Potential Findings

* Security whitepapers
* Compliance documentation
* Security architecture guides

---

# Architecture Documentation Discovery

## Example

```text id="w2na4s"
site:target.com architecture
```

### Purpose

Find technical architecture references.

### Potential Findings

* System design documents
* Infrastructure overviews
* Engineering diagrams

---

# Cloud Whitepaper Discovery

Organizations often publish detailed technical documents.

## Example

```text id="h6tv2e"
site:target.com filetype:pdf cloud
```

### Potential Findings

* Whitepapers
* Architecture documents
* Technical reports

---

# Engineering Blog Discovery

Engineering blogs frequently discuss cloud infrastructure.

## Example

```text id="k9ym7q"
site:target.com engineering cloud
```

### Purpose

Locate cloud implementation discussions.

---

# Public Resources Discovery

## Example

```text id="n4zw8m"
site:target.com resources cloud
```

### Potential Findings

* Technical resources
* Learning materials
* Public infrastructure documentation

---

# Cloud Technology Research Workflow

## Step 1

Identify Main Domain

```text id="s7px3v"
site:target.com
```

## Step 2

Find Cloud References

```text id="u8ar5k"
site:target.com cloud
```

## Step 3

Discover Documentation

```text id="w1tx9n"
site:target.com documentation
```

## Step 4

Research Technologies

```text id="z6hm4q"
site:target.com AWS
site:target.com Azure
site:target.com Kubernetes
```

## Step 5

Review Architecture Content

```text id="p5kr7c"
site:target.com architecture
```

---

# Common Findings

Researchers often discover:

* Cloud migration projects
* Architecture documentation
* Cloud provider references
* CDN technologies
* Kubernetes deployments
* Container platforms
* Infrastructure blogs
* Engineering resources

These findings help build a high-level understanding of an organization's cloud ecosystem.

---

# Best Practices

## Stay Within Scope

Only investigate assets that are explicitly included within an authorized engagement or bug bounty program.

## Focus on Public Information

Use publicly available resources and documentation.

## Verify Findings

Validate information through official sources whenever possible.

## Document Everything

Maintain notes regarding:

* Domains
* Cloud providers
* Technologies
* Documentation
* Architecture references

---

# Summary

Cloud asset discovery is an important component of modern reconnaissance. By leveraging search operators such as `site:`, `inurl:`, `intitle:`, and `filetype:`, researchers can locate publicly indexed cloud resources, documentation, architecture guides, and technology references.

Understanding an organization's cloud footprint helps improve asset visibility, technology awareness, and reconnaissance effectiveness while remaining within the boundaries of responsible and authorized research.
