# IT Service Desk Troubleshooting Lab

A hands-on **osTicket workflow and scenario-based troubleshooting portfolio** for Tier 1 service desk support, prioritization, customer communication, incident documentation, validation, and escalation.

> **Transparency:** All tickets represent simulated incidents. The osTicket records and screenshots were created in a local lab. Troubleshooting commands, outputs, user interactions, and resolutions described here were scenario exercises, not evidence of production work or live execution on the described workstations.

## Lab stack
- osTicket hosted locally using XAMPP (Apache and MySQL) on a Windows virtual machine
- Windows 11 and Windows Server / Active Directory home lab for related identity and permissions practice
- Scenario-based Windows and network troubleshooting

## Incident index
| Case | Problem | Outcome |
|---|---|---|
| [INC-001](INC-001-Mapped-Drive/README.md) | Mapped drive access denied / stale AD group token | Resolved in scenario |
| [INC-002](INC-002-High-CPU/README.md) | High CPU / pending Windows Update restart | Resolved in scenario |
| [INC-003](INC-003-DNS-Resolution/README.md) | DNS lookup failure despite working IP connectivity | Workaround validated; escalation recommended |

## Support workflow practiced
1. Clarify symptoms and business impact.
2. Establish scope and authorization.
3. Form and test hypotheses.
4. Apply an approved remedy or workaround.
5. Verify the result with the user.
6. Record evidence, uncertainty, and escalation requirements.

## Related projects
- [Active Directory Lab](https://github.com/kmauldinbm-ai/ActiveDirectory-Lab)
- [Networking Labs](https://github.com/kmauldinbm-ai/networking-labs)
- [NOC Monitoring and Incident Response](https://github.com/kmauldinbm-ai/noc-network-monitoring-incident-response)

## Screenshot note
All names, addresses, and events are part of a fictional training scenario. The six osTicket screenshots are uploaded in their corresponding incident folders.
