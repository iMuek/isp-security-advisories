# Vulnerability Advisories for ISPs — Master IT Support

Security information for Internet Service Providers (ISPs), in three parts:
- **Advisories:** concise notes on vulnerabilities affecting equipment and software used by ISPs: what the issue is, who is affected, how severe it is according to the official source, and what to do now.
- **Abuse list** ([abuse/](abuse/)): one CSV per UTC day with the external IP addresses that attacked our network and that we reported to AbuseIPDB.
- **MikroTik block list** ([mikrotik/](mikrotik/)): the same addresses as plain text, one IPv4 per line, with its SHA-256 checksum.

**Maintained by:** Master IT Support · **Updated:** whenever a new advisory is published, with a weekly summary.

## Latest
| Date (UTC) | ID | Product | Severity | Advisory |
|---|---|---|---|---|
| 2026-11-26 | CVE-2026-123007 | nginx | Critical (CVSS 4.0: 9.2) | [view](advisories/2026-11-26-CVE-2026-123007.md) |

[Full index by date and severity](INDEX.md) · [Weekly summaries](weekly/)

## How to use
- **Read:** open an advisory. Severity and "Recommended action" appear at the top.
- **Follow:** watch the repository, or check [INDEX.md](INDEX.md) and the [weekly summaries](weekly/).
- **Integrate:** use the data files below via their raw links.

## Formats
| File | Purpose | Raw link |
|---|---|---|
| `advisories/*.md` | Human-readable, one advisory per vulnerability | `https://raw.githubusercontent.com/iMuek/isp-security-advisories/main/advisories/<file>.md` |
| `index.csv` | Flat list: date, ID, product, CVSS, link | `https://raw.githubusercontent.com/iMuek/isp-security-advisories/main/index.csv` |
| `abuse/YYYY-MM-DD.csv` | Daily abuse list (see [abuse/README.md](abuse/README.md)) | `https://raw.githubusercontent.com/iMuek/isp-security-advisories/main/abuse/<YYYY-MM-DD>.csv` |
| `mikrotik/ipv4-list.txt` | Plain-text IPv4 block list + `.sha256` (see [mikrotik/README.md](mikrotik/README.md)) | `https://raw.githubusercontent.com/iMuek/isp-security-advisories/main/mikrotik/ipv4-list.txt` |

## Reading an advisory
- **Severity:** the CVSS score published by the source (NVD or the vendor). We do not assign our own scores.
- **Recommended action:** the vendor's general guidance. Detailed step-by-step remediation is not included here (see Support).
- **Sources:** every advisory links to the official notice. In case of any discrepancy, the official source prevails.

## Support
- **Error in an advisory** (data, link, version): open an Issue. **Do not include your IP addresses, device names, configurations or logs.**
- **Personalized or advanced support:** ISPs that need personalized or more advanced support: contact Master IT Support — info@masteritsupport.com · +1 833-648-7877
- **Reporting a new vulnerability:** do not use Issues. See [SECURITY.md](SECURITY.md).
- **Removal from the abuse list:** email info@masteritsupport.com with the IP, the date(s) and the reason.

## What this repository does not contain
Customer data, our own or our customers' IP addresses or network details, credentials, raw logs, or full remediation guides. The only IP addresses published are the external addresses in the abuse list and the MikroTik block list.
This information is general in nature and does not replace the vendor's advisory.

## License
This work is licensed under [CC BY 4.0](LICENSE) (Creative Commons Attribution 4.0 International).
