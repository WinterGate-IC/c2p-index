## Priority Assessment (For Defensive Research)

Based on threat intelligence and active malicious infrastructure confirmation, the following providers are prioritized for defensive countermeasures:

**Tier 1 – Active C2 Infrastructure Confirmed:**

| Provider | Observed Activity |
|----------|--------------------|
| **Noyan Abr Arvan (ASN 202468)** | Cobalt Strike BEACON – active command channel |
| **Maral Host** | SmartLoader C2 – active malware distribution |
| **WorldStream** | Iranian C2 infrastructure – confirmed active |

**Tier 2 – CDN Fronting Abuse:**

| Provider | Observed Activity |
|----------|--------------------|
| **Cloudflare** | APT34 C2 traffic obfuscation – active abuse |

**Tier 3 – Iranian Domestic Infrastructure:**

| Provider | Observed Activity |
|----------|--------------------|
| Asiatech (ASN 43754) | Iranian APT IPs |
| Gostaresh Pardazesh (ASN 51889) | AdaptixC2 |
| AbrArvan CDN | RondoDox botnet, 15k daily exploit attempts |
| Shuttle | Iranian domestic hosting |

**Note:** This is a defensive research document. No attack methodologies are disclosed. All findings are derived from public threat intelligence reports and open-source verification.
