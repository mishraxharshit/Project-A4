# Security Policy

The Project-A4 maintainers take the security of this ecosystem seriously. We appreciate responsible disclosure and will make every effort to acknowledge and address reports promptly.

## Supported Versions

| Version | Supported |
|---|---|
| `main` (latest) | ✅ |
| Older tagged releases | Evaluated case-by-case |

This table will be updated as versioned releases are published.

## Reporting a Vulnerability

**Please do not report security vulnerabilities through public GitHub issues.**

Instead:

1. Use GitHub's [private vulnerability reporting](../../security/advisories/new) feature for this repository, if enabled, **or**
2. Email the maintainers at a security contact address (to be published in [`GOVERNANCE.md`](GOVERNANCE.md) once established), including:
   - A description of the vulnerability and its potential impact
   - Steps to reproduce, or a proof of concept if available
   - Any suggested remediation

## What to Expect

- **Acknowledgment**: within a reasonable timeframe of the report being received.
- **Assessment**: maintainers will investigate and determine severity and scope.
- **Resolution**: a fix or mitigation will be prioritized based on severity; the reporter will be kept informed.
- **Disclosure**: once resolved, details may be published as a security advisory, with credit to the reporter unless they request anonymity.

## Scope

This policy covers code and infrastructure maintained directly in this repository. Vulnerabilities in third-party dependencies should generally be reported upstream as well.

## Research-Specific Considerations

Because this ecosystem includes research artifacts (data, models, experiment code), please also report:

- Data handling or privacy issues in shared datasets
- Reproducibility-breaking issues that could mislead downstream research
- Any content that could be misused to cause harm

These will be triaged alongside conventional security issues.
