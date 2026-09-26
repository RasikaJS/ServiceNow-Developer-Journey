# Scenario 01 — Incident Resolution Notes Mandatory

## Difficulty

Basic

## Business Requirement

When an Incident is moved to Resolved, the Resolution notes field must become mandatory.

The user should not be able to save the Incident as Resolved without entering Resolution notes.

## ServiceNow Table

Incident [incident]

## Fields Involved

- State
- Resolution notes

## Requirement Analysis

When the Incident State becomes Resolved:

Resolution notes → Mandatory

## Selected ServiceNow Feature

UI Policy

## UI Policy Configuration

Table:

Incident [incident]

Condition:

State is Resolved

## UI Policy Action

Field:

Resolution notes

Mandatory:

True

## Why UI Policy?

The requirement is related to dynamic form behavior.

When the Incident State changes to Resolved, the Resolution notes field should become mandatory.

## UI Action

No UI Action is required for this requirement.

## Expected Behavior

### Before Resolution

Resolution notes should not be mandatory.

### When State = Resolved

Resolution notes should become mandatory.

### Resolved + Empty Resolution Notes

The user should not be able to save the Incident.

### Resolved + Resolution Notes Provided

The Incident should save successfully.

## Key Learning

UI Policy can be used to dynamically control field behavior on a form based on a condition.

## Developer Question

Does a UI Policy protect data when a record is updated through an API,
import, integration, background script, or another server-side mechanism?

This will be explored in a later advanced scenario.
