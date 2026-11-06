# INC-001 — Mapped Drive Access Denied

**Scenario:** User cannot access a previously mapped M: drive and receives "Access Denied."

**Environment:** Windows 11 workstation, Active Directory security groups, SMB share and NTFS permissions, osTicket.

## Investigation (simulated)
- Confirmed the drive was mapped and connected.
- Checked the account was enabled and belonged to the Avengers security group.
- Reviewed share and NTFS permissions.
- Compared current logon group membership using `whoami /groups`; the group was absent from the current access token.

## Resolution (simulated)
User signed out and back in to refresh the Windows logon token. Group membership then appeared in `whoami /groups`, and the mapped drive was accessible.

**Likely root cause in scenario:** Stale Windows logon token after group membership change.

**Ticket:** #777882 — Resolved.

> This was a scripted support scenario documented in a local osTicket installation, not a live production incident.
