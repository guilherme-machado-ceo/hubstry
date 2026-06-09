# Hubstry Deep Tech

**Quantum-Ready IoT Protocol for Industry 4.0 — with Post-Quantum Cryptography**

[![Site](https://img.shields.io/badge/site-hubstry.dev-00C9B8?style=flat-square)](https://guilherme-machado-ceo.github.io/hubstry)
[![Nautam Protocol](https://img.shields.io/badge/Nautam-IoT_Protocol-00C9B8?style=flat-square)](https://guilherme-machado-ceo.github.io/nautam-iot-protocol-site/)
[![DOI HPG 1.0](https://img.shields.io/badge/DOI-10.5281%2Fzenodo.19056387-blue?style=flat-square)](https://doi.org/10.5281/zenodo.19056387)
[![DOI Quantum Logistics](https://img.shields.io/badge/DOI-10.5281%2Fzenodo.20467804-blue?style=flat-square)](https://doi.org/10.5281/zenodo.20467804)
[![TRL](https://img.shields.io/badge/TRL-4_PoC_Validated-yellow?style=flat-square)](https://github.com/guilherme-machado-ceo/iot-protocol-hubstry)
[![ISO 42001](https://img.shields.io/badge/ISO%2FIEC_42001-Certified_2026%2F53%2FIPQ-green?style=flat-square)](https://orcid.org/0009-0008-1083-0784)
[![ORCID](https://img.shields.io/badge/ORCID-0009--0008--1083--0784-A6CE39?style=flat-square)](https://orcid.org/0009-0008-1083-0784)

> *An IoT communication protocol derived from the mathematics of musical harmony.  
> No interference. No negotiation overhead. 50–65% less energy than MQTT, CoAP, or DDS.  
> Post-quantum secure. Pure software. Any hardware.*

---

## What is Hubstry Deep Tech?

**Hubstry Deep Tech** is a Brazilian deep tech venture studio founded in 2023 in Rio de Janeiro, dedicated to developing proprietary technologies with a 30-year strategic horizon. Our model creates **technological moats** in emerging sectors before they become market standards.

**Founder:** Guilherme Gonçalves Machado — CEO/CTO/CPO  
**Co-Founder / CMO:** Rebeca Machado  
**Location:** Rio de Janeiro, Brazil → Seoul, Korea (planned relocation)  
**Website:** [hubstry.dev](https://guilherme-machado-ceo.github.io/hubstry)

---

## Core Product: Nautam IoT Protocol

### HALE + HPG Framework — Harmonic Addressing & Protocol Grid

The **Nautam IoT Protocol** is a 4-layer communication framework for connected devices built on the **rational harmonic series** — the same mathematical principle that governs how musical instruments produce sound without interference.

Instead of devices competing for bandwidth (conventional MQTT/CoAP/DDS), Nautam assigns each device a mathematically derived communication slot from a master frequency f₀. The result:

| Capability | Value |
|---|---|
| Energy reduction vs. MQTT/CoAP/DDS | **50–65%** |
| Interference | **Zero** (mathematically guaranteed orthogonality) |
| Synchronization overhead | **None** (native harmonic sync) |
| Hardware requirement | **None** (pure software implementation) |
| Unique addresses · O₁₆ | **160 bidimensional** |
| Post-quantum security | **Kyber768 / Dilithium3** (NIST PQC standards) |
| Coordination overhead | **~8–12%** vs MQTT ~40%, CoAP ~25%, DDS ~35% |
| TRL | **4** (PoC validated — Python/C++ codebase, dashboard, HSL Auth 500 cycles) |

### Protocol Architecture

| Layer | Name | Description | Mathematical Construct |
|---|---|---|---|
| **L1** | HPG Core | Master frequency, harmonic slot assignment, orthogonality engine | H_N = {a/b ∈ Q⁺ : gcd(a,b)=1, b≤N} |
| **L2** | HPG Signal | Composite signal generation, FFT decoding, spectral verification | s(t) = Σ Aₖ sin(2π(aₖ/bₖ)f₀t+φₖ) |
| **L3** | HALE | Device addressing, latency management, synchronization | O_N = H_N × {-1, +1} · \|O₁₆\| = 160 |
| **L4** | HPG-Sec | Timbral PUF authentication, spectral intrusion detection, LFSR key rotation | Kyber768 / Dilithium3 · NIST PQC |

### Protocol Family

| Variant | Focus | Status |
|---|---|---|
| **HPG-Core** | Base harmonic protocol | Active · TRL 4 |
| **HPG-D** | Pure digital / NCO implementation | Active · TRL 4 |
| **HPG-Sec** | Acoustic cryptography — timbral PUF authentication | Research |
| **HPG-R** | Intelligent robotics — harmonic hierarchy per subsystem | Research → Korea PoC target |
| **HMAL** | Marine Acoustic Layer — underwater communication, NATO C2/JANUS overlay, oceanographic monitoring | Published · DOI [10.5281/zenodo.20184616](https://doi.org/10.5281/zenodo.20184616) |
| **HPD-T** | Temperament-derived addressing (12-TET to 96-tone) | Research |

## Business Model — The ARM Analogy

Hubstry's long-term revenue model is royalty-per-device — structurally analogous to ARM Holdings. ARM does not manufacture chips; it owns the instruction set architecture and collects royalties from every device that implements it. ARM was acquired by SoftBank for USD 32 billion in 2016 on the strength of that licensing model alone. Nautam does not manufacture hardware: it owns the harmonic communication protocol and licenses it to device manufacturers, industrial integrators, and government infrastructure operators. Every IoT device that implements HPG generates a royalty. With 30 billion devices projected by 2030, the addressable licensing base is structural — not dependent on winning individual procurement contracts. The Korean market, as the world's most robot-dense industrial economy, is the optimal first deployment environment for this model.

---

## Validated Application: Quantum-Ready Logistics Platform

The [`hubstry-logistics-quantum`](https://github.com/Hubstry-DeepTech/hubstry-logistics-quantum) repository demonstrates the full Hubstry stack in a production-ready logistics optimization scenario:

- **IoT telemetry** via Nautam protocol
- **QUBO-VRP** (Quadratic Unconstrained Binary Optimization — Vehicle Routing Problem) via D-Wave Ocean SDK
- **PQC-secured** data transmission (Kyber768/Dilithium3)
- **Real GPS data**: Porto Taxi Trajectory Dataset (442 taxis, 30 delivery points)

### Benchmark vs. Google OR-Tools

| Solver | Time | Distance | CO₂ saved | Reduction | Gap vs OR-Tools |
|---|---|---|---|---|---|
| Hubstry Builtin SA | 7.73s | 46.61 km | 12.0 kg | 44.4% | +14.1% |
| **Hubstry D-Wave neal** | **1.03s** | **43.14 km** | **13.1 kg** | **48.6%** | **+5.6%** |
| Google OR-Tools GLS | 1.02s | 40.86 km | 13.8 kg | 51.3% | baseline |

> D-Wave neal closes **66% of the gap** vs. OR-Tools and is **7.5× faster** than Builtin SA.  
> The QUBO formulation runs on real D-Wave QPU hardware with **zero code changes**.

---

## Scientific Foundation — Peer-Reviewed Prior Art

All core Hubstry frameworks are published open access on Zenodo:

| Year | Publication | DOI | License |
|---|---|---|---|
| 2026 | Quantum-Ready Sustainable Logistics MVP (v0.3.0) | [10.5281/zenodo.20467804](https://doi.org/10.5281/zenodo.20467804) | CC BY-NC-SA 4.0 |
| 2026 | HMAL: Mapeamento Harmônico Racional de Vocalizações Cetáceas | [10.5281/zenodo.20184616](https://doi.org/10.5281/zenodo.20184616) | CC BY 4.0 |
| 2025 | Harmonic Protocol Grid (HPG 1.0) | [10.5281/zenodo.19056387](https://doi.org/10.5281/zenodo.19056387) | CC BY 4.0 |
| 2025 | HALE: Harmonic Addressing & Labeling Equation | [10.5281/zenodo.18901934](https://doi.org/10.5281/zenodo.18901934) | CC BY 4.0 |

**Author ORCID:** [0009-0008-1083-0784](https://orcid.org/0009-0008-1083-0784) · 15+ publications across IoT, quantum computing, semiotics, and linguistics.

---

## Institutional Partnerships & Certifications

| Partner / Institution | Program / Credential |
|---|---|
| **Microsoft** | Microsoft for Startups Founders Hub |
| **Google Cloud** | Google Cloud for Startups |
| **Amazon Web Services** | AWS Activate |
| **AIIA** | International Artificial Intelligence Industry Alliance — Member since July 2025 |
| **IPQ** | NP ISO/IEC 42001:2023 AI Management Systems — Certificate No. 2026/53/IPQ |
| **ABES** | Brazilian Association of Software Companies |
| **ABRIA** | Brazilian Association of Artificial Intelligence |

---

## Team

### Guilherme Gonçalves Machado — Founder & CEO/CTO
Deep tech architect and polymath founder. Developer of the HPG/HALE mathematical framework. Holds IPQ certification in NP ISO/IEC 42001:2023 AI management systems. AIIA member. Institutional partnerships with Microsoft, Google Cloud, and AWS. ORCID: [0009-0008-1083-0784](https://orcid.org/0009-0008-1083-0784).

**Core competencies:** IoT Protocol Design · Quantum Computing (QUBO/D-Wave) · Post-Quantum Cryptography · Python · C++ · Semiotic Systems · Deep Tech P&D

### Rebeca Machado — Co-Founder & CMO
Chief Marketing Officer of Hubstry Deep Tech and co-founder of [Laos UP](https://www.agencialaos.online/), a digital communications platform specializing in human-centered technology branding. Leads all marketing, brand strategy, and partner communications across the Hubstry ecosystem.

**Core competencies:** Brand Strategy · Digital Communications · Market Localization · Creative Direction · AI-integrated Marketing

---

## Korea Market Entry — K-Startup Grand Challenge 2026

Hubstry Deep Tech is applying to the **K-Startup Grand Challenge (KSGC) 2026**, promoted by the Ministry of SMEs and Startups of Korea (MSS).

**This is not a market exploration. Korea is our planned operational headquarters.**

### Target Sectors (KSGC Emerging Industry Classification)
- ③ **5G+** — IoT communication protocol (Nautam/HPG)
- ⑦ **Intelligent Robotics** — HPG-R variant for humanoid subsystem coordination
- ②⑥ **Quantum Technology** — QUBO-VRP logistics optimization
- ②⑦ **Cybersecurity** — PQC layer (Kyber768/Dilithium3)

### Target Korean Partners for PoC
- Samsung SDS — Industrial IoT integration
- KT IoT — Network infrastructure PoC
- Hyundai Glovis — Quantum logistics application
- POSCO — Smart manufacturing · HPG sensors
- Hyundai Robotics — HPG-R protocol variant
- KAIST / ETRI — Research partnership · PQC layer
- D-Wave Korea — QPU hardware integration (real quantum backend)

### Commitment to Settlement
- ✅ Full family relocation to Seoul prepared (CEO + CMO + family, valid passports)
- ✅ Korean legal entity (Yuhan Hoesa) planned for Phase 2
- ✅ Both founders as directors in Korean entity
- ✅ ISO/IEC 42001:2023 certified — directly relevant to Korean enterprise procurement
- ✅ Embassy of Brazil in Seoul (Itamaraty) — Embassy Recommendation Track

---

## Repository Structure

```
guilherme-machado-ceo/hubstry          ← This repo (hubstry.dev landing page)
guilherme-machado-ceo/iot-protocol-hubstry  ← Nautam IoT Protocol (HALE + HPG)
Hubstry-DeepTech/hubstry-logistics-quantum  ← Quantum-Ready Logistics Platform
guilherme-machado-ceo/hubstry-security      ← Cybersecurity platform (HSL + PQC)
guilherme-machado-ceo/hubstry-hale-ecosystem ← HALE mathematical framework
```

---

## Contact

**Email:** guilhermemachado@hubstry.onmicrosoft.com  
**LinkedIn:** [guilhermegoncalvesmachado](https://www.linkedin.com/in/guilhermegoncalvesmachado)  
**GitHub:** [guilherme-machado-ceo](https://github.com/guilherme-machado-ceo) · [Hubstry-DeepTech](https://github.com/Hubstry-DeepTech)  
**Nautam Site:** **Website:** [hubstry.dev](https://guilherme-machado-ceo.github.io/hubstry)


---

**Hubstry Deep Tech** · Rio de Janeiro, Brazil · Est. 2023  
*Founder & Owner: Guilherme Gonçalves Machado*  
© 2026 Hubstry Deep Tech — All rights reserved.
