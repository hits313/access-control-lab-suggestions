# Security Policy

Access Range (https://access-range.vercel.app) is a hands-on web-security
training platform. The lab content is intentionally vulnerable. The platform
that hosts it is not. This policy covers the hosting platform only.

## Reporting a vulnerability

If you believe you have found a real security issue in the platform itself,
report it privately first:

- Preferred: open a private security advisory at
  https://github.com/hits313/access-control-lab-suggestions/security/advisories/new
- Low-risk, non-sensitive issues may instead be filed as a public issue at
  https://github.com/hits313/access-control-lab-suggestions/issues

Please include a clear description, the affected URL or endpoint, reproduction
steps, and the impact. A minimal proof of concept helps us triage quickly.

Do not open a public issue for anything that exposes user data, secrets, or
allows account takeover. Use the private advisory channel for those.

## Scope

In scope (the platform shell):

- Account takeover, session hijacking, or handle theft
- Reading or modifying another user's data on the platform
- Tampering with solves, hints, or the leaderboard
- Stored or reflected injection on the platform shell (profile, leaderboard, settings)
- Bypassing the per-category unlock or anti-cheat in a way the labs do not intend
- Hosting or configuration mistakes that expose user data or secrets

Out of scope (the curriculum and expected behaviour):

- Anything under /labs, /steamish, /tradex, /pinsta, and /e/. These paths are the
  intentionally vulnerable training content.
- Self-XSS, or payloads pasted into your own browser console
- Public CVEs in dependencies without a working proof of concept on this platform
- Denial of service through traffic volume
- Social engineering, physical access, or network-layer attacks
- Issues in the underlying hosting provider

## Response targets

| Severity | First response | Fix target |
| --- | --- | --- |
| Critical | 24 hours | 7 days |
| High | 48 hours | 14 days |
| Medium | 72 hours | 30 days |
| Low | 72 hours | 60 days |

These are targets, not guarantees, for a community-run training project.

## Safe harbour

Test only against your own account. Do not access or retain another user's data
beyond the minimum needed to demonstrate impact. No destructive actions, no
traffic floods, no spam, no automated scanning that degrades the service.

If you make a good-faith effort to follow this policy, disclose privately, and
give us reasonable time to remediate, we will not pursue or support legal action
against you, and we are happy to credit you for the report.

## Disclosure

We follow coordinated disclosure. We will confirm the issue, keep you updated on
remediation, and agree a public disclosure date with you once a fix is deployed.
