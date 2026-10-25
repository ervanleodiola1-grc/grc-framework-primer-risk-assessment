# Control Mapping

Each treatment from the risk register is mapped to NIST CSF 2.0, ISO 27001:2022 Annex A, and SOC 2 Trust Services Criteria.

| Risk | Control (plain English) | NIST CSF 2.0 | ISO 27001:2022 Annex A | SOC 2 | Verified |
|---|---|---|---|---|---|
| R1 | MFA and strong authentication for customers | PR.AA-03 | 8.5 Secure authentication | CC6.1 | ☐ |
| R2 | Phishing awareness training | PR.AT-01 | 6.3 Awareness and training | CC2.2 | ☐ |
| R3 | Remove and review access rights | PR.AA-05 | 5.18 Access rights | CC6.2 | ☐ |
| R4 | Review third-party risk | GV.SC-07 | 5.19 Supplier relationships | CC9.2 | ☐ |
| R5 | Endpoint protection against malware | PR.PS-05 | 8.7 Protection against malware | CC6.8 | ☐ |
| R6 | Scan for vulnerabilities | PR.PS-02 | 8.8 Technical vulnerabilities | CC7.1 | ☐ |
| R7 | Secure cloud configuration and encryption | PR.DS-01 | 5.23 Cloud services | CC6.1 | ☐ |
| R8 | Back up and test restores | PR.DS-11 | 8.13 Information backup | A1.2 | ☐ |
| R9 | Log and monitor access to customer data | DE.CM-03 | 8.15 Logging | CC7.2 | ☐ |

## What I noticed

All three frameworks directly substantially overlap on core security requirements, such as R2 where NIST CSF (PR.AT-01), ISO 27001 (6.3), and SOC 2 (CC2.2) all require phishing awareness training. On the other hand, R7 shows where frameworks differ in detail: ISO 27001 features a dedicated clause specifically for cloud services (Annex A 5.23), whereas NIST CSF and SOC 2 address this requirement through broader data security and access controls like PR.DS-01 and CC6.1. This shows that while fundamental security goals are shared across frameworks, the way specific technical areas—like cloud security—are categorized varies.
