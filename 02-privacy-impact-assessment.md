# Practical 2: Privacy Impact Assessment of Instagram

## Aim
Map a data-processing activity, identify affected people and privacy risks, and select safeguards.

## Hypothetical assessment scenario
Consider an Instagram feature that recommends posts and accounts using profile, engagement, device, and content signals. This is a teaching scenario and does not assert access to Meta's internal systems. Meta's public policy describes broad data categories and uses, but this review does not verify the exact inputs or model behavior for any recommendation [1].

## Data subjects and potential effects
| Person | Example information | Potential effect |
|---|---|---|
| Account holder | Profile, posts, follows, likes, searches, comments, settings | Profiling, exposure, unwanted inference |
| Person shown or mentioned | Image, tag, location clue, comment | Identification or disclosure without their choice |
| Teen user | Profile, interactions, inferred interests | Greater impact from exposure or unsuitable recommendations |
| Creator/business | Public content and audience analytics | Disclosure of business and audience behavior |

## Simplified data flow
```text
Person/device → Instagram app → collection and processing → service delivery,
safety, personalization or analytics → permitted recipients under policy
→ account controls and support
```

## Risk register
| Risk | Likelihood | Impact | Initial rating | Candidate control |
|---|---|---|---|---|
| Audience setting exposes content | Medium | High | High | Clear audience indicator and review before posting |
| Activity supports sensitive inference | Medium | High | High | Limit sensitive inference; explain personalization and controls |
| Third-party access exceeds expectations | Low–Medium | High | Medium–High | Minimize shared data; review access; expire permissions |
| Teen information exposed | Medium | High | High | Age-appropriate defaults and teen-scenario testing |
| Data retained after purpose ends | Medium | Medium | Medium | Retention schedule and deletion verification |
| Account takeover | Medium | High | High | MFA, secure recovery, session controls, anomaly detection |

## Mitigation and residual risk
Assign each safeguard an owner and evidence: design review, permission test, retention report, or user test. Residual risk remains when users choose public sharing or others copy content; explain that limit clearly.

## Conclusion
Before launch, document the data inventory, purpose, audience defaults, retention, vendor access, and control testing. This is an educational example, not an assessment of Instagram's internal design.

## References
[1] Meta Privacy Policy: https://privacycenter.instagram.com/policy/
[2] Meta Privacy Center: https://privacycenter.instagram.com/
[3] NIST Privacy Framework: https://www.nist.gov/privacy-framework
