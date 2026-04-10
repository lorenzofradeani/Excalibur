<p align="center">
  <img src="https://img.shields.io/badge/Status-Closed%20Source-black?style=flat-square" alt="Closed Source">
  <img src="https://img.shields.io/badge/License-Proprietary-red?style=flat-square" alt="Proprietary">
  <img src="https://img.shields.io/badge/Access-KYB%2FKYC%20Required-orange?style=flat-square" alt="KYB/KYC">
</p>

# Excalibur

**AI Agentic Offensive Framework**

Closed-source penetration testing platform with full kill chain autonomy — from reconnaissance to forensic-grade reporting in a single, AI-orchestrated operation.

---

## What It Does

Excalibur conducts autonomous security assessments across the entire attack lifecycle. The operator defines the scope and rules of engagement; Excalibur handles reconnaissance, scanning, vulnerability analysis, exploitation, post-exploitation, and report generation — with mandatory human checkpoints at every critical decision.

## Capabilities

- **Autonomous Kill Chain** — AI-driven pipeline from target discovery to forensic report, with operator approval at every phase gate
- **Agentic Architecture** — Six specialized Docker agents (network enumeration, application security, wireless, chaos engineering, OSINT intelligence, orchestration) coordinated via encrypted MQTT
- **Plan Mode** — Mandatory planning phase generates a target-specific attack strategy with risk assessment, OPSEC considerations, and AI recommendations before any exploitation begins. Operator reviews and approves the plan
- **Adversarial Debate** — RED agent argues for exploitation, BLUE agent argues against, ARBITER makes the final call. Every exploit decision is challenged before execution
- **Exploit Modules** — Native implementations with real wire protocol interactions (not HTTP wrappers). Includes WAF bypass techniques for enterprise-hardened targets
- **Evasion Engine** — Multiple evasion techniques with high-performance native encoding backend
- **C2 Server** — Command and control with per-session key rotation, real-time multi-operator synchronization, role-based access control, and cryptographic audit trail
- **Tactical Dashboard** — Real-time operational HUD with session management, lock enforcement, and instant event notifications across operators
- **Forensic Evidence Chain** — Every action generates a SHA-256 linked, tamper-evident audit entry. Designed for legal and compliance requirements
- **CVE Intelligence** — Deterministic vulnerability matching against NVD, CISA KEV, and EPSS data. Automatic exploit chain generation prioritized by real-world exploitation probability
- **Cross-Platform** — Core framework operates on Linux, macOS, and Windows. Agents run in Docker containers

## Architecture

```
                    Operator
                       |
        +--------------+--------------+
        |              |              |
    CLI / TUI    Dashboard HUD    MQTT Agents
        |              |              |
        +--------------+--------------+
                       |
             Orchestration Layer
      Campaign Engine | Plan Mode | AI Planner
                       |
               Core Framework
   Exploit Registry | Evidence Chain | CVE Engine
   Grounded Reasoning | Multi-Model Consensus
                       |
            Execution Layer
    Native Exploits | Evasion Engine | C2 Server
```

## What Makes It Different

1. **AI decides, not just suggests.** The AI doesn't autocomplete commands — it reasons through multi-step attack chains, debates each decision, and adapts the plan based on intermediate results.

2. **Evidence-first design.** Every action is cryptographically chained. The audit trail is not an afterthought — it's the foundation. Built for engagements where legal admissibility matters.

3. **Plan before you strike.** No blind exploitation. The mandatory Plan Mode generates a detailed, target-specific strategy with OPSEC assessment before any exploit runs. The operator always has full visibility and control.

4. **Multi-operator coordination.** Multiple operators work on the same engagement simultaneously with real-time synchronization, session locking, and per-operator attribution in the audit trail.

## Access

Excalibur is not publicly available. Access is restricted to:

- Certified Managed Security Service Providers (MSSPs)
- Enterprise Red Team operations
- Government security agencies

**Process:** Application &rarr; KYB/KYC verification &rarr; Lawful use contract &rarr; Annual enterprise license

This is intentional. The capabilities in this framework — if released publicly — would be weaponized within hours. Controlled distribution is a security decision, not a marketing one.

## Not For

- Individual pentesters without organizational affiliation
- Bug bounty hunters (use purpose-built tools instead)
- Unauthorized security testing of any kind
- Academic or research use without explicit agreement

## Author

**Lorenzo Fradeani**
- [LinkedIn](https://www.linkedin.com/in/lorenzofradeani/)
- [Website](https://lorenzofradeani.com)

## Legal

Copyright &copy; 2025-2026 Lorenzo Fradeani. All rights reserved.

This software is proprietary and confidential. Unauthorized access, copying, distribution, modification, reverse engineering, or use of this software is strictly prohibited and may result in legal action. See [LICENSE](LICENSE) for full terms.
