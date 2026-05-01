# Security Policy

## Our commitment

Karma Infinity treats security as a responsibility to the people, communities, contributors, and partners who may rely on our systems.

Security issues should be handled carefully, privately, and quickly.

## Reporting a vulnerability

Do not open a public issue for a security vulnerability.

Use one of these private reporting paths:

- GitHub private vulnerability reporting, when enabled on the affected repository
- Email: security@karmainfinity.org

If the official security email changes, update this file immediately.

## What to include

Please include as much of the following as possible:

- A clear description of the vulnerability
- Affected repository, branch, package, endpoint, or file
- Steps to reproduce
- Potential impact
- Proof of concept, if safe to share
- Suggested mitigation, if known
- Your contact information for follow-up

Do not include exploit code beyond what is necessary to understand and reproduce the issue safely.

## What not to do

Please avoid:

- Accessing data that is not yours
- Disrupting services
- Exfiltrating secrets or personal information
- Social engineering contributors, maintainers, users, or partners
- Publicly disclosing the issue before maintainers have had a reasonable chance to respond

## Supported repositories

This organization-level policy applies by default to Karma Infinity repositories that do not define their own security policy.

Individual repositories may define additional version support windows, maintenance status, or reporting instructions.

## Response expectations

Karma Infinity will make a good-faith effort to:

- Acknowledge valid reports
- Investigate promptly
- Prioritize based on impact and exploitability
- Coordinate disclosure where appropriate
- Credit responsible reporters when requested and appropriate

Because the project is early-stage, formal response timelines may evolve as maintainer capacity grows.

## Severity guidance

| Severity | Examples |
|---|---|
| Critical | Remote code execution, credential exposure, privilege escalation, major data exposure |
| High | Authentication bypass, sensitive data leak, serious injection flaw |
| Medium | Cross-site scripting, insecure configuration, limited data exposure |
| Low | Minor information disclosure, best-practice hardening, low-impact misconfiguration |

## AI and automation security

If a vulnerability involves AI agents, prompts, automations, retrieval systems, generated code, or model outputs, include:

- Prompt or input used
- Expected safe behavior
- Actual unsafe behavior
- Impact on users, data, tools, or downstream actions
- Whether the issue can be repeated consistently

## Safe harbor

Karma Infinity supports good-faith security research that avoids harm, respects privacy, and follows this policy.

We will not pursue action against researchers who make reasonable efforts to comply with this policy and report issues responsibly.
