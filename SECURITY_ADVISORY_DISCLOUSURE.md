# Micronaut Security Disclosure Policy

The goal of this policy is to responsible disclose security vulnerabilities to minimize exposure windows.

This policy describes the steps to follow if a security advisory is reported in the Micronaut code. Every active and not archived repository that publishes components to Maven Central or is hosted publicly on Github is in scope.

The embargo window is 45 days.

## Intake

Security Advisories to any of the framework components are reported via the [GitHub Security Advisory UI](https://docs.github.com/en/code-security/how-tos/report-and-fix-vulnerabilities/fix-reported-vulnerabilities/creating-a-repository-security-advisory#creating-a-security-advisory). Publicly known security problems including CVEs do not fall under the embargo (as they are public already) and they will be patched immediately.

## Triage 

- The Micronaut core development team reviews the security advisory. 

- The Micronaut core development team attempts to reproduce the issue, and they verify that it is indeed a valid security advisory. 

- Advisories with [CVSS 3.1](https://www.first.org/cvss/calculator/3.1) score > 4.0 (Medium and above), enter the embargo period. 

- The core development team will acknowledge receipt of the advisory within 5 business days. After triaging the issue, the core development team will notify the reporter of the outcome and tell them: 
- That the reporter will be credited via the GitHub UI
- Ask the reporter to please respect the embargo window and avoid talking about the security advisory publicly before the public patch date which will be 45 days after the reporting (the end of the embargo window).
- The Micronaut core development team creates a private fork with a reproducer and a patch.  

## Early disclosure
Entities interested on receiving an early disclousure must sign a non disclosure agreement to receive early notification of security vulnerabilities. 

The framework notifies entities in the early disclosure programm within 72 hours, telling them: 
- Security advisory description
- Code changes that will be added to the framework to patch it. 

The Micronaut Core development team will not make the patch publicly available during the embargo window.

During that period, partners can apply the code changes that mitigate the vulnerability directly to their own forks and use the time window to release a patched version of their forks and notify their consumers internally. 

## After the embargo window
- The GitHub private forks with the patch will be merged
- A patched version of Micronaut components will be released
- Security advisories will be made public in the GitHub UI
- Security CVEs will be requested via the GitHub UI
- Blog post will announce the security advisories. 