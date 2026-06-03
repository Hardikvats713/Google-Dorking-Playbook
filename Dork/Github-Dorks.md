# GitHub Dorks

## Overview

GitHub is one of the largest repositories of source code, documentation, infrastructure configurations, automation workflows, and software projects in the world.

GitHub search operators allow users to efficiently discover:

* Open-source projects
* Configuration files
* Documentation
* CI/CD pipelines
* Infrastructure-as-Code examples
* API implementations
* Development frameworks
* Learning resources

GitHub Dorking refers to the use of GitHub's advanced search capabilities to locate specific files, repositories, technologies, and development patterns.

This guide focuses on educational, research, OSINT, and software engineering use cases.

---

# Why GitHub Dorking Matters

GitHub contains valuable information for:

## Developers

* Learn implementation patterns
* Discover code examples
* Find reusable solutions

## Security Researchers

* Understand application architectures
* Analyze public projects
* Research technologies

## DevOps Engineers

* Study infrastructure automation
* Review deployment workflows
* Explore CI/CD implementations

## Students

* Learn programming concepts
* Understand project structures
* Study real-world applications

---

# GitHub Search Basics

GitHub supports several search filters that help narrow results.

## filename

Search for a specific file name.

### Example

```text
filename:package.json
```

### Purpose

Find Node.js projects.

### Common Findings

* JavaScript Applications
* Frontend Projects
* Backend Services

---

## extension

Search by file extension.

### Example

```text
extension:yaml
```

### Purpose

Locate YAML-based configurations.

### Common Findings

* GitHub Actions
* Kubernetes Configurations
* CI/CD Pipelines

---

## path

Search within specific paths.

### Example

```text
path:.github/workflows
```

### Purpose

Locate automation workflows.

---

## language

Search repositories written in a specific language.

### Example

```text
language:python
```

### Purpose

Find Python projects.

---

## repo

Search within a specific repository.

### Example

```text
repo:owner/project
```

### Purpose

Analyze a particular project.

---

## user

Search repositories belonging to a user.

### Example

```text
user:octocat
```

### Purpose

Explore projects from a specific developer.

---

# Project Discovery

## JavaScript Projects

### Query

```text
filename:package.json
```

### Purpose

Discover Node.js applications.

### Why Useful

Most JavaScript applications contain a package.json file.

---

## Python Projects

### Query

```text
filename:requirements.txt
```

### Purpose

Locate Python projects.

### Possible Findings

* Flask Applications
* Django Projects
* Automation Scripts

---

## Java Projects

### Query

```text
filename:pom.xml
```

### Purpose

Find Maven-based Java applications.

---

## .NET Projects

### Query

```text
extension:csproj
```

### Purpose

Locate C# projects.

---

## Go Projects

### Query

```text
filename:go.mod
```

### Purpose

Discover Go-based applications.

---

# Docker Discovery

Docker is widely used for containerized deployments.

## Query

```text
filename:Dockerfile
```

### Purpose

Find containerized applications.

### Common Findings

* Deployment Examples
* Development Environments
* Application Containers

---

## Query

```text
filename:docker-compose.yml
```

### Purpose

Discover multi-container environments.

### Common Findings

* Local Development Stacks
* Microservice Architectures
* Database Integrations

---

# Kubernetes Discovery

Kubernetes configurations are often stored as YAML files.

## Query

```text
filename:deployment.yaml
```

### Purpose

Locate Kubernetes deployments.

---

## Query

```text
filename:service.yaml
```

### Purpose

Find Kubernetes service definitions.

---

## Query

```text
filename:ingress.yaml
```

### Purpose

Discover traffic routing configurations.

---

# GitHub Actions Discovery

GitHub Actions are commonly used for CI/CD.

## Query

```text
path:.github/workflows
```

### Purpose

Locate automation pipelines.

### Possible Findings

* Build Workflows
* Test Automation
* Deployment Pipelines

---

## Query

```text
path:.github/workflows language:yaml
```

### Purpose

Review workflow implementations.

---

# Infrastructure as Code Discovery

Infrastructure-as-Code (IaC) enables automated infrastructure management.

---

## Terraform

### Query

```text
extension:tf
```

### Purpose

Locate Terraform configurations.

### Common Findings

* AWS Infrastructure
* Azure Deployments
* Cloud Automation

---

## Query

```text
filename:main.tf
```

### Purpose

Find Terraform projects.

---

# Ansible Discovery

### Query

```text
filename:playbook.yml
```

### Purpose

Locate Ansible automation projects.

### Common Findings

* Server Automation
* Configuration Management
* Infrastructure Provisioning

---

# API Development Discovery

## OpenAPI Specifications

### Query

```text
filename:openapi.yaml
```

### Purpose

Find API specification files.

---

## Swagger Documentation

### Query

```text
swagger language:yaml
```

### Purpose

Discover API documentation examples.

---

# Documentation Discovery

Documentation often provides valuable learning resources.

## Query

```text
filename:README.md
```

### Purpose

Locate project documentation.

---

## Query

```text
filename:CONTRIBUTING.md
```

### Purpose

Learn contribution processes.

---

## Query

```text
filename:CHANGELOG.md
```

### Purpose

Review project evolution.

---

# Configuration File Discovery

## Nginx

### Query

```text
filename:nginx.conf
```

### Purpose

Study Nginx configurations.

---

## Apache

### Query

```text
filename:httpd.conf
```

### Purpose

Analyze Apache setups.

---

## Environment Examples

### Query

```text
filename:.env.example
```

### Purpose

Understand application configuration requirements.

---

# Framework Discovery

## React

### Query

```text
"react" filename:package.json
```

### Purpose

Find React projects.

---

## Next.js

### Query

```text
filename:next.config.js
```

### Purpose

Locate Next.js applications.

---

## Django

### Query

```text
filename:manage.py
```

### Purpose

Find Django projects.

---

## Flask

### Query

```text
"Flask" language:python
```

### Purpose

Discover Flask applications.

---

# DevOps Research

## CI/CD Implementations

### Query

```text
path:.github/workflows deployment
```

### Purpose

Research deployment pipelines.

---

## Monitoring Solutions

### Query

```text
prometheus filename:docker-compose.yml
```

### Purpose

Study monitoring environments.

---

## Logging Solutions

### Query

```text
elk filename:docker-compose.yml
```

### Purpose

Explore logging stack deployments.

---

# OSINT Applications

GitHub can be useful for:

* Technology Research
* Open Source Intelligence
* Architecture Analysis
* Development Workflow Research
* Learning Infrastructure Automation

---

# Practical Research Workflow

## Step 1

Identify Technology

```text
language:python
```

---

## Step 2

Find Real Projects

```text
filename:requirements.txt
```

---

## Step 3

Locate Deployment Methods

```text
filename:Dockerfile
```

---

## Step 4

Review CI/CD Workflows

```text
path:.github/workflows
```

---

## Step 5

Analyze Documentation

```text
filename:README.md
```

---

# Common Learning Opportunities

Researchers often discover:

* Project Structures
* Architecture Patterns
* DevOps Workflows
* Cloud Deployments
* Containerized Applications
* Infrastructure Automation
* CI/CD Pipelines
* Framework Best Practices

---

# Best Practices

## Respect Licensing

Always review repository licenses before reusing code.

## Attribute Sources

Provide proper credit when using open-source projects.

## Verify Code Quality

Review implementations carefully before adoption.

## Avoid Sensitive Information

Do not search for or use credentials, tokens, secrets, or other private information.

## Learn Responsibly

Use GitHub searches for education, research, development, and authorized security work.

---

# GitHub Dorks Cheat Sheet

| Objective             | Query                         |
| --------------------- | ----------------------------- |
| Find Node.js Projects | filename:package.json         |
| Find Python Projects  | filename:requirements.txt     |
| Find Docker Projects  | filename:Dockerfile           |
| Find Docker Compose   | filename:docker-compose.yml   |
| Find Terraform        | extension:tf                  |
| Find Kubernetes       | filename:deployment.yaml      |
| Find GitHub Actions   | path:.github/workflows        |
| Find OpenAPI Specs    | filename:openapi.yaml         |
| Find Nginx Configs    | filename:nginx.conf           |
| Find React Apps       | "react" filename:package.json |

---

# Summary

GitHub Dorking is a powerful technique for discovering open-source projects, development patterns, infrastructure automation, deployment workflows, and technology implementations. By leveraging search operators such as `filename:`, `extension:`, `path:`, `language:`, `repo:`, and `user:`, developers and researchers can efficiently explore the GitHub ecosystem and learn from real-world software projects.

The primary goal of GitHub Dorking should be knowledge acquisition, technology research, open-source collaboration, and responsible security research.
