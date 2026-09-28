# Practical 10: Data Privacy Case Studies

## Aim
Compare documented privacy incidents and regulatory findings, identify lessons, and connect them to the previous practicals.

## Case 1: Facebook and Cambridge Analytica
The FTC described deceptive collection by a third-party app and use of Facebook information for voter profiling and targeting [1]. This is a Facebook ecosystem case, not an Instagram-specific incident.
**Lessons:** review app access, enforce platform permissions, make disclosures accurate, audit third-party use, and provide meaningful controls.

## Case 2: Instagram child-user inquiry
In 2022 the Irish Data Protection Commission announced a €405 million fine and corrective measures regarding processing of child users' personal data. The inquiry included public disclosure of contact details through business-account features and public-by-default settings during the period examined [2].
**Lessons:** privacy by default, minimization, child-focused impact assessment, and clear notices matter in product design. The historical decision does not establish today's settings.

## Case 3: Equifax breach
The FTC reported that a 2017 Equifax breach affected about 147 million people and linked the incident to failure to take reasonable steps to secure its network [3].
**Lessons:** patch promptly, inventory exposed systems, monitor access, minimize retained data, and rehearse response.

## Comparison
| Case | Main issue | Course connection |
|---|---|---|
| Facebook/Cambridge Analytica | Third-party access, deception, profiling | Audit, policy clarity, consent, processor governance |
| Instagram child-user inquiry | Defaults and children's data | PIA, privacy by design, ethics, regulation |
| Equifax | Security weakness and large-scale exposure | Cryptography, operations, breach response |

## Common lessons and conclusion
Privacy needs more than encryption or a written policy. It depends on minimization, accurate notices, safe defaults, third-party oversight, secure engineering, user controls, and tested incident handling. These cases show different failure paths and connect the practical sequence from risk discovery to technical protection and accountability.

## References
[1] FTC, Facebook/Cambridge Analytica: https://www.ftc.gov/news-events/news/press-releases/2019/07/ftc-sues-cambridge-analytica-settles-former-ceo-app-developer
[2] Irish DPC, Instagram inquiry: https://www.dataprotection.ie/en/news-media/press-releases/data-protection-commission-announces-decision-instagram-inquiry
[3] FTC, Equifax breach: https://www.ftc.gov/news-events/news/press-releases/2019/07/equifax-pay-575-million-part-settlement-ftc-cfpb-states-related-2017-data-breach
[4] NIST Privacy Framework: https://www.nist.gov/privacy-framework
