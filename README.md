# fs-lab-cron

Centralized repository for cron jobs and scheduled workflows
used across fs-lab projects.

## Scope

This repository contains:

- GitHub Actions workflows
- External benchmark execution jobs
- Time-based data retention and maintenance tasks

This repository does NOT contain:

- Application code
- Database schemas
- Secrets or credentials

## Responsibilities

- Periodically benchmark backend health endpoints
- Store raw benchmark data in Supabase
- Enforce data retention policies (e.g. delete records older than 40 days)

## Principles

- Cron jobs run externally to avoid measurement bias
- Backends and databases are treated as passive measurement targets
- Only raw observations are written to the database
- Interpretation logic (e.g. cold vs warm) is handled outside of cron
- All scheduling logic is versioned and reproducible
