# UISP — Bundled OpenResty/nginx and the November 2026 nginx CVEs (NOT CONFIRMED BY UBIQUITI)

> **NOT CONFIRMED BY UBIQUITI.** UISP bundles OpenResty (an nginx distribution) for its web interface. Whether a given UISP release uses an affected OpenResty/nginx version, and whether its configuration exposes each flaw, has not been confirmed by Ubiquiti. This advisory has been reported to Ubiquiti and will be updated with their answer.

| Field | Details |
|---|---|
| **ID** | MITS-2026-0010 |
| **Product** | UISP (Ubiquiti), through its bundled OpenResty/nginx. |
| **Summary** | Six nginx CVEs published in November 2026 affect wide ranges of nginx versions. OpenResty is built on nginx, so an OpenResty release based on an affected nginx version is also in range. UISP may be affected if its bundled OpenResty is based on an affected nginx version; **not confirmed by Ubiquiti**. |
| **Related CVEs** | [CVE-2026-123007](2026-11-26-CVE-2026-123007.md) (HTTP/2), [CVE-2026-123633](2026-11-26-CVE-2026-123633.md) (HTTP/2), [CVE-2026-123634](2026-11-26-CVE-2026-123634.md) (resolver), [CVE-2026-121810](2026-11-26-CVE-2026-121810.md) (HTTP/3), [CVE-2026-113425](2026-11-26-CVE-2026-113425.md) (mail proxy): Critical, CVSS 4.0 9.2 (F5). [CVE-2026-132779](2026-11-26-CVE-2026-132779.md) (TLS 1.3 early data): Medium, CVSS 4.0 6.9 (F5). |
| **Affected nginx versions** | CVE-2026-123007: 1.9.5–1.31.8 · CVE-2026-123633: 1.19.7–1.31.8 · CVE-2026-123634: 0.6.18–1.31.8 · CVE-2026-121810: 1.25.0–1.31.8 · CVE-2026-113425: 0.5.33–1.31.8 · CVE-2026-132779: 1.21.4–1.31.9. Source: [nginx.org security advisories](https://nginx.org/en/security_advisories.html). |
| **Fixed versions** | **OpenResty 1.31.9.1** (2026-11-23) upgrades its nginx core from 1.31.8 to 1.31.9 and lists fixes for CVE-2026-123007, -123633, -123634, -121810 and -113425 (source: [OpenResty 1.31.9.x changelog](https://openresty.org/en/changelog-1031009.html)). nginx: 1.30.7 and 1.31.9 fix those five (source: nginx.org). |
| **Not yet fixed in OpenResty** | **CVE-2026-132779** is fixed in nginx 1.30.8 and 1.31.10 (source: nginx.org). No OpenResty release with this fix was found: the latest release on the [OpenResty download page](https://openresty.org/en/download.html) is 1.31.9.1, and its changelog does not mention CVE-2026-132779 (checked 2026-11-27). |
| **Ubiquiti status** | No UISP update or advisory from Ubiquiti about these CVEs is cited here. Check Ubiquiti's UISP release notes for updates. |
| **Recommended action** | Apply Ubiquiti's UISP update as soon as one that addresses these CVEs is released. |
| **Note (Master IT Support)** | General hardening, not a vendor recommendation: (1) limit access to the UISP web interface to trusted management networks; (2) disable HTTP/2 where it is not needed (see [CVE-2026-123007](2026-11-26-CVE-2026-123007.md) for the nginx directives). UISP manages its own nginx configuration: a manual change may be overwritten by a UISP update and is not supported by Ubiquiti, so check with Ubiquiti before changing it. |
| **Published (UTC)** | 2026-11-27 |

ISPs that need personalized or more advanced support: contact Master IT Support — info@masteritsupport.com · +1 833-648-7877
