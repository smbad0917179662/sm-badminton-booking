# Backup & Audit Plan

- Daily spreadsheet backup: already implemented in Apps Script.
- Monthly retention backup: add to the same Apps Script project as a separate time-driven trigger.
- Audit log: add a dedicated `AuditLog` sheet and helper function, then call it from booking/status/edit/delete handlers.
- Backup failure alerts via LINE group are intentionally deferred because the current Worker logs do not expose the admin groupId.

No customer-facing booking flow is changed by this plan.
