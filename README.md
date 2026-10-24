# Framework Primer and Risk Assessment

A beginner GRC (Governance, Risk, and Compliance) project in two parts. First, I compared three major security frameworks: NIST CSF 2.0, ISO 27001, and SOC 2. Then I applied them by running a small risk assessment on a fictional company and mapping the controls to all three.

## Why I made this

I'm a student studying criminology with a business administration minor and I'm building skills for an entry-level GRC role. Reading about frameworks only got me so far, so I wanted to use them on a realistic scenario to see how risks, controls, and frameworks connect in practice.

## The scenario

Example Co. is a fictional 40-person payments company in Toronto. It moves money for small businesses, so it holds customer data and depends on its platform and a third-party payment processor. The company is invented, and no real organization's information was used.

## What's inside

| File | Contents |
|---|---|
| `01-framework-comparison.md` | Side-by-side comparison of NIST CSF 2.0, ISO 27001, and SOC 2, plus which one Example Co. would likely choose and why |
| `02-risk-assessment.md` | Company profile, scoring method, and a risk register of 9 risks with likelihood, impact, and planned treatments |
| `03-control-mapping.md` | Each planned control mapped to NIST CSF 2.0, ISO 27001 Annex A, and SOC 2 criteria |

## How I did it

1. **Compared the frameworks** using their public documentation.
2. **Described the company and its key assets** (customer data, payment platform, laptops, cloud storage, payment processor).
3. **Identified 9 risks** and scored each one using likelihood x impact on a 5-point scale.
4. **Chose a treatment** for each risk and noted which existing policies already helped.
5. **Mapped each control** to the three frameworks.

## What I learned

- SOC 2 is an audit report and NIST CSF is not certifiable
- Risk scoring and how subjective likelihood and impact are
- All three frameworks asking for managing risk, information security protection, and establishing disciplined internal controls


## Limitations

- This is a learning project on a fictional company, not a real assessment.
- Risk scores are my own judgment as a beginner. In a real assessment they would be agreed with the business and based on incident data.
- The ISO 27001 standard is paywalled, so I used public summaries of its structure and Annex A control names. 
- Framework mappings involve judgment, and a different reviewer might choose differently. I checked the control IDs against.

## Next steps

- Link this to my [policy-to-control mapping project](https://github.com/ervanleodiola1-grc/grc-policy-control-mapping), which uses the same fictional company
- Load the risk register into SQL and build a simple dashboard to summarize risks by rating and framework function

## References

- [NIST Cybersecurity Framework 2.0](https://www.nist.gov/cyberframework)
- [AICPA Trust Services Criteria](https://www.aicpa-cima.com)
- [ISO/IEC 27001 overview](https://www.iso.org/standard/27001)
