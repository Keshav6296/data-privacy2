# Practical 4: Cryptography for Data Privacy

## Aim
Explain how cryptography supports confidentiality, integrity, and authentication in a social platform, and distinguish encryption from hashing.

## Techniques
| Technique | Function | Suitable use |
|---|---|---|
| Symmetric encryption | Same secret key encrypts and decrypts | Protect stored records or data in an established secure session |
| Public-key cryptography | Public/private key pair | Key exchange, certificates, digital signatures |
| Cryptographic hash | Fixed-size digest; not reversible encryption | Integrity checks and components of authentication |
| Password hashing | Salted, slow password verifier | Store credentials; never store plaintext passwords |
| Digital signature | Binds data to signing key | Verify authenticity and detect tampering |

## Data lifecycle example
1. Browser establishes HTTPS/TLS and verifies the service certificate.
2. Authentication stores a password verifier using a dedicated password-hashing algorithm, not a raw password or plain fast hash.
3. Sensitive stored records are encrypted where appropriate; keys are kept separate and access limited.
4. Plan key rotation, backup protection, recovery, and audit logging along with encryption [1].
5. Use integrity checks where the system needs evidence data has not changed.

## Classroom exercise
Use the fictional record `user=U17; visibility=private; location=hidden`.
- Explain what TLS protects while the record travels over a network.
- Explain what database encryption protects if storage media is lost.
- Why does encryption not stop an authorized, overprivileged employee from reading it?
- Why can a SHA-256 digest not recover the record, and why is SHA-256 alone not an appropriate password-storage scheme?
- Who should control the encryption key? What if it is lost or compromised?

## Limitations
Cryptography does not decide whether data should be collected, who should see it, or how long it should be kept. Weak key management, insecure endpoints, or excessive permissions can defeat strong algorithms. Use reviewed libraries and protocols; do not invent a cipher.

## Conclusion
Encryption, password hashing, signatures, and key management solve different problems. Combine them with access control, minimization, retention limits, and incident response.

## References
[1] NIST SP 800-57 Key Management: https://csrc.nist.gov/pubs/sp/800/57/pt1/r5/final
[2] Meta Privacy Policy: https://privacycenter.instagram.com/policy/
