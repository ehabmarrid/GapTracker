# Security Policy

GapTracker is a closed-source iOS application. This public repository contains product documentation, research materials, and screenshots. It does not distribute the application source code.

## Data Architecture

GapTracker does not operate a user-account server, application backend, or central database.

- App data is stored locally on the user's device.
- iCloud synchronization is optional and provided through the user's Apple account.
- Moodle and Canvas communication occurs directly between the user's device and institution.
- Moodle authentication tokens are stored in the iOS Keychain.
- Imported learning-platform information remains on the device.
- AI-assisted syllabus processing occurs only when initiated by the user.

## Supported Versions

Only the latest App Store version is considered for security fixes.

| Version | Supported          |
| ------- | ------------------ |
| 2.2     | :white_check_mark: |
| < 2.2   | :x:                |

Users should update to the latest App Store version before reporting an issue.

## Reporting a Vulnerability

Do not publish suspected vulnerabilities through GitHub issues, discussions, App Store reviews, or social media.

Use GitHub's private vulnerability-reporting feature:

**Security → Advisories → Report a vulnerability**

If private reporting is unavailable, contact the repository owner through their GitHub profile to request a private communication channel. Do not include vulnerability details in a public message.

Include:

- The affected GapTracker version
- Device model and iOS version
- A description of the issue and its potential impact
- Clear reproduction steps
- Relevant screenshots with personal and institutional information removed

## In Scope

Reports should concern a reproducible security or privacy issue caused by GapTracker, including:

- Unauthorized exposure of locally stored or iCloud-synchronized app data
- Moodle or Canvas authentication, import, matching, or synchronization vulnerabilities
- Privacy issues involving AI-assisted syllabus processing

## Responsible Disclosure

Test only with devices, accounts, institutions, and data that you own or are authorized to use.

A vulnerability report does not authorize access to another person's data, testing against institutional systems without permission, service disruption, or destructive activity.

Stop testing and report the issue if you encounter information that you are not authorized to access.

Do not publicly disclose a vulnerability before it has been reviewed.

## Third-Party Services

GapTracker integrates with services operated by other organizations, including Apple, iCloud, Moodle and Canvas institutions, identity providers, and external AI-processing services.

GapTracker can investigate issues caused by how the application interacts with these services. It cannot control or correct vulnerabilities, outages, access restrictions, configuration problems, policy changes, or data-handling practices originating solely within a third-party service.

Issues affecting a third-party service independently of GapTracker should be reported directly to that service or institution.

## Out of Scope

The following are generally outside the scope of this policy:

- Vulnerabilities originating solely in Apple, iCloud, Moodle, Canvas, an educational institution, an identity provider, or an AI service
- Compromised Apple, Moodle, Canvas, or institutional accounts
- Issues requiring physical access to an already unlocked device
- Issues affecting unsupported GapTracker versions
- Modified, jailbroken, or unsupported operating systems
- Social-engineering attacks
- Denial-of-service or destructive testing
- Reports without a reproducible impact caused by GapTracker

## Response Process

Reports are reviewed on a best-effort basis.

If an issue is reproducible and caused by GapTracker, it will be assessed for a future application update. Response and resolution times depend on severity, reproducibility, App Store review requirements, and any involvement from external services or institutions.

Reports that concern unsupported versions, cannot be reproduced, fall outside GapTracker's control, or originate solely in a third-party service may be closed or redirected to the appropriate provider.

No bug-bounty or monetary-reward program is currently offered.

## Policy Limitations

This policy describes a vulnerability-reporting process. It does not create a warranty, guarantee, contractual obligation, guaranteed response time, or commitment to resolve every submitted report.
