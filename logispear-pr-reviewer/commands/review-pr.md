---
name: review-pr
description: Review any GitHub PR. Pass the PR URL or owner/repo#N as the argument.
argument-hint: [pr-url-or-ref]
---

Review the GitHub PR `$ARGUMENTS` using the `logispear-pr-reviewer` skill. Follow the skill's 8-step workflow: parse the PR reference, gather CI checks, fetch the diff, classify each failing check, scan code quality, set overall status, set the ready flag, and emit the structured verdict.

If `$ARGUMENTS` is empty, ask the user for a PR URL or `owner/repo#N` reference and stop.
