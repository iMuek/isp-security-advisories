# MikroTik block list

`ipv4-list.txt` is **plain text**: one IPv4 address per line, nothing else. It is built from the accepted reports in
[`../abuse/`](../abuse/) (see that README for where the data comes from and what it does NOT contain).
`ipv4-list.txt.sha256` is its SHA-256 checksum, published with every version.

**We do not publish a `.rsc` file to `/import`.** A `.rsc` is code that your router runs with full rights. Whatever you use to
load it should only read the text and only add valid IPv4 addresses, ignoring any other line. An example script for RouterOS
will be published here after we finish testing it in a lab.

## Warnings

- **Test first** on a lab router; enable any blocking rule with Safe Mode.
- **List poisoning.** If this repository were ever altered, the list could contain wrong addresses (for example your upstream or your
  customers). That is why you should keep an allow-list of your own networks evaluated before the block, give entries a short expiry
  (for example 2 days), start with the blocking rules disabled, and review before enabling. Watch how many IPs come in each day and distrust a sudden jump.
- This list shows who attacked **us**; it guarantees nothing about any IP.

Removal requests: **info@masteritsupport.com**

---
Master IT Support · HRCOM
