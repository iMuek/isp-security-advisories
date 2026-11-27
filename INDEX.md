# Advisory Index

ID: our own stable identifier (`MITS-YYYY-NNNN`, never reused). CVE: the official CVE identifier.

Dates shown are the official CVE publication dates (CVE record). index.csv also keeps our advisory date (date_utc).

File naming: `advisories/YYYY-MM-DD-<CVE>.md` (advisory date, UTC). An advisory about a product affected by several CVEs uses `advisories/YYYY-MM-DD-<Product>-<topic>.md`.

## By CVE publication date (newest first)
| CVE published | ID | CVE | Product | Severity (CVSS, source) | Advisory |
|---|---|---|---|---|---|
| 2026-11-23 | MITS-2026-0006 | CVE-2026-132779 | nginx | 4.0: 6.9 · 3.1: 5.3 (F5) | [view](advisories/2026-11-26-CVE-2026-132779.md) |
| 2026-11-19 | MITS-2026-0009 | CVE-2026-115560 | PHP | 4.0: 9.2 (PHP Group) | [view](advisories/2026-11-27-CVE-2026-115560.md) |
| 2026-11-18 | MITS-2026-0001 | CVE-2026-123007 | nginx | 4.0: 9.2 · 3.1: 8.1 (F5) | [view](advisories/2026-11-26-CVE-2026-123007.md) |
| 2026-11-18 | MITS-2026-0002 | CVE-2026-123633 | nginx | 4.0: 9.2 · 3.1: 8.1 (F5) | [view](advisories/2026-11-26-CVE-2026-123633.md) |
| 2026-11-18 | MITS-2026-0003 | CVE-2026-123634 | nginx | 4.0: 9.2 · 3.1: 8.1 (F5) | [view](advisories/2026-11-26-CVE-2026-123634.md) |
| 2026-11-18 | MITS-2026-0004 | CVE-2026-121810 | nginx | 4.0: 9.2 · 3.1: 8.1 (F5) | [view](advisories/2026-11-26-CVE-2026-121810.md) |
| 2026-11-18 | MITS-2026-0005 | CVE-2026-113425 | nginx | 4.0: 9.2 · 3.1: 8.1 (F5) | [view](advisories/2026-11-26-CVE-2026-113425.md) |
| 2026-11-18 | MITS-2026-0011 | CVE-2026-118899 | nginx | 4.0: 8.7 · 3.1: 7.5 (F5) | [view](advisories/2026-11-27-CVE-2026-118899.md) |
| 2026-11-18 | MITS-2026-0012 | CVE-2026-125283 | nginx | 4.0: 6.9 · 3.1: 5.3 (F5) | [view](advisories/2026-11-27-CVE-2026-125283.md) |
| 2026-11-18 | MITS-2026-0013 | CVE-2026-120967 | nginx | 4.0: 6.3 · 3.1: 4.8 (F5) | [view](advisories/2026-11-27-CVE-2026-120967.md) |
| 2026-11-18 | MITS-2026-0014 | CVE-2026-123640 | nginx | 4.0: 6.9 · 3.1: 5.3 (F5) | [view](advisories/2026-11-27-CVE-2026-123640.md) |
| 2026-11-18 | MITS-2026-0015 | CVE-2026-120993 | nginx | 4.0: 6.9 · 3.1: 5.3 (F5) | [view](advisories/2026-11-27-CVE-2026-120993.md) |
| 2026-10-21 | MITS-2026-0007 | CVE-2026-109618 | PHP | 4.0: 9.2 · 3.1: 9.8 (PHP Group / NVD) | [view](advisories/2026-11-27-CVE-2026-109618.md) |
| 2026-10-21 | MITS-2026-0008 | CVE-2026-109619 | PHP | 4.0: 9.2 · 3.1: 8.1 (PHP Group / NVD) | [view](advisories/2026-11-27-CVE-2026-109619.md) |
| — | MITS-2026-0010 | Several (see advisory) | UISP (bundled nginx/OpenResty) | Not rated: not confirmed by Ubiquiti | [view](advisories/2026-11-27-UISP-bundled-OpenResty.md) |

## By severity
Rating is based on the most recent CVSS version published by the source (currently 4.0). If only 3.1 is available, 3.1 is used.
### Critical (9.0–10.0)
- MITS-2026-0007 [CVE-2026-109618](advisories/2026-11-27-CVE-2026-109618.md): PHP (4.0: 9.2)
- MITS-2026-0008 [CVE-2026-109619](advisories/2026-11-27-CVE-2026-109619.md): PHP (4.0: 9.2)
- MITS-2026-0009 [CVE-2026-115560](advisories/2026-11-27-CVE-2026-115560.md): PHP (4.0: 9.2)
- MITS-2026-0002 [CVE-2026-123633](advisories/2026-11-26-CVE-2026-123633.md): nginx, HTTP/2 use-after-free (4.0: 9.2)
- MITS-2026-0003 [CVE-2026-123634](advisories/2026-11-26-CVE-2026-123634.md): nginx, proxy/resolver use-after-free (4.0: 9.2)
- MITS-2026-0004 [CVE-2026-121810](advisories/2026-11-26-CVE-2026-121810.md): nginx, HTTP/3 use-after-free (4.0: 9.2)
- MITS-2026-0005 [CVE-2026-113425](advisories/2026-11-26-CVE-2026-113425.md): nginx, mail proxy use-after-free (4.0: 9.2)
- MITS-2026-0001 [CVE-2026-123007](advisories/2026-11-26-CVE-2026-123007.md): nginx (4.0: 9.2)
### High (7.0–8.9)
- MITS-2026-0011 [CVE-2026-118899](advisories/2026-11-27-CVE-2026-118899.md): nginx, TLS 1.3 request body infinite loop (4.0: 8.7)
### Medium (4.0–6.9)
- MITS-2026-0012 [CVE-2026-125283](advisories/2026-11-27-CVE-2026-125283.md): nginx, alias with try_files buffer overflow (4.0: 6.9)
- MITS-2026-0013 [CVE-2026-120967](advisories/2026-11-27-CVE-2026-120967.md): nginx, stream client-certificate bypass (4.0: 6.3)
- MITS-2026-0014 [CVE-2026-123640](advisories/2026-11-27-CVE-2026-123640.md): nginx, stream ssl_preread validation (4.0: 6.9)
- MITS-2026-0015 [CVE-2026-120993](advisories/2026-11-27-CVE-2026-120993.md): nginx, PROXY protocol v2 NULL dereference (4.0: 6.9)
- MITS-2026-0006 [CVE-2026-132779](advisories/2026-11-26-CVE-2026-132779.md): nginx, TLS 1.3 early data CPU exhaustion (4.0: 6.9)
### Low (0.1–3.9)
- (none)
### Not rated (product advisories not confirmed by the vendor)
- MITS-2026-0010 [UISP bundled nginx/OpenResty](advisories/2026-11-27-UISP-bundled-OpenResty.md): UISP, related to the November 2026 nginx CVEs; not confirmed by Ubiquiti

Rating bands follow FIRST's CVSS qualitative severity scale. Scores are those of the source; we only map them to a band.
