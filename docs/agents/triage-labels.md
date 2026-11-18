# Triage label mapping

Skills read these exact label strings from the issue tracker. If your tracker uses different names, edit this file (not the skill); the skill will apply what you configure.

## Canonical roles

| Role | GitHub / GitLab label | Meaning |
|------|------------------------|---------|
| `needs-triage` | `needs-triage` | Issue not yet reviewed by a maintainer |
| `needs-info` | `needs-info` | Awaiting reporter clarification |
| `ready-for-agent` | `ready-for-agent` | Agent can pick up; sufficient context |
| `ready-for-human` | `ready-for-human` | Human action needed (design, decision, merge, release) |
| `wontfix` | `wontfix` | Will not be addressed |

## Notes

- The `triage` skill applies these labels on GitHub via `gh issue edit <n> --add-label "..."`. Ensure labels exist in the repo (e.g. `gh label create "needs-triage" --description "..."`).
- This repo uses GitHub Issues; create missing labels as needed before running triage workflows.
