# Abuse list

**What this is.** One CSV file per UTC day with the IP addresses that attacked our network that day and that we reported to
[AbuseIPDB](https://www.abuseipdb.com), where the report was accepted (HTTP 200). It is the same information that is already public
on AbuseIPDB, grouped by day.

## Columns

| column | meaning |
|---|---|
| `ip` | the attacking IP address |
| `date_utc` | day, UTC (`YYYY-MM-DD`) |
| `categories` | AbuseIPDB category numbers, `;`-separated |
| `service` | generic service: `ssh`, `telnet`, `smtp`, `http`, `portscan` or `other` (`+` when more than one) |
| `count` | how many accepted reports for that IP that day |
| `link` | `https://www.abuseipdb.com/check/<ip>` |

Categories: <https://www.abuseipdb.com/categories>

Files dated 2026-11-26 and later use the `categories` and `service` columns. Files dated 2026-11-25 and earlier use the earlier format, with a single `type` column (category numbers and the service in parentheses). Each file is written once; the only later change is removing an IP after an accepted removal request.

## Where it comes from

Our own sensors. We only report connections where the TCP handshake was completed; we never report bare SYN packets, UDP, or an
IP only because of its reputation score, following the [AbuseIPDB reporting policy](https://www.abuseipdb.com/reporting-policy).
Each file is written once, after the UTC day is closed.

## What it does NOT contain

No usernames or passwords tried, no commands, no paths, no web headers, no e-mail domains, no IDS signature details, no exact ports
or times, and no information about our own systems or our customers. Our own and our customers' address ranges are filtered out
twice before a file is written; if any of them appears, the file is not produced.

## Use it with care

This list shows who attacked **us**. It is not a guarantee about any IP and may contain addresses that are shared, dynamic or
already cleaned. If you block with it, keep an allow-list of your own networks, use an expiry, and review before enabling.

## Removal requests

Write to **info@masteritsupport.com** with the IP, the date(s) and why it should be removed (for example: the address was
reassigned or the host has been cleaned). We review each request; if accepted, the IP is removed from the affected files.

---
Master IT Support
