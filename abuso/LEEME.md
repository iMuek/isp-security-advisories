# Abuse list / Lista de abuso

**What this is.** One CSV file per UTC day with the IP addresses that attacked our network that day and that we reported to
[AbuseIPDB](https://www.abuseipdb.com), where the report was accepted (HTTP 200). It is the same information that is already public
on AbuseIPDB, grouped by day.

**Qué es.** Un archivo CSV por día UTC con las IP que atacaron nuestra red ese día y que denunciamos a AbuseIPDB, cuando la denuncia
fue aceptada (HTTP 200). Es la misma información que ya es pública en AbuseIPDB, agrupada por día.

## Columns / Columnas

| column | meaning |
|---|---|
| `ip` | the attacking IP address / la IP que atacó |
| `dia_utc` | day, UTC (`YYYY-MM-DD`) / día UTC |
| `tipo` | AbuseIPDB category numbers (`;`-separated) and a generic service in parentheses (`ssh`, `telnet`, `smtp`, `http`, `puertos` = port scan, `varios` = other; `+` when more than one) / categorías de AbuseIPDB y servicio genérico |
| `conteo` | how many accepted reports for that IP that day / cuántas denuncias aceptadas ese día |
| `enlace` | `https://www.abuseipdb.com/check/<ip>` |

Categories: <https://www.abuseipdb.com/categories>

## Where it comes from / De dónde sale

Our own sensors. We only report connections where the TCP handshake was completed; we never report bare SYN packets, UDP, or an
IP only because of its reputation score, following the [AbuseIPDB reporting policy](https://www.abuseipdb.com/reporting-policy).
Each file is written once, after the UTC day is closed.

Nuestros propios sensores. Solo denunciamos conexiones con el saludo TCP completo; nunca SYN sueltos, UDP ni una IP solo por su
reputación, según la política de AbuseIPDB. Cada archivo se escribe una vez, con el día UTC cerrado.

## What it does NOT contain / Qué NO trae

No usernames or passwords tried, no commands, no paths, no web headers, no e-mail domains, no IDS signature details, no exact ports
or times, and no information about our own systems or our customers. Our own and our customers' address ranges are filtered out
twice before a file is written; if any of them appears, the file is not produced.

Ni usuarios o claves probados, ni comandos, rutas, cabeceras web, dominios de correo, detalle de firmas IDS, puertos u horas exactas,
ni datos de nuestros equipos o clientes. Nuestros rangos y los de clientes se filtran dos veces; si aparece uno, el archivo no se genera.

## Use it with care / Úsela con cuidado

This list shows who attacked **us**. It is not a guarantee about any IP and may contain addresses that are shared, dynamic or
already cleaned. If you block with it, keep an allow-list of your own networks, use an expiry, and review before enabling.

Esta lista muestra quién **nos** atacó. No es una garantía sobre ninguna IP. Si bloquea con ella, mantenga una lista de sus propias
redes que nunca se bloquean, use vencimiento y revise antes de activar.

## Removal requests / Pedir que se quite una IP

Write to **info@masteritsupport.com** with the IP, the date(s) and why it should be removed (for example: the address was
reassigned or the host has been cleaned). We review each request; if accepted, the IP is removed from the affected files.

Escriba a **info@masteritsupport.com** con la IP, la(s) fecha(s) y el motivo. Revisamos cada pedido; si procede, se quita de los
archivos afectados.

---
Master IT Support · HRCOM
