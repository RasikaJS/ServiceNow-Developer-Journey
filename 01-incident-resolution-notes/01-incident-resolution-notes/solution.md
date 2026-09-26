# Solution

## Selected ServiceNow Feature

UI Policy

## Configuration

### Table

Incident [incident]

### Condition

State is Resolved

### UI Policy Action

Field:

Resolution notes

Mandatory:

True

## Configuration Flow

Incident
   ↓
State = Resolved
   ↓
UI Policy condition becomes true
   ↓
UI Policy Action executes
   ↓
Resolution notes becomes mandatory

## Why UI Policy?

The requirement is related to form behavior.

When the Incident State changes to Resolved, the Resolution notes field should become mandatory.

## UI Action

No UI Action is required for this requirement.

## Important Note

This solution controls behavior on the form.

It does not by itself provide server-side protection for updates performed through integrations, imports, APIs, background scripts, or other server-side mechanisms.
