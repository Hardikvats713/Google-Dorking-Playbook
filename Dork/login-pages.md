# Login Page Discovery Dorks

## Overview

Login pages are one of the most common entry points into modern web applications. Organizations often maintain multiple authentication portals for customers, employees, partners, developers, and administrators.

Discovering publicly accessible login portals helps researchers, administrators, and security teams understand an organization's external-facing authentication surface.

This guide focuses on identifying publicly indexed authentication-related resources using search operators.

> Important: Discovery of login pages does not imply authorization to access or test them. Always follow applicable laws, organizational policies, and bug bounty program rules.

---

# What Are Login Pages?

Login pages are interfaces that allow users to authenticate into applications or services.

Common examples include:

* Customer Portals
* Employee Portals
* Partner Dashboards
* Support Systems
* Developer Platforms
* SaaS Applications
* Administrative Consoles
* Single Sign-On (SSO) Portals

---

# Why Login Page Discovery Matters

Login page discovery helps:

## Security Researchers

* Map authentication surfaces
* Identify public-facing applications
* Understand application ecosystems

## System Administrators

* Maintain asset inventories
* Verify exposed services
* Audit authentication portals

## OSINT Analysts

* Discover public services
* Understand organizational infrastructure

---

# Common Search Operators

## site

Restricts results to a specific domain.

### Example

```text
site:example.com
```

### Purpose

Search only within a target organization.

---

## intitle

Searches page titles.

### Example

```text
intitle:"login"
```

### Purpose

Find pages containing login-related titles.

---

## inurl

Searches URL paths.

### Example

```text
inurl:login
```

### Purpose

Locate URLs commonly associated with authentication.

---

## allintitle

Requires multiple keywords in page titles.

### Example

```text
allintitle: login portal
```

### Purpose

Locate portal-related login systems.

---

# Basic Login Page Discovery

## Query

```text
site:target.com login
```

### Purpose

Find pages containing the word "login".

### Possible Findings

* User Login Pages
* Customer Portals
* Application Entry Points

### Example

```text
site:example.com login
```

---

# Login Pages by Title

## Query

```text
site:target.com intitle:"login"
```

### Purpose

Locate pages with "Login" in the title.

### Why Useful

Many authentication systems clearly identify themselves through page titles.

---

# Sign-In Page Discovery

Many applications use "Sign In" rather than "Login".

## Query

```text
site:target.com intitle:"sign in"
```

### Purpose

Discover alternative authentication pages.

### Possible Findings

* SaaS Platforms
* Customer Dashboards
* Internal Portals

---

# Authentication Portal Discovery

## Query

```text
site:target.com authentication
```

### Purpose

Locate authentication-related documentation and systems.

### Possible Findings

* Login Guides
* Authentication Services
* Identity Management Resources

---

# Portal Discovery

Organizations frequently use portal-based authentication systems.

## Query

```text
site:target.com portal
```

### Purpose

Discover:

* Customer Portals
* Employee Portals
* Partner Portals

---

# Customer Portal Discovery

## Query

```text
site:target.com customer portal
```

### Purpose

Locate customer-facing service platforms.

### Possible Findings

* Account Management Systems
* Billing Portals
* Support Dashboards

---

# Employee Portal Discovery

## Query

```text
site:target.com employee
```

### Purpose

Identify employee-related services and documentation.

### Possible Findings

* HR Systems
* Employee Resources
* Internal Access Information

---

# Partner Portal Discovery

## Query

```text
site:target.com partner
```

### Purpose

Locate partner-facing services.

### Possible Findings

* Reseller Portals
* Business Dashboards
* Partner Resources

---

# Dashboard Discovery

Many applications use dashboard interfaces after authentication.

## Query

```text
site:target.com dashboard
```

### Purpose

Find references to application dashboards.

### Possible Findings

* User Dashboards
* Management Interfaces
* Reporting Systems

---

# Account Management Discovery

## Query

```text
site:target.com account
```

### Purpose

Locate account-related resources.

### Possible Findings

* Profile Management
* Account Settings
* User Services

---

# Single Sign-On (SSO) Discovery

Many organizations use centralized authentication systems.

## Query

```text
site:target.com SSO
```

### Purpose

Locate Single Sign-On references.

### Possible Findings

* Identity Platforms
* Login Documentation
* Access Management Systems

---

## Query

```text
site:target.com "single sign-on"
```

### Purpose

Find official SSO documentation and portals.

---

# Identity Provider Discovery

Organizations often document identity solutions.

## Query

```text
site:target.com identity
```

### Purpose

Locate identity management resources.

### Possible Findings

* Identity Documentation
* Authentication Systems
* Access Control Resources

---

# Support Login Discovery

Support platforms frequently require authentication.

## Query

```text
site:target.com support login
```

### Purpose

Locate customer support authentication portals.

### Possible Findings

* Ticket Systems
* Help Centers
* Customer Service Platforms

---

# Developer Portal Authentication

Developer platforms often provide dedicated login systems.

## Query

```text
site:target.com developer login
```

### Purpose

Discover developer access portals.

### Possible Findings

* API Platforms
* Developer Dashboards
* Integration Portals

---

# Mobile Platform Authentication

Organizations often provide separate mobile authentication systems.

## Query

```text
site:target.com mobile login
```

### Purpose

Locate mobile-related authentication resources.

---

# Authentication Documentation Discovery

## Query

```text
site:target.com authentication guide
```

### Purpose

Locate official authentication documentation.

### Possible Findings

* User Guides
* Login Procedures
* Security Documentation

---

# Knowledge Base Discovery

## Query

```text
site:target.com "login help"
```

### Purpose

Find support content related to authentication.

### Possible Findings

* Login Troubleshooting
* Account Recovery Guides
* User Assistance Articles

---

# Combined Search Techniques

## Login + Documentation

```text
site:target.com login documentation
```

### Goal

Understand authentication workflows.

---

## Login + Portal

```text
site:target.com login portal
```

### Goal

Locate portal entry points.

---

## Login + Dashboard

```text
site:target.com login dashboard
```

### Goal

Discover user-facing application interfaces.

---

## Authentication + Support

```text
site:target.com authentication support
```

### Goal

Locate authentication-related help resources.

---

# Reconnaissance Workflow

## Step 1

Identify Main Domain

```text
site:target.com
```

## Step 2

Locate Login Pages

```text
site:target.com login
```

## Step 3

Discover Portals

```text
site:target.com portal
```

## Step 4

Find Authentication Documentation

```text
site:target.com authentication
```

## Step 5

Map User Access Systems

```text
site:target.com dashboard
```

---

# Common Findings

Researchers frequently discover:

* Customer Login Pages
* User Dashboards
* Support Portals
* Developer Platforms
* Single Sign-On Systems
* Account Management Interfaces
* Authentication Documentation
* Knowledge Base Articles

These findings help create a comprehensive inventory of publicly accessible authentication-related assets.

---

# Best Practices

## Remain Within Scope

Only investigate assets covered by authorized programs or engagements.

## Respect Authentication Boundaries

Do not attempt unauthorized access to any system.

## Focus on Discovery

Use search operators to identify and document assets rather than interact with protected systems.

## Maintain Asset Inventories

Record:

* Login URLs
* Portal Types
* Authentication Technologies
* Documentation Resources

---

# Login Page Discovery Cheat Sheet

| Objective                | Query                             |
| ------------------------ | --------------------------------- |
| Find Login Pages         | site:target.com login             |
| Find Sign-In Pages       | site:target.com intitle:"sign in" |
| Find Portals             | site:target.com portal            |
| Find Dashboards          | site:target.com dashboard         |
| Find SSO Resources       | site:target.com SSO               |
| Find Authentication Docs | site:target.com authentication    |
| Find Customer Portals    | site:target.com customer portal   |
| Find Support Logins      | site:target.com support login     |
| Find Developer Access    | site:target.com developer login   |

---

# Summary

Login page discovery is an important aspect of asset inventory, OSINT, and authorized reconnaissance. By using search operators such as `site:`, `intitle:`, and `inurl:`, researchers can efficiently identify public authentication portals, user dashboards, support systems, developer platforms, and related documentation.

The purpose of login page discovery is to improve visibility into an organization's authentication ecosystem while respecting legal, ethical, and program-specific boundaries.
