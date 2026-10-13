# QA Review Guidelines (Invite-only)

## Purpose

- Ensure testing is reproducible, actionable, and focused.
- Provide clear signals to engineers for prioritization.

## Before you begin

- Confirm you have the correct private build and access credentials.
- Back up any device you use for testing. Use disposable hardware where possible.
- Read TEST_PLAN.md and select the scope of your review session.

## During a review session

- Work in short focused sessions (30–90 minutes) and document time stamps.
- Capture screenshots or short screen recordings for UI bugs.
- Save logs immediately after reproducing an issue.
- Attempt to reproduce a fault at least twice before filing a bug.

## When filing an issue

- Use the Bug Report template.
- Provide exact reproduction steps with timings, keystrokes, and menu names.
- Attach logs, screenshots, and the machine/VM config.
- Assign a severity level (Blocker/Major/Minor/Trivial).
- If the issue is security-sensitive, follow SECURITY.md and do not publish it publicly.

## Scope & boundaries

- Focus on reproducibility and clear technical failure modes.
- If a test requires hardware that you do not have, mark it Blocked and indicate required hardware.

## Communication

- Use the private testing channel for coordination and triage questions.
- Keep public discussion minimal — this repo is invite-only.
