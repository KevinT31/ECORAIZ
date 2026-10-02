# ECORAIZ — Project Status

This page separates **implemented**, **validated locally**, **environment-dependent** and **pending** work so the showcase does not overstate production readiness.

## Implemented

- Public Next.js web application
- Protected CRM routes
- Protected Ecolytics route structure
- Supabase-auth integration code
- Role/profile checks
- RLS-oriented schema/migrations
- CRM entities and operational workflows
- Audit trail
- Manual assignment/reassignment flows
- Product/event tracking code
- PostgreSQL restore verification tooling
- CI quality checks
- Playwright browser tests
- Artifact generation/integrity checks

## Validated in the reviewed development environment

- Lint
- Build
- Typecheck
- Domain tests
- Database/RLS checks
- Logical backup/restore
- Artifact integrity
- PostHog configured/unconfigured test modes
- Existing browser flows
- Responsive/accessibility checks

## Environment-dependent

These areas need approved external accounts/configuration to be considered fully operational:

- production Supabase Auth validation
- real PostHog project
- private Metabase instance
- warehouse ingestion identity
- BigQuery dataset execution
- production dbt runs
- external WhatsApp runtime
- production legal/consent configuration

## Still pending / incomplete

- full production inventory transaction flows
- production quoting/separation/sales flows
- advanced automatic assignment and SLA logic
- executable production n8n workflows
- full operational warehouse ingestion
- final legal/operational approvals

## Showcase rule

Nothing in this public repository should be interpreted as claiming that pending integrations are live in production.
