# Vulnerability Advisories for ISPs — Master IT Support

Concise advisories on security vulnerabilities affecting equipment and software used by Internet Service Providers (ISPs): what the issue is, who is affected, how severe it is according to the official source, and what to do now.

**Maintained by:** Master IT Support · **Updated:** whenever a new advisory is published, with a weekly summary.

## Latest
| Date (UTC) | ID | Product | Severity | Advisory |
|---|---|---|---|---|
| 2026-11-26 | CVE-2026-123007 | nginx / UISP (OpenResty) | Critical (CVSS 4.0: 9.2) | [view](advisories/2026-11-26-CVE-2026-123007.md) |

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

## Reading an advisory
- **Severity:** the CVSS score published by the source (NVD or the vendor). We do not assign our own scores.
- **Recommended action:** the vendor's general guidance. Detailed step-by-step remediation is not included here (see Support).
- **Sources:** every advisory links to the official notice. In case of any discrepancy, the official source prevails.

## Support
- **Error in an advisory** (data, link, version): open an Issue. **Do not include your IP addresses, device names, configurations or logs.**
- **Personalized or advanced support:** ISPs that need personalized or more advanced support: contact Master IT Support — info@masteritsupport.com · +1 833-648-7877
- **Reporting a new vulnerability:** do not use Issues. Email the address above.

## What this repository does not contain
Customer or internal network data, IP addresses, credentials, logs, or full remediation guides.
This information is general in nature and does not replace the vendor's advisory.

## License
This work is licensed under [CC BY 4.0](LICENSE) (Creative Commons Attribution 4.0 International).
