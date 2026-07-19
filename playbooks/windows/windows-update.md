# Windows Update

## Purpose

This module helps OpsForge understand, diagnose, and resolve Windows Update issues using evidence-based and low-risk troubleshooting.

It covers failed updates, stuck downloads, installation rollbacks, servicing corruption, and repeated update errors.

---

## Scope

This module applies to:

- Windows workstations
- Enterprise-managed devices
- Feature updates
- Quality updates
- Driver updates delivered through Windows Update

Management platforms such as Intune or Configuration Manager may require additional organization-specific investigation.

---

## How Windows Update Works

Windows Update generally performs these stages:

1. Checks for applicable updates
2. Downloads update files
3. Stages the files
4. Installs the update
5. Restarts when required
6. Verifies or rolls back the installation

Knowing where the failure occurs helps narrow the possible cause.

---

## Common Symptoms

- Update repeatedly fails
- Download remains at the same percentage
- Installation remains pending
- Computer rolls back after restarting
- Windows displays an update error code
- Update history shows repeated failures
- Device becomes slow during servicing
- DISM or SFC reports corruption

---

## Initial Questions

Before recommending repairs, determine:

- What is the exact error code?
- Which update is failing?
- At what stage does it fail?
- How long has the issue existed?
- Is a restart pending?
- Is internet connectivity working?
- Is sufficient disk space available?
- What troubleshooting has already been completed?
- Is the device managed by enterprise update policies?

---

## Evidence to Collect

Collect only the evidence needed for the next decision.

### Windows version

```powershell
winver
