# Micronaut Security Disclosure Policy

The goal of this policy is to responsibly disclose security vulnerabilities to minimize exposure windows.

This policy describes the steps to follow if a security advisory is reported against Micronaut code. Every active, non-archived repository that publishes components to Maven Central or is hosted publicly on GitHub is in scope.

The embargo window is 45 days.

## Intake

Security advisories for framework components are reported via the [GitHub Security Advisory UI](https://docs.github.com/en/code-security/how-tos/report-and-fix-vulnerabilities/fix-reported-vulnerabilities/creating-a-repository-security-advisory#creating-a-security-advisory). Publicly known security problems, including CVEs, do not fall under the embargo because they are already public, and they will be patched immediately.

## Triage

- The [Micronaut core development team](https://github.com/orgs/micronaut-projects/teams/core-developers) reviews the security advisory.

- The [Micronaut core development team](https://github.com/orgs/micronaut-projects/teams/core-developers) attempts to reproduce the issue and verifies that it is indeed a valid security advisory.

- Advisories with a [CVSS 3.1](https://www.first.org/cvss/calculator/3.1) score > 4.0 (Medium and above) enter the embargo period.

- The [Micronaut core development team](https://github.com/orgs/micronaut-projects/teams/core-developers) will acknowledge receipt of the advisory within 5 business days. After triaging the issue, the [Micronaut core development team](https://github.com/orgs/micronaut-projects/teams/core-developers) will notify the reporter of the outcome and tell them:
  - The reporter will be credited via the GitHub UI.
  - The reporter should respect the embargo window and avoid discussing the security advisory publicly before the public patch date, which will be 45 days after the report (the end of the embargo window).
- The [Micronaut core development team](https://github.com/orgs/micronaut-projects/teams/core-developers) creates a private fork with a reproducer and a patch.

## Early Disclosure

Entities interested in receiving an early disclosure must sign a nondisclosure agreement to receive early notification of security vulnerabilities.

The framework notifies entities in the early disclosure program within 72 hours, informing them of:

- The security advisory description.
- The code changes that will be added to the framework to patch it.

The [Micronaut core development team](https://github.com/orgs/micronaut-projects/teams/core-developers) will not make the patch publicly available during the embargo window.

During that period, partners can apply the code changes that mitigate the vulnerability directly to their own forks and use the time window to release patched versions of their forks and notify their consumers internally.

## After the Embargo Window

- The private GitHub forks with the patch will be merged.
- A patched version of the Micronaut components will be released.
- Security advisories will be made public in the GitHub UI.
- CVEs will be requested via the GitHub UI.
- A blog post will announce the security advisories.
