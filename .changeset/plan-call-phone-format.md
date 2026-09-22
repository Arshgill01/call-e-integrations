---
"@call-e/cli": patch
---

Validate `--to-phone` locally in `calle call plan` and `calle call start` so malformed or fictional numbers fail as a format problem instead of being forwarded to `plan_call`, where they could be mislabeled as an unsupported region.

Fixes #144
