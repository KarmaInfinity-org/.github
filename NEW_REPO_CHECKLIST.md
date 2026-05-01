# Karma Infinity New Repository Checklist

## Purpose

Use this checklist before creating or launching any new Karma Infinity repository.

The goal is to keep every repository elite, consistent, secure, legally accurate, accessible, and mission-aligned from day one.

## Phase 1: Define the repository

- [ ] Repository name is clear, lowercase, and hyphenated
- [ ] Repository purpose is specific
- [ ] Repository owner or maintainer is identified
- [ ] Project status is clear: concept, planning, prototype, experimental, preview, production, or archived
- [ ] Legal status is clear: Karma Infinity LLC, New Jersey limited liability company
- [ ] Repository does not imply nonprofit, charity, 501(c)(3), tax-exempt, public charity, or foundation status
- [ ] Funding language is LLC-safe

## Phase 2: Create the repository

- [ ] Create repository under KarmaInfinity-org
- [ ] Choose visibility intentionally: public or private
- [ ] Set default branch to `main`
- [ ] Add short description
- [ ] Add relevant topics
- [ ] Add README
- [ ] Add license if the repo contains reusable code, docs, data, or creative assets
- [ ] Add `.gitignore` appropriate to the stack

## Phase 3: Required documentation

- [ ] `README.md` explains what the repo is and why it exists
- [ ] README includes project status
- [ ] README includes setup instructions when applicable
- [ ] README includes usage instructions when applicable
- [ ] README includes legal-status note or links to `LEGAL.md`
- [ ] README includes security/privacy/accessibility notes when applicable
- [ ] README links to contribution, support, security, and license files
- [ ] Local policy files are added only when the default `.github` files are not enough

## Phase 4: Legal and compliance review

- [ ] No nonprofit, charity, public charity, foundation, tax-exempt, or 501(c)(3) claims
- [ ] No tax-deductible donation claims
- [ ] No donation language unless legally reviewed and documented
- [ ] Grant language confirms LLC eligibility when relevant
- [ ] Public benefit language does not imply nonprofit status
- [ ] Health, mental health, legal, financial, crisis, or safety claims are reviewed
- [ ] User-data handling is reviewed before any data collection
- [ ] Terms, privacy, consent, disclaimers, and contracts are reviewed when needed

## Phase 5: Security setup

- [ ] `SECURITY.md` available by default or local override
- [ ] `main` protected with branch protection or ruleset when production-intended
- [ ] Pull request review required before merge when appropriate
- [ ] Force pushes blocked on `main`
- [ ] Branch deletion blocked on `main`
- [ ] Required checks added when tests/scans exist
- [ ] Secret scanning enabled where available
- [ ] Dependabot alerts enabled where supported
- [ ] Dependabot security updates enabled where supported
- [ ] Code scanning enabled when code exists and language support is available
- [ ] `.github/dependabot.yml` added when dependencies exist
- [ ] No secrets in repository history

## Phase 6: Contribution workflow

- [ ] Issue templates inherited or local templates added
- [ ] Pull request template inherited or local template added
- [ ] CODEOWNERS configured when team structure exists
- [ ] Standard labels created
- [ ] `good first issue` and `help wanted` only used when maintainers can respond
- [ ] AI-assisted contribution disclosure remains in PR template

## Phase 7: Accessibility and user impact

- [ ] User-facing interfaces consider keyboard access
- [ ] User-facing interfaces consider screen reader support
- [ ] Color contrast is considered
- [ ] Mobile usability is considered
- [ ] Clear language is used
- [ ] Captions or alternatives are provided for media when relevant
- [ ] Reduced-motion needs are considered when animations exist

## Phase 8: AI and automation review

- [ ] AI-assisted content is human-reviewed
- [ ] AI agents have scoped permissions
- [ ] Action-taking automation has a human review point
- [ ] Automation has a kill switch or rollback path
- [ ] Data boundaries are documented
- [ ] Prompt injection and misuse risks are considered
- [ ] External messaging, payments, deployments, or file writes are reviewed

## Phase 9: Launch readiness

- [ ] README is accurate
- [ ] License is present and appropriate
- [ ] Security policy is discoverable
- [ ] Legal status is accurate
- [ ] Funding language is safe
- [ ] Branch protection or rulesets are configured when needed
- [ ] Labels exist
- [ ] Initial issues or roadmap exist
- [ ] Maintainer knows the next three actions

## Phase 10: Post-launch maintenance

- [ ] Review open issues weekly during active development
- [ ] Review dependencies monthly or when alerts appear
- [ ] Review security posture before public demos or pilots
- [ ] Review legal language before funding, grant, investor, or partnership outreach
- [ ] Archive stale experimental repos when they are no longer active

## Maintainer rule

If the repository touches people, money, data, public claims, security, health, mental health, legal, financial, crisis, education, children, or vulnerable populations, slow down and request review before launch.
