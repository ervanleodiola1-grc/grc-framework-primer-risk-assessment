# Framework Comparison: NIST CSF 2.0, ISO 27001, and SOC 2

*A beginner's comparison written from public sources. Not legal or audit advice.*

| | NIST CSF 2.0 | ISO/IEC 27001 | SOC 2 |
|---|---|---|---|
| **Published by** | NIST (U.S. government) | ISO/IEC (international standards bodies) | AICPA (accounting body) |
| **What it is** | A voluntary framework of security outcomes | A standard for running an Information Security Management System (ISMS) | An audit report on a company's controls |
| **Certifiable?** | No | Yes, by an accredited certification body | No certificate. A CPA firm issues an attestation report |
| **Structure** | 6 Functions: Govern, Identify, Protect, Detect, Respond, Recover, split into Categories and Subcategories | Management clauses (4-10) plus Annex A controls (93 in the 2022 version, in 4 themes) | 5 Trust Services Criteria: Security, Availability, Processing Integrity, Confidentiality, Privacy |
| **Cost to read** | Free | Full standard is paid | Criteria are free from the AICPA |
| **Typically used by** | Organizations of any size, often as a starting point | Companies that need an internationally recognized certificate | Service providers (SaaS, fintech) proving security to customers |
| **Question it answers** | "What outcomes should our security program achieve?" | "Do we manage security systematically, and can we prove it?" | "Can an auditor confirm our controls work?" |

## Key differences in plain English

- **NIST CSF** is a guide. It tells you what to aim for but nobody certifies you against it.
- **ISO 27001** is a management system. It cares about the process (risk assessment, policies, reviews, improvement) as well as the controls.
- **SOC 2** is an audit. A Type I report checks whether controls are designed properly at one point in time. A Type II report checks whether they worked over a period, usually 3 to 12 months.

## How they relate

They overlap heavily. For example, strong authentication appears in all three. Companies often implement controls once and map them to several frameworks, which is what I do in `03-control-mapping.md`.

## Which would Example Co. pick?

[Your answer in 3-4 sentences. Hint: a small payments company selling to banks and businesses would probably be asked for a SOC 2 report by customers, and might choose NIST CSF as an internal guide first. Explain your reasoning in your own words.]

## Sources

- NIST Cybersecurity Framework 2.0: nist.gov/cyberframework
- AICPA Trust Services Criteria: aicpa-cima.com
- ISO/IEC 27001 overview: iso.org (the full standard is paywalled, so I used public summaries of its structure)
