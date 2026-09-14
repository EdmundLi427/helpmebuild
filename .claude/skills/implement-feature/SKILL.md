---
name: implement-feature
description: Use when the user wants a feature, fix, or change implemented in this repo — plans it, implements it, tests it, and reviews it before reporting back.
---
1. Read claude.md for this repo's current state, stack, and commands.
2. Delegate to the planner agent to produce a concrete plan for the task.
   If the repo is still empty/unscaffolded, the plan should include the
   minimal setup needed to get a working starting point.
3. Delegate to the implementer agent to carry out the plan.
4. Delegate to the test-runner agent to run this repo's real test/lint
   commands (if defined). If anything fails, send the failure back to the
   implementer and repeat this step — don't move on with known failures.
5. Delegate to the reviewer agent for an independent check of the diff.
6. Report a short summary to the user: what was built, what was verified,
   what (if anything) still needs their input or a decision.
