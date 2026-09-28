# Practical 7: Privacy-Enhancing Technologies

## Aim
Compare technologies that may reduce privacy exposure while supporting legitimate service and analytics functions.

## Technology comparison
| Technology | Goal | Illustrative use | Limitation |
|---|---|---|---|
| Encryption | Prevent unauthorized reading | Protect account or message data | Does not block an authorized endpoint or key holder |
| Pseudonymization | Separate identity from analysis records | Internal analytics IDs | Linkage remains possible if keys or auxiliary data exist |
| Anonymization | Reduce identification in a release | Aggregate usage statistics | Re-identification risk can return when datasets are combined |
| Differential privacy | Bound one person's effect on aggregate output | Publish audience/usage statistics | Requires privacy-budget governance; can reduce accuracy |
| Federated learning | Avoid centralizing raw training examples | Learn from distributed signals | Updates can leak information; secure aggregation and tests matter |
| Homomorphic encryption | Compute on encrypted data | Specialized cloud analytics | High compute cost and limited use cases |
| Zero-knowledge proofs | Prove a claim without revealing its value | Privacy-preserving eligibility check | Complex design; does not solve unrelated collection |

## Selection exercise
1. Secure a login session: TLS encryption.
2. Share weekly engagement counts: aggregation, suppress small groups, and consider differential privacy.
3. Analyze support cases without exposing names: pseudonymize and restrict access; redact unnecessary message text.
4. Prove age eligibility without exposing a full birth date: evaluate a privacy-preserving credential/proof and test usability and abuse risks.

## Recommendations and conclusion
Start with minimization and purpose limitation. Choose a PET for a defined threat model, data sensitivity, desired utility, and key ownership. Test leakage and re-identification; document parameters and owners. PETs can make one processing step safer but do not guarantee privacy across the whole service. Combine them with access controls, transparency, retention limits, and user choice.

## References
[1] NIST Privacy-Enhancing Cryptography: https://csrc.nist.gov/projects/pec
[2] NIST Privacy Framework: https://www.nist.gov/privacy-framework
