# Practical 5: Anonymization Techniques for Data Privacy

## Aim
Transform a small synthetic social-media dataset for analysis and explain why removing names alone does not guarantee anonymity.

## Synthetic dataset
These rows are invented for teaching and are not Instagram user data.
| ID | Age | City | Posts/week | Topic viewed |
|---|---:|---|---:|---|
| Asha | 19 | Jaipur | 8 | Health |
| Bharat | 20 | Jaipur | 6 | Finance |
| Chitra | 21 | Pune | 12 | Health |
| Dev | 22 | Pune | 4 | Education |
| Esha | 38 | Kochi | 10 | Health |

## Transformation exercise
- **Suppression:** remove direct IDs and sensitive-topic values if the research question does not need them.
- **Generalization:** use age bands and broad regions instead of exact age and city.
- **Masking:** replace names with random study IDs; keep any re-identification key separately with restricted access. This is pseudonymization, not anonymization.
- **Aggregation:** report group counts or averages instead of row-level records.
- **Noise addition:** use a defined privacy mechanism and budget for published statistics; arbitrary noise is not differential privacy.

## Re-identification analysis
An attacker may combine age, city, posting patterns, timestamps, or public profiles with outside information. Rare combinations create risk. Removing names does not eliminate linkability; public images and posts may reveal identity. Consider the whole release, including metadata and repeated queries.

## Procedure
1. Define the question and minimum necessary fields.
2. Identify direct identifiers, quasi-identifiers, and sensitive attributes.
3. Generalize or suppress risky values; check uniqueness and small groups.
4. Test plausible linkage attacks with realistic auxiliary data.
5. Restrict access, set retention dates, and document residual risk.
6. Reassess when datasets are combined or published widely.

## Result and conclusion
The small synthetic dataset could still contain unique combinations after simple transformations. For this example, avoid publishing row-level records; release only coarse aggregates. Anonymization is an ongoing risk-management process, not a one-time deletion of names.

## References
[1] NIST Privacy Framework: https://www.nist.gov/privacy-framework
[2] NIST Privacy-Enhancing Cryptography: https://csrc.nist.gov/projects/pec
