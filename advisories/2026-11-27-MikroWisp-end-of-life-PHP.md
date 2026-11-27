# MikroWisp — End-of-life PHP and Node.js with no security fixes (NOT CONFIRMED BY MIKROSYSTEM)

> **NOT CONFIRMED BY MIKROSYSTEM.** The versions below come from MikroWisp's public installer, not from a Mikrosystem advisory. Whether a given MikroWisp installation uses these versions, and whether its configuration exposes each flaw, has not been confirmed by Mikrosystem.

| Field | Details |
|---|---|
| **ID** | MITS-2026-0016 |
| **Product** | MikroWisp (Mikrosystem), through the PHP and Node.js versions installed by its public installer. |
| **Summary** | According to MikroWisp's public v6 installer, MikroWisp installs PHP 7.2 and Node.js 21. Both reached end of life and receive no security fixes from their projects. **Not confirmed by Mikrosystem.** |
| **Source** | MikroWisp public installer `https://mikrowisp.net/v6/install` (read 2026-11-27 17:31 UTC; SHA-256 `82d4066c74256db357198a5ec79d6fe28f654e31274137ad9255cef51aad9a13`). It installs the `php7.2` packages and configures the Node.js 21 (`setup_21.x`) repository. |
| **PHP 7.2** | Security support ended on 2020-11-30 ([php.net end-of-life branches](https://www.php.net/eol.php)). The installer configures the third-party Sury repository (packages.sury.org), which lists PHP 7.2 packages for current Debian and Ubuntu releases; whether those packages include fixes for these CVEs is not stated here — check your package changelog. The installer does not pin a package version. |
| **Node.js 21** | End of life since 2024-06-01 ([Node.js release schedule](https://github.com/nodejs/Release)). |
| **Related PHP CVEs** | [CVE-2026-115560](2026-11-27-CVE-2026-115560.md): related (CVE record has no lower bound; PHP advisory: older unsupported releases may also be affected). · [CVE-2026-109618](2026-11-27-CVE-2026-109618.md) and [CVE-2026-109619](2026-11-27-CVE-2026-109619.md): unknown: PHP 7.x was not evaluated by the PHP Group. |
| **Fixed versions** | None from the PHP project for PHP 7.2 or from the Node.js project for Node.js 21 (both end of life). Fixed PHP versions exist only in supported branches; see each linked advisory. |
| **Mikrosystem status** | Master IT Support contacted Mikrosystem about security issues in MikroWisp on 2026-10-27 (per Master IT Support). No Mikrosystem advisory or update about these versions is cited here. |
| **Recommended action** | Ask Mikrosystem for a MikroWisp release that runs on supported PHP and Node.js versions, and apply it when available. |
| **Published (UTC)** | 2026-11-27 |

ISPs that need personalized or more advanced support: contact Master IT Support — info@masteritsupport.com · +1 833-648-7877
