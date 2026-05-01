# Karma Infinity Repository Standards

## Purpose

This file defines the default repository operating standard for Karma Infinity.

Every Karma Infinity repository should be created, configured, documented, and maintained with the same baseline of legal accuracy, security, accessibility, contribution quality, and mission alignment.

## Legal baseline

Every repository must treat Karma Infinity as:

```text
Karma Infinity LLC = New Jersey limited liability company
Karma Infinity LLC != nonprofit
Karma Infinity LLC != 501(c)(3)
Karma Infinity LLC != tax-exempt charitable organization
Karma Infinity LLC != public charity
Karma Infinity LLC != private foundation
```

Required reference:

```text
LEGAL.md
```

Do not use donation, charitable donation, tax-deductible donation, nonprofit donation, public charity, foundation, or 501(c)(3) language unless a qualified legal structure is formally established, reviewed, and documented.

## Repository naming standard

Use clear, lowercase, hyphenated names.

Recommended examples:

```text
karma-command-center
karma-ai-agents
karma-web
karma-api
karma-docs
karma-impact-metrics
karma-accessibility-lab
karma-security-baseline
karma-studios
```

Avoid names that are vague, overly broad, or imply regulated services before review.

## Required root files for product repositories

Every production-intended repository should include:

```text
README.md
LICENSE
.gitignore
CONTRIBUTING.md or inherited default
CODE_OF_CONDUCT.md or inherited default
SECURITY.md or inherited default
SUPPORT.md or inherited default
LEGAL.md or link to organization default
.github/PULL_REQUEST_TEMPLATE.md or inherited default
.github/ISSUE_TEMPLATE/ or inherited default
.github/dependabot.yml when dependencies exist
```

## README standard

Every repository README should include:

- What the repository is
- Why it exists
- Current status
- Legal status note for Karma Infinity LLC
- Installation or setup instructions
- Usage examples, when applicable
- Security and privacy notes
- Accessibility notes, when user-facing
- Contribution link
- License link
- Maintainer or ownership information

## Status labels

Use honest project status language:

- `concept`
- `planning`
- `prototype`
- `experimental`
- `internal-preview`
- `public-preview`
- `production`
- `archived`

Do not imply that an experimental system is production-ready.

## Branching standard

Default branch:

```text
main
```

Recommended branch names:

```text
feat/short-description
fix/short-description
docs/short-description
security/short-description
legal/short-description
governance/short-description
chore/short-description
```

## Commit standard

Recommended format:

```text
type(scope): short description
```

Examples:

```text
docs(readme): add legal status note
security(config): add dependabot template
legal(status): clarify LLC funding language
feat(api): add health endpoint
fix(ui): improve keyboard navigation
```

Recommended types:

- `feat`
- `fix`
- `docs`
- `chore`
- `refactor`
- `test`
- `security`
- `legal`
- `governance`
- `accessibility`

## Pull request standard

Every meaningful change should go through a pull request unless it is an emergency maintainer correction.

Pull requests should include:

- Summary
- Related issue
- What changed
- Review/test steps
- Risk review
- Legal-status and funding-language review
- AI-assisted work disclosure, if applicable
- Security/privacy/accessibility considerations

## Issue standard

Issues should be actionable and use the default templates whenever possible.

Blank issues should remain disabled unless maintainers decide otherwise.

## Security standard

Repositories should follow `SECURITY_BASELINE.md`.

At minimum:

- No secrets in code, issues, logs, screenshots, comments, or documentation
- Dependency scanning strategy when dependencies exist
- Dependabot configuration when package ecosystems exist
- Security policy available through default `SECURITY.md`
- Pull request review required for sensitive changes
- Legal/security/privacy escalation for regulated or high-risk work

## Accessibility standard

User-facing tools and documents should consider:

- Clear language
- Keyboard navigation
- Screen reader support
- Color contrast
- Mobile usability
- Captions or alternatives for media
- Reduced motion when appropriate
- Meaningful headings and labels

## AI-assisted work standard

AI-assisted work is allowed when reviewed by a human.

Review AI-assisted work for:

- Accuracy
- Legal-status mistakes
- Security issues
- Privacy issues
- Accessibility issues
- Hallucinated citations
- Unsupported claims
- Licensing concerns
- Bias or harmful assumptions
- Maintainability

## High-risk work requires review

Escalate before publishing or merging changes involving:

- Health, mental health, legal, financial, crisis, or safety-related content
- Grants, funding, investment, sponsorship, tax, or public-benefit language
- Sensitive personal information
- Children, schools, clinics, governments, or vulnerable populations
- AI agents that take external actions
- Payment flows
- Public claims about impact, research, or outcomes
- Security-sensitive infrastructure

## Maintainer rule

If a change is unclear, sensitive, or potentially harmful, slow down, document the concern, and request review.
