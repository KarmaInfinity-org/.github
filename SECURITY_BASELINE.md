# Karma Infinity Security Baseline

## Purpose

This file defines the minimum security posture expected for Karma Infinity repositories.

Security protects people, contributors, partners, data, infrastructure, reputation, and the long-term mission.

## Legal baseline

Security decisions must also follow `LEGAL.md`.

Karma Infinity is Karma Infinity LLC, a New Jersey limited liability company. Security, funding, grant, partnership, and public-benefit language must not imply nonprofit, 501(c)(3), tax-exempt, charitable, or tax-deductible donation status.

## Minimum repository security checklist

Every repository should be reviewed for:

- [ ] No secrets committed
- [ ] No credentials in examples, docs, screenshots, logs, issues, or pull requests
- [ ] `SECURITY.md` available through repo default or local override
- [ ] Pull request review required before merge when the repo becomes production-intended
- [ ] Branch protection or repository ruleset configured for `main`
- [ ] Dependabot alerts enabled where supported
- [ ] Dependabot security updates enabled where supported
- [ ] Dependabot version updates configured when dependencies exist
- [ ] Code scanning enabled when code exists and GitHub supports the language
- [ ] Secret scanning enabled where available
- [ ] Private data and sensitive logs excluded from the repo
- [ ] `.gitignore` covers local environment files and generated artifacts
- [ ] High-risk changes escalated for review

## Branch protection and rulesets

For production-intended repositories, protect `main` using branch protection or repository rulesets.

Recommended baseline:

- Require pull request before merging
- Require at least one approving review
- Dismiss stale approvals when new commits are pushed
- Require conversation resolution before merge
- Require status checks when tests or scans exist
- Block force pushes to `main`
- Block deletions of `main`
- Require signed commits where practical
- Restrict who can bypass protections

## Dependabot baseline

Use `.github/dependabot.yml` when the repository contains dependencies.

Recommended ecosystems to consider:

- `github-actions` for GitHub Actions workflows
- `npm` for JavaScript or TypeScript projects
- `pip` for Python projects
- `docker` for Dockerfiles
- `docker-compose` for Compose files
- `gomod` for Go projects
- `cargo` for Rust projects
- `bundler` for Ruby projects

Do not add package ecosystems that do not exist in the repository.

## Code scanning baseline

Enable code scanning when code exists and GitHub supports the repository language.

Recommended approach:

- Use GitHub CodeQL default setup when available
- Use language-specific tooling when CodeQL is not the best fit
- Treat findings as triage items, not automatic proof of exploitability
- Track unresolved high-risk findings before production use

## Secret handling

Never commit:

- API keys
- Passwords
- Private tokens
- Signing keys
- Certificates or private keys
- Service account files
- Database credentials
- OAuth secrets
- Production `.env` files
- User data exports
- Unredacted logs

If a secret is committed:

1. Rotate the secret immediately.
2. Remove it from current code.
3. Assess whether git history cleanup is needed.
4. Document the incident privately.
5. Review how it happened and add prevention.

## AI and automation security

AI agents, scripts, bots, and automated workflows require extra caution when they can:

- Read private data
- Write to files
- Open pull requests
- Send messages
- Execute code
- Deploy software
- Modify infrastructure
- Process health, legal, financial, crisis, or sensitive data

Before enabling action-taking automation, define:

- Scope
- Permissions
- Logs
- Kill switch
- Human review point
- Rollback path
- Data boundaries
- Abuse and misuse risks

## Data and privacy baseline

Repositories must not contain unnecessary personal data.

Before adding data, confirm:

- Why the data is needed
- Whether synthetic or anonymized data is safer
- Whether consent is required
- Whether deletion is possible
- Whether the data creates legal, privacy, or safety risk

## High-risk escalation

Escalate before merging or publishing changes involving:

- Authentication
- Authorization
- Payment workflows
- Personal or sensitive data
- Health, mental health, legal, financial, crisis, or safety systems
- AI agents with external actions
- Infrastructure or deployment credentials
- Public claims about security, compliance, impact, or outcomes
- Partnerships with schools, clinics, governments, nonprofits, or vulnerable populations

## Security review cadence

Recommended review rhythm:

- Before first public launch
- Before handling user data
- Before adding payments or external actions
- Before grants, partnerships, or public pilots
- Monthly for production-intended repositories
- After any security incident

## Maintainer rule

When uncertain, reduce permissions, remove secrets, slow down, and request review.
