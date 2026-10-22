# Discord reaction-system observation service

<!-- 561-group-standards:badges:start -->
[![Red Cup Engineering](https://img.shields.io/badge/561%20Group-Red%20Cup%20Engineering-c0392b)](https://github.com/red-cup-engineering)
[![License: MIT](https://img.shields.io/badge/license-MIT-c0392b)](LICENSE)
[![Indigenous data: CARE](https://img.shields.io/badge/Indigenous%20data-CARE-4b6f44)](https://github.com/red-cup-engineering/.github/blob/main/GOVERNANCE.md)
[![Tips welcome](https://img.shields.io/badge/tips-welcome-d4a017)](https://github.com/561-group/.github/blob/main/TIPS.md)
<!-- 561-group-standards:badges:end -->

This service observes a declared, bounded set of Discord configuration messages and their aggregate reactions. It makes only GET requests, never lists reaction users, never fetches channel histories, and publishes message content only from an explicitly configured administrator allowlist. Member-specific permission overwrites are redacted.

Callers provide all guild, selector, role, channel, integration, mapping, and output coordinates. The service contains no server-specific identifiers, credentials, policy copy, environment loading, or network writes.
