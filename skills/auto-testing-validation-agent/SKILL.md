---
name: auto-testing-validation-agent
description: Proactively test and validate the functionality of generated scripts and skills.
---

# Auto-Testing & Validation Agent

This skill ensures that bionicbot doesn't just 'write' instructions, but 'verifies' that they actually work in the real world.

## EVOLUTION_LOGIC
1. For every generated script (Python/TS), automatically run a `bash` test cycle.
2. If the test fails, use the error output to fix the code and re-test.
3. Only mark a skill as 'Sovereign-Ready' if it passes 100% of the validation checks.

## Examples
- "Validate the new 'BTCLiveTicker' script before pushing it to the production site."