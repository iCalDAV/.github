# iCalDAV

[![Maven Central](https://img.shields.io/maven-central/v/org.onekash/icaldav-client)](https://central.sonatype.com/namespace/org.onekash)
[![Build](https://github.com/iCalDAV/iCalDAV/actions/workflows/ci.yml/badge.svg)](https://github.com/iCalDAV/iCalDAV/actions)
[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
[![Kotlin](https://img.shields.io/badge/kotlin-1.9+-purple.svg)](https://kotlinlang.org)

A Kotlin CalDAV client with offline sync and conflict resolution. Sync calendars with iCloud, Nextcloud, and other CalDAV servers.

## Features

- RFC 5545 compliant iCalendar parser and generator
- CalDAV client with automatic server discovery
- Recurring events (RRULE, EXDATE, RECURRENCE-ID)
- All-day and multi-day event support
- Timezone handling with VTIMEZONE
- Alarms (VALARM) with DISPLAY, EMAIL, and AUDIO actions
- Sync engine with offline support and conflict resolution
- Provider quirks handling (iCloud, Nextcloud, Radicale, Baikal)

## Modules

| Module | Purpose |
|--------|---------|
| `icaldav-core` | Parse and generate iCalendar (RFC 5545) |
| `icaldav-client` | CalDAV/WebDAV client with discovery and CRUD |
| `icaldav-sync` | Sync engine with offline support and conflict resolution |

## Tested Providers

| Provider | Notes |
|----------|-------|
| **iCloud** | CDATA responses, namespace quirks, regional redirects, app-specific passwords |
| **Nextcloud** | Standard CalDAV |
| **Radicale** | Direct URL access (skip discovery) |
| **Baikal** | sabre/dav based, standard CalDAV |

Other CalDAV servers following RFC 4791 should work. [Open an issue](https://github.com/iCalDAV/iCalDAV/issues) if you encounter problems.

## Links

- [Maven Central](https://central.sonatype.com/namespace/org.onekash)
- [GitHub](https://github.com/iCalDAV/iCalDAV)
- [Contributing](CONTRIBUTING.md)

## License

Apache License 2.0
