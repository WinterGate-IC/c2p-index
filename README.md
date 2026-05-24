# 🛡️ C2P-WATCH – Command & Control Provider Watchlist

**Tracking hosting providers that knowingly or unknowingly harbor nation-state APT command-and-control infrastructure.**

---

## 📋 Executive Summary

This repository documents hosting providers, CDNs, and infrastructure services that have been confirmed to host malicious command-and-control (C2) traffic for nation-state APT groups, ransomware affiliates, and other threat actors.

The intelligence is derived from public threat reports, independent security research, and open-source intelligence (OSINT) verification.

**Key Findings:**
- **9 active providers** confirmed hosting Iranian APT C2 infrastructure
- **1,357+ active C2 servers** identified across the Middle East
- **Cloudflare** actively abused by APT34 (OilRig) for C2 fronting
- **European providers** (OVH, WorldStream) turning blind eye to Iranian C2
- **Iranian domestic providers** operating openly under state protection

---

## 🎯 Confirmed C2 Providers (Active)

| Provider | Location | Malicious Activity | Source |
|----------|----------|---------------------|--------|
| **Noyan Abr Arvan** | Tehran, Iran | Cobalt Strike BEACON (ASN 202468) | Hunt.io Report |
| **Asiatech** | Tehran, Iran | Iranian APT IPs (ASN 43754) | Hunt.io Report |
| **Gostaresh Pardazesh** | Tehran, Iran | AdaptixC2 (ASN 51889) | Hunt.io Report |
| **AbrArvan CDN** | Iran | RondoDox botnet, 15k daily exploit attempts | Hunt.io Report |
| **WorldStream** | Netherlands | Iranian C2 infrastructure | Hunt.io Report |
| **OVH** | France/Global | Iranian Cobalt Strike C2 | Hunt.io Report |
| **Maral Host** | Isfahan, Iran | SmartLoader C2 | Anomali Report |
| **Shuttle** | Iran | Iranian domestic hosting | Hunt.io Report |
| **Cloudflare** | Global (fronting) | APT34 C2 obfuscation | Anomali Report |

---

## 📡 Full Threat Intelligence Reports

### Hunt.io Middle East Malicious Infrastructure Report (May 20, 2026)

The Hunt.io report identified **1,357 active C2 servers** across **98 infrastructure providers** in 14 Middle Eastern countries. Key findings:

- **96.8%** of observed malicious artifacts were C2 infrastructure
- IoT botnets (Hajime, Mozi, Mirai) combined with offensive frameworks (Cobalt Strike, Sliver)
- Iranian domestic ASNs actively hosting Cobalt Strike BEACON and AdaptixC2

**Specific Iranian ASNs Confirmed:**

| ASN | Provider | Malware |
|-----|----------|---------|
| ASN 202468 | Noyan Abr Arvan | Cobalt Strike BEACON |
| ASN 43754 | Asiatech | Iranian APT IPs |
| ASN 51889 | Gostaresh Pardazesh | AdaptixC2 |

**Source:** https://hunt.io/blog/middle-east-malicious-infrastructure-report

---

### Anomali: Iran's Cyber Arsenal Is Reloading (May 21, 2026)

The Anomali assessment confirmed that Iranian state cyber infrastructure is actively refreshing while offensive operations remain paused. Key findings:

- Iranian APT infrastructure confirmed on **OVH**, **WorldStream**, and **Maral Host**
- **SmartLoader C2** confirmed on Maral Host (213.176.73[.]163)
- **APT34 (OilRig)** actively using **Cloudflare fronting** to obscure C2 traffic
- Iran-Russia shared cyber infrastructure confirmed on ASN 213790

**Source:** https://www.anomali.com/blog/irans-cyber-arsenal-is-reloading

---

### Anomali: The Ceasefire Is a Lie (April 26, 2026)

This report documented Iranian cyber operations during the period immediately following the Cloudzy takedown. Key findings:

- Iranian offensive cyber ops **"conspicuously paused"**
- **Handala, Cyber Av3ngers, DieNet, 313 Team** operationally silent for 12+ days
- **43-day intelligence gap** in defense-industrial base monitoring – longest ever recorded
- Iranian APTs in **"coiled spring" posture** – infrastructure warm, operations cold

**Source:** https://www.anomali.com/blog/the-ceasefire-is-a-lie

---

### Hunt.io: Iranian Threat Actors Migrate to New Hosting Providers (May 14, 2026)

This report confirmed that following the Cloudzy disruption, Iranian APTs migrated to alternative hosting providers:

- **WorldStream** and **OVH** identified as new C2 providers
- Iranian Cobalt Strike infrastructure active on European VPS providers
- MuddyWater C2 server identified on Netherlands VPS containing C2 binaries, scripts, and operation logs

**Source:** https://hunt.io/blog/iranian-threat-actors-migrate

---

### Anomali: IRGC Names Western Tech Giants as Legitimate Targets (April 2, 2026)

This report documented Iran's official designation of Western technology companies as military targets, including:

- **Cloudflare** explicitly named as a target
- APT34's use of Cloudflare fronting for C2 obfuscation documented
- Iranian justification for attacking civilian infrastructure

**Source:** https://www.anomali.com/blog/irans-irgc-names-western-tech-giants-as-legitimate-targets

---

## 🔥 Iranian APT Groups Currently Active

| Group | Sponsor | Hosting Provider | Activity |
|-------|---------|------------------|----------|
| **APT34 (OilRig)** | MOIS | Cloudflare (fronting), OVH | Corporate espionage |
| **MuddyWater** | MOIS | Netherlands VPS, OVH | Multi-country espionage |
| **APT42** | IRGC-IO | OVH, WorldStream | Credential harvesting |
| **Charming Kitten** | IRGC-IO | Asiatech (Tehran) | Espionage campaigns |
| **Infy (Prince of Persia)** | State-backed | Telegram-based C2 | Espionage since 2004 |
| **APT33 (Elfin)** | IRGC | Unknown hosting | Aerospace, defense targeting |

---

## 🧬 The "Coiled Spring" Posture (May 2026)

The May 21, 2026, Anomali assessment describes Iranian cyber forces as a **"coiled spring"** :

> *"Iranian state cyber infrastructure is actively refreshing while offensive operations remain conspicuously paused. This is not de-escalation — it is reloading."*

**What this means:**
- The infrastructure is warm
- The C2 servers are active
- They are waiting for the order

**The 43-day intelligence gap** in defense-industrial base monitoring is the longest period without visibility into Iranian dormant access in defense contractor networks. That gap coincides directly with the Cloudzy freeze.

---

## 📊 Hosting Provider Risk Assessment

| Provider | Type | Risk Level | Notes |
|----------|------|------------|-------|
| **Cloudflare** | CDN | **CRITICAL** | Actively used for APT34 C2 fronting |
| **OVH** | Hosting | **HIGH** | Iranian Cobalt Strike C2 confirmed |
| **WorldStream** | Hosting | **HIGH** | Iranian C2 infrastructure confirmed |
| **Noyan Abr Arvan** | Iranian ISP | **CRITICAL** | Active Cobalt Strike BEACON |
| **Asiatech** | Iranian ISP | **HIGH** | Iranian APT IPs |
| **Gostaresh Pardazesh** | Iranian ISP | **HIGH** | AdaptixC2 |
| **Maral Host** | Hosting | **HIGH** | SmartLoader C2 |
| **AbrArvan CDN** | CDN | **CRITICAL** | RondoDox botnet, 15k daily exploits |

---

## 🔐 Defensive Recommendations

| Action | Priority |
|--------|----------|
| Block Iranian ASNs (202468, 43754, 51889, 213790) in firewall rules | HIGH |
| Monitor traffic to/from OVH and WorldStream IP ranges | HIGH |
| Replace Cloudflare with self-hosted alternative (Pangolin) | CRITICAL |
| Implement multi-CDN routing to avoid single-provider dependency | MEDIUM |
| Deploy identity-aware access control (Pangolin) | HIGH |

---

## 📁 Full Disclosure Resources

| Report | Link |
|--------|------|
| Hunt.io Middle East Malicious Infrastructure Report (May 20, 2026) | https://hunt.io/blog/middle-east-malicious-infrastructure-report |
| Anomali: Iran's Cyber Arsenal Is Reloading (May 21, 2026) | https://www.anomali.com/blog/irans-cyber-arsenal-is-reloading |
| Anomali: The Ceasefire Is a Lie (Apr 26, 2026) | https://www.anomali.com/blog/the-ceasefire-is-a-lie |
| Hunt.io: Iranian Threat Actors Migrate (May 14, 2026) | https://hunt.io/blog/iranian-threat-actors-migrate |
| Cyber Press: Telecom Networks Exploited (May 21, 2026) | https://cyberpress.org/telecom-networks-exploited/ |
| Anomali: IRGC Names Western Tech Giants as Targets (Apr 2, 2026) | https://www.anomali.com/blog/irans-irgc-names-western-tech-giants-as-legitimate-targets |

---

## ❅ Conclusion

Nine active hosting providers are currently confirmed to harbor Iranian APT command-and-control infrastructure. European providers (OVH, WorldStream) turn a blind eye. Iranian domestic providers (Noyan Abr Arvan, Asiatech, Gostaresh Pardazesh, Maral Host, Shuttle, AbrArvan CDN) operate openly under state protection.

Cloudflare is actively abused by APT34 for C2 fronting.

**The infrastructure is warm. The C2 servers are active. The 43-day intelligence gap is the longest ever recorded.**

They are reloading. Not resting.

**The Gatekeeper watches. The providers are documented. The criminals have nowhere left to hide.**

— WinterGate Intelligence Collective (WIC)
*Threat Intelligence. Infrastructure Defense. Community Empowerment.*
