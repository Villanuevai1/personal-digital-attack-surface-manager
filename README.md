# personal-digital-attack-surface-manager

# Personal Digital Attack Surface Manager (PDASM)

A web app that helps individuals understand and reduce their online security risk by tracking accounts (email, social, financial), security controls (MFA, password reuse), breach exposure, and producing a risk score over time.

## Why this exists
Most people have dozens of online accounts but no single view of their overall security posture. PDASM centralizes account security settings and highlights the highest-risk areas to fix first.

## Features
### User
- Register / login
- Add online accounts and categorize them (email/social/financial/etc.)
- Record security settings: MFA, password reuse, breach exposure
- View a dashboard with risk score + highest-risk accounts
- Update settings over time to track improvement

### Admin
- Manage platforms/categories (optional)
- Ensure data integrity and basic moderation (no access to user secrets)

## Risk Score (high level)
Risk score is computed from account security posture:
- No MFA increases risk
- Password reuse increases risk
- Breach exposure increases risk
- Certain categories (e.g., financial) have higher impact

See: `docs/05-risk-scoring.md`

## Tech Stack (planned)
- Frontend: React + Tailwind
- Backend: Flask (REST API)
- Database: SQLite (dev) / Postgres (prod)
- Deployment: AWS (EC2)

## Docs
- Project brief: `docs/00-project-brief.md`
- Requirements: `docs/01-requirements.md`
- Threat model: `docs/02-threat-model.md`
- Architecture: `docs/03-architecture.md`
- DB schema: `docs/04-database-schema.md`
- API spec: `docs/06-api-spec.md`
- Deployment: `docs/08-deployment.md`

## Screenshots
Screenshots are in `/screenshots`.

## Status
In progress (MVP).
