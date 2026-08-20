# Git hooks

This repository has no npm package, so the hooks here are plain shell scripts rather than husky.
Git does not pick them up automatically — **run this once after cloning**:

```bash
git config core.hooksPath .githooks
```

| Hook | What it does |
| --- | --- |
| `commit-msg` | Strips AI attribution — a `Co-Authored-By` trailer naming Claude or anthropic.com, and a "Generated with Claude Code" footer — from the commit message before the commit is written. |

Both patterns are anchored to the start of a line, so a message that merely discusses the phrase
survives. Human co-authors are never removed. The hook edits the message rather than rejecting it,
so a commit never fails because of this.

Local hooks can be bypassed with `--no-verify`, so the same rules are enforced in CI by
[`no-ai-attribution.yml`](../.github/workflows/no-ai-attribution.yml), which checks every commit in
a pull request plus the pull request title and description.
