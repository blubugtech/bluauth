# BluAuth

**BluAuth** is a self-hosted Identity and Access Management (IAM) platform built with **Java and Spring Boot**, designed as a Keycloak-like authentication and authorization solution.

It provides centralized user authentication, OAuth 2.0, OpenID Connect, JWT-based authentication, roles, groups, scopes, sessions, MFA, and authorization policies. BluAuth integrates with **BluKeys** for secure cryptographic key management and JWT signing.

## Tech Stack

- Java
- Spring Boot
- Spring Security
- Spring Authorization Server
- PostgreSQL
- Redis
- Docker
- Next.js
- Tailwind CSS

## Architecture

```mermaid
flowchart TD
    A[Applications] --> B[BluAuth]
    B -->|JWT Signing / Cryptographic Operations| C[BluKeys]
    B --> D[PostgreSQL]
    B --> E[Redis]
    C --> F[HSM]
````

## Ecosystem

```mermaid
flowchart LR
    A[Applications] --> B[BluAuth]
    B --> C[BluKeys]
    C --> D[Cryptographic Infrastructure]
```

> 🚧 BluAuth is currently under development.
