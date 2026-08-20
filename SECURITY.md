# Security Policy

## Reporting a Vulnerability

**Do not open a public issue for a security vulnerability.**

Report it privately, one of two ways:

1. **GitHub private advisory** *(preferred)* — on the affected repository, go to
   **Security → Report a vulnerability**. This keeps the report private until a fix ships.
2. **Email** — [security@slinttech.org](mailto:security@slinttech.org), or
   [admin@slinttech.org](mailto:admin@slinttech.org) if that does not reach you.

Please include:

- What the issue is and which repository or system it affects
- Steps to reproduce it
- What an attacker could do with it
- Any suggested fix, if you have one

## What to Expect

| Stage | Timeline |
| --- | --- |
| We acknowledge your report | within **3 business days** |
| We give you an initial assessment | within **10 business days** |
| We ship a fix or publish a mitigation | as fast as severity requires |

We will keep you updated as we work, and we will credit you in the advisory when the fix is
published — unless you ask us not to.

## Scope

In scope:

- Source code in any [@SLINT-Tech](https://github.com/SLINT-Tech) repository
- The `slinttech.org` website and any service we operate
- Exposed secrets, credentials, or personal data in our repositories

Out of scope:

- Third-party platforms we merely use (report those to the platform)
- Social-engineering our members or staff
- Volumetric denial-of-service testing

## Safe Harbour

If you research in good faith, follow this policy, avoid privacy violations and service
disruption, and give us reasonable time to fix the issue before disclosing it, we will not pursue
action against you.

We are a nonprofit and cannot currently pay bug bounties. We can offer public credit and our
genuine thanks.

## For SLINT Tech Members

If you commit a secret — an API key, a token, a password, a `.env` file — **tell us immediately**
at [security@slinttech.org](mailto:security@slinttech.org). Deleting the commit is not enough;
the credential must be rotated. Reporting it fast is never punished. Hiding it is.
