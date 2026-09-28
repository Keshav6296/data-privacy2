# Practical 8: Privacy Breach Response Plan

## Aim
Prepare a response workflow for a hypothetical incident involving personal information.

## Hypothetical scenario
A staff member reports that an internal analytics export containing account IDs and engagement records was exposed through misconfigured storage. This is a classroom scenario, not an allegation that Instagram experienced this incident.

## Response sequence
```text
Detect → Triage → Contain → Investigate → Decide notification → Recover → Review
```

## Roles
- **Incident lead:** coordinates decisions and maintains timeline.
- **Security team:** contains access, preserves logs, investigates cause.
- **Privacy/legal team:** assesses affected people, jurisdiction, and notification duties.
- **Communications lead:** prepares accurate user messages.
- **Service owner:** restores service and tracks corrective actions.

## First-response checklist
1. Preserve logs and evidence; record each change.
2. Restrict public access, revoke exposed credentials, and isolate affected systems.
3. Identify fields, time period, people affected, and whether the file was accessed.
4. Assess ongoing exposure and risk, including risk to minors.
5. Ask privacy/legal reviewers to determine applicable duties and deadlines for each jurisdiction; there is no universal deadline.
6. Explain what is known, unknown, what was done, and what affected people can do.
7. Restore only after verification; rotate keys/credentials when needed.
8. Review root cause and test corrective actions.

## Notification outline
“On [date], we identified [plain-language description]. Information potentially involved: [categories]. We have [actions]. We are investigating [unknowns]. If affected, please [specific action]. Contact [support channel].”

## Tabletop questions
Who can authorize containment? How will you learn if the file was downloaded? Who needs direct notice? What evidence must be preserved? Which laws apply? What changes if messages, precise location, or teen-user data were included?

## Conclusion
A response balances speed, evidence preservation, user protection, and accurate communication. Document and rehearse the plan; base notifications on confirmed facts and applicable law.

## References
[1] NIST SP 800-61 Rev. 2: https://csrc.nist.gov/pubs/sp/800/61/r2/final
[2] GDPR text: https://eur-lex.europa.eu/eli/reg/2016/679/oj/eng
[3] India DPDP Act: https://www.meity.gov.in/static/uploads/2024/06/2bf1f0e9f04e6fb4f8fef35e82c42aa5.pdf
