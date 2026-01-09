---
description: Commit (and optionally push) changes with proper message style
disable-model-invocation: true
---

User will instruct to commit or commit+push changes you have done.

**CRITICAL**: Never use destructive git commands (checkout --, reset --hard, clean -f) to discard uncommitted changes without explicit user instruction; if you encounter changes you don't understand or that appear unrelated, STOP and ask the user rather than discarding; prefer creating comprehensive commits over complex separation attempts; changes are presumed intentional until user confirms otherwise.

For that:

1. Use git status + any other git command needed to get a sense/recap of the current changes. Use cmd tool.
2. Add the relevant files with git add etc.
3. Commit with a proper commit message (take a look at previous commit messages with cmd tool to get a sense of the commit msgs style, tone and voice; NEVER EVER use line breaks; NEVER use markdown bulleted or numbered lists; separate concepts, ideas or changes or whatever with ";", always one line no matter how much info you put; NEVER EVER add signature, Co-Authored-By, or "Generated with Claude Code" - NO SIGNATURE UNDER ANY CIRCUMSTANCES; if working on a GitHub issue, reference it with (#XXX) at the end of the commit message).
4. If the instruction was to commit, it's done. If the instruction was to push, then push.
