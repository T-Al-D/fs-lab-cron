# fs-lab-cron

Centralized repository for cron jobs and scheduled workflows
used across fs-lab projects.

## Scope
This repository contains:
- GitHub Actions workflows
- Time-based benchmark and maintenance jobs

This repository does NOT contain:
- Application code
- Database schemas
- Secrets or credentials

## Principles
- Cron jobs run externally to avoid measurement bias
- Backends and databases are treated as passive targets
- All scheduling logic is versioned and reproducible
