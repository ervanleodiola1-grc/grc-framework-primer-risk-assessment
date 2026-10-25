# Risk Assessment: Example Co. (fictional)

## 1. Company profile

Example Co. is a fictional 40-person company in Toronto that offers online payment transfers to small businesses. Its main customers are business clients and banks that need a reliable platform to process customer account data, like names, email addresses, and bank details. The company operates on a hybrid model, where employees use laptops and company email to collaborate both remotely and from the office. PaySwift relies on cloud storage and databases to store sensitive client data, alongside a third-party payment processor to complete real-time financial transactions.

**Key assets**

| Asset | Why it matters |
|---|---|
| Customer account data (names, emails, bank details) | Privacy obligations and fraud risk |
| Payment platform (web app and API) | Revenue depends on it being available |
| Employee laptops and email | Main entry point for attackers |
| Cloud storage and databases | Holds customer data |
| Third-party payment processor | Moves the actual money |

## 2. Method

I used a simple likelihood x impact approach. It is inspired by NIST SP 800-30 and ISO 27005 but heavily simplified.

- **Likelihood (1-5):** 1 = rare, 3 = possible, 5 = almost certain within a year
- **Impact (1-5):** 1 = minor, 3 = moderate (some customers affected), 5 = severe (major outage, large data loss, regulatory action)
- **Score:** Likelihood x Impact
- **Rating:** 1-6 Low, 7-12 Medium, 13-19 High, 20-25 Critical

Scores are my own judgment as a beginner. In a real assessment they would be agreed with the business using incident history and data.

## 3. Risk register

| ID | Risk | Asset | L | I | Score | Rating | Existing control (from my policies) | Planned treatment |
|---|---|---|---|---|---|---|---|---|
| R1 | Criminals take over customer accounts using stolen passwords | Customer accounts | 4 | 4 | 16 | High | Password Policy 3.4, 4.1 (for staff only) | Add MFA and login anomaly alerts for customers |
| R2 | Phishing email tricks an employee into giving up credentials | Employee email | 4 | 4 | 16 | High | Password Policy 4.1 (MFA) | Annual plus new-hire phishing training and simulations |
| R3 | Former employees or role-changers keep access they should not have | All systems | 3 | 4 | 12 | Medium | Access Control Policy 6.1, 7.1, 7.2 | Track removals in a checklist and audit quarterly |
| R4 | Payment processor suffers an outage or breach | Payment processor | 3 | 5 | 15 | High | None | Vendor risk review and a backup processor plan |
| R5 | Ransomware encrypts laptops or shared files | Laptops, file storage | 3 | 5 | 15 | High | Incident Response Policy 7.1, 7.4 | Endpoint protection plus offline backups |
| R6 | Undetected application or system vulnerabilities are exploited due to lack of scanning. | Payment platform | 3 | 4 | 12 | Medium | None | Monthly vulnerability scans and a patch schedule |
| R7 | Misconfigured cloud storage exposes customer data | Cloud storage | 2 | 5 | 10 | Medium | None | Configuration reviews and encryption |
| R8 | Backups fail when needed, causing a long outage | Databases | 2 | 4 | 8 | Medium | Incident Response Policy 7.4 | Test restores twice a year |
| R9 | Employee misuses customer data | Customer data | 2 | 4 | 8 | Medium | Access Control Policy 5.3 (admin logging) | Log and review access to customer records |

## 4. Findings

The highest risks in the assessment are R1, R2, R4, and R5, as they all carry "High" risk ratings with scores of 15 or 16. Currently, there are no existing controls in place for risks R4, R6, and R7. Out of these unmitigated risks, R4 (payment processor outage or breach) requires immediate attention because it carries a High risk rating. To address this highest-priority gap first, the company should conduct a vendor risk review and establish a backup payment processor plan. Following that, implementing controls for R6 and R7 will fix the remaining gaps where security coverage is currently missing.

## 5. Limitations

This is a learning exercise on a fictional company. Scores are subjective, the company is small and simple, and no real systems were tested.
