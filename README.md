# Incident Response Casebook

> Status: Planning

A collection of simulated, evidence-based incident investigations showing how alerts are validated, scoped, contained, and communicated in a controlled cybersecurity lab.

## Goals

- Demonstrate a repeatable investigation process.
- Connect endpoint, identity, authentication, and network evidence.
- Practice timelines, scoping decisions, and defensible conclusions.
- Separate facts, analyst inferences, and unanswered questions.
- Produce both technical case notes and concise executive summaries.

## Planned cases

| Case | Scenario | Main skills |
|---|---|---|
| IR-001 | Suspected account compromise | Authentication analysis, scoping, containment |
| IR-002 | Suspicious PowerShell execution | Process analysis, ATT&CK mapping, endpoint response |
| IR-003 | Unexpected exposed service | Network investigation, configuration review, remediation |
| IR-004 | Unauthorized privileged account | Identity investigation, change review, access control |
| IR-005 | Possible data staging | File activity, timeline analysis, evidence limitations |

All cases will use synthetic data generated in an isolated lab.

## Investigation method

1. Record the alert, source, and initial severity.
2. Preserve relevant evidence and document timestamps.
3. Separate confirmed facts from hypotheses.
4. Build a normalized event timeline.
5. Determine affected users, hosts, and data.
6. Map observed behavior to ATT&CK where supported by evidence.
7. Recommend containment and eradication steps.
8. Define recovery checks and monitoring.
9. Write technical and executive summaries.
10. Record lessons learned and detection improvements.

## Planned repository structure

```text
.
├── README.md
├── templates/
│   ├── case-report.md
│   ├── evidence-log.md
│   └── timeline.csv
├── cases/
│   └── IR-001-case-name/
│       ├── executive-summary.md
│       ├── technical-report.md
│       ├── evidence-log.md
│       ├── timeline.csv
│       └── lessons-learned.md
└── docs/
    ├── methodology.md
    └── handling-and-sanitization.md
```

## Case report standard

Each case will contain:

- Incident summary and severity
- Scope and assumptions
- Evidence inventory with provenance
- Timeline in a consistent timezone
- Confirmed findings
- Analyst assessments clearly labeled as inference
- ATT&CK mappings supported by observed behavior
- Containment, eradication, and recovery recommendations
- Detection and prevention improvements
- Outstanding questions and limitations
- Sanitized supporting artifacts

## Milestones

- [ ] Create reusable report, evidence, and timeline templates.
- [ ] Document evidence-handling and sanitization rules.
- [ ] Complete IR-001 with synthetic authentication logs.
- [ ] Complete IR-002 with endpoint and PowerShell telemetry.
- [ ] Complete IR-003 with network and server evidence.
- [ ] Add two advanced cases.
- [ ] Publish a case index and ATT&CK coverage table.
- [ ] Review every case for unsupported conclusions and sensitive data.

## Evidence policy

This repository will contain only synthetic or heavily sanitized lab evidence. It will not contain employer or customer data, credentials, personal information, malicious payloads, or confidential system details.

## References

- [NIST Incident Response](https://csrc.nist.gov/projects/incident-response)
- [MITRE ATT&CK](https://attack.mitre.org/)
