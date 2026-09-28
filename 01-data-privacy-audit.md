# Practical 1: Data Privacy Audit of Instagram

## Aim
Review Instagram's publicly described data practices, identify privacy risks, and recommend controls. This is a desk-based student audit, not an internal audit or legal finding.

## Organization and scope
Instagram is a social networking service operated by Meta. This review considers account/profile data, content and messages, activity, device information, personalization/advertising, third-party access, and user controls. Policy wording and settings vary by region and may change; check the version available at submission.

## Audit method
Read the Meta Privacy Policy and Privacy Center. Separate statements in those sources from risks inferred by the student. Rate likelihood and impact qualitatively as Low, Medium, or High.

## Audit observations
| Area | Public-document observation | Risk / recommendation |
|---|---|---|
| Collection | Meta describes information users provide, activity on its products, device/browser information, and information from partners or other sources [1]. | Broad signals may reveal habits and interests. Explain purposes clearly and collect only what each feature needs. |
| Public content | Users can manage audience and privacy settings [2]. | Posts, tags, comments, and location clues can expose personal details. Make audience defaults visible before posting. |
| Personalization | Meta explains information uses for product personalization and advertising [1][2]. | Users may not understand how activity or partner information affects recommendations and ads. Offer clear explanations and usable controls. |
| Sharing | The policy describes sharing within Meta and with service providers or other parties in specified cases [1]. | Third-party access increases governance and transfer complexity. Limit fields, purposes, retention, and access. |
| User control | Accounts Center includes information access and download tools [3]. | Controls may be hard to find or downstream retention unclear. Explain access, correction, deletion, and exceptions in plain language. |
| Security | Public policy materials describe safeguards, but an outside student cannot verify implementation [1]. | A policy does not prove that controls work. Seek evidence such as testing and audit results. |

## Major risks
Potential risks include unexpected secondary use, overexposure of public content, unclear third-party flows, profiling, retention uncertainty, and risks to younger users. These are review questions, not claims that each risk has occurred.

## Conclusion
Public materials describe collection, use, sharing, safeguards, and user controls. A policy review cannot establish how controls operate in practice. **Illustrative overall risk: Medium** (classroom judgment, not a measured platform-wide score).

## References
[1] Meta Privacy Policy: https://privacycenter.instagram.com/policy/
[2] Meta Privacy Center: https://privacycenter.instagram.com/
[3] Meta information controls: https://about.fb.com/news/2023/10/manage-your-information-across-apps/
[4] NIST Privacy Framework: https://www.nist.gov/privacy-framework
