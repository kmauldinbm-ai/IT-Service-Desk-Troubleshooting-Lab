# INC-002 — Windows 11 High CPU Usage

**Scenario:** Accounting user reports slow application launches and lag when switching between programs after Windows updates.

**Environment:** Windows 11, Task Manager, Windows Update, osTicket.

## Investigation (simulated)
- Obtained permission for remote support.
- Reviewed Task Manager: CPU utilization was 96%; Windows Modules Installer Worker was consuming approximately 78%.
- Checked Windows Update and found a pending restart.
- Confirmed the user had saved work before proceeding.

## Resolution and verification (simulated)
Restarted the workstation to complete updates. CPU utilization dropped to approximately 8%. User confirmed Excel, Outlook, and accounting software performed normally.

**Root cause in scenario:** Pending Windows Update restart associated with high CPU activity.

**Ticket:** #486543 — Resolved.

> This was a scripted support scenario documented in a local osTicket installation, not a live production incident.
