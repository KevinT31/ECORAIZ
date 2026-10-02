# ECORAIZ — Architecture Notes

## System Boundaries

The public showcase intentionally separates three surfaces:

1. **Public Website** — commercial discovery and customer-facing content.
2. **CRM** — authenticated operational workflows.
3. **Ecolytics** — authenticated analytics and reporting capabilities.

## Logical Flow

```mermaid
flowchart TB
    Public[Public User] --> Website[Next.js Website]
    Team[Authorized Team] --> Auth[Authentication]

    Auth --> CRM
    Auth --> Ecolytics

    Website --> Domain[Shared Domain Contracts]
    CRM --> Domain
    Ecolytics --> Domain

    Domain --> Data[Supabase / Data Services]
    Website --> Telemetry[Product Analytics]
    CRM --> Automation[Automation Workflows]

    CI[CI Checks] --> Deploy[Vercel]
    Website --> Deploy
```

## Design Considerations

- Public and internal functionality are intentionally separated.
- Authentication protects operational functionality.
- Business data and infrastructure details are not published in this showcase.
- CI validates application quality before deployment.
- Product analytics are treated as a first-class part of the product architecture.
