# Scenario 01 — Requirement

## Business Requirement

When an Incident is moved to the **Resolved** state, the **Resolution notes** field must become mandatory.

The user should not be able to save the Incident as Resolved without providing Resolution notes.

---

## Table

**Incident [incident]**

---

## Fields Involved

- State
- Resolution notes

---

## User

- Incident user
- ServiceNow system

---

## Trigger

The Incident State changes to **Resolved**.

---

## Expected Behavior

When:

```text
State = Resolved
