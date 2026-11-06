# INC-003 — DNS Resolution Failure

**Scenario:** User cannot open websites despite an active Ethernet connection.

**Environment:** Windows 11, TCP/IP, DNS, DHCP concepts, osTicket.

## Findings (simulated)
- Workstation IPv4: `192.168.10.45/24`; gateway: `192.168.10.1`.
- Configured DNS: `192.168.10.99`; documented DNS: `192.168.10.10`.
- `ping 8.8.8.8` succeeded, suggesting external IP connectivity.
- `nslookup google.com` timed out using the configured DNS.
- `nslookup google.com 192.168.10.10` succeeded.

## Workaround and escalation (simulated)
Configured the workstation to use the approved DNS server `192.168.10.10` and confirmed websites loaded. Recommended Tier 2 investigate DHCP scope option 006 and possible workstation DNS overrides.

**Important distinction:** The incorrect DNS value was observed, but its source was not established. DHCP misconfiguration is a hypothesis, not a confirmed root cause.

**Ticket:** #477065 — Open; workaround validated, investigation pending. Ticket history includes an initial resolved state followed by reopening.

> This was a scripted support scenario documented in a local osTicket installation, not a live production incident.
