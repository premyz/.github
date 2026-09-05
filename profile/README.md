# Premyz

*(pronounced "PREM-iz")*

**Your coding agent starts writing before it knows what you want.**

You describe a feature. The agent starts writing files in thirty seconds. Ten minutes
later you have four hundred lines that solve a slightly different problem, on an
architecture nobody chose, and you can't tell which of your original constraints
survived. The bug isn't code quality — it's that intent was never written down, so
there was nothing to check the output against.

Premyz is a Claude Code plugin with one command.

```
/intent
```

It reads the repository you already have, tells you what it thinks the project is,
and interviews you to correct it. The result is `docs/INTENT.md` — two pages of plain
markdown your agent reads before it writes code.

## Why brownfield

Most tools in this space assume you're starting fresh: write a spec, then build.
Almost nobody works that way. Real work happens in a repo that already exists, has no
documentation, and whose intent lives in one person's head or nowhere at all.

Asked to describe an inherited project from a blank page, you'll write something
vague. Shown a specific and slightly wrong description, you'll correct it precisely.
Premyz opens with the description.

## What `INTENT.md` holds

- The problem, stated without a solution in it
- Who it's for, and who it explicitly isn't for
- What success looks like, observably
- Constraints — separating the ones you chose from the ones you inherited
- What's explicitly out of scope
- Open questions, recorded verbatim rather than quietly answered
- Assumptions, each with the evidence in the code that supports it

## Principles

- **Zero network calls.** No telemetry, no analytics, no update check. Read the
  source and verify it yourself.
- **Writes exactly one file.** After a run, `git status` shows one change.
- **The artifact is yours.** Plain markdown in your repo. Works with any agent.
  Outlives this project.
- **Free and complete.** MIT. No gate, no trial, no upgrade prompt in the tool.

## Status

Not released yet — first release targeted for **October 2026**.
Watch [premyz/premyz](https://github.com/premyz/premyz) if you want to know when.

If you want a full development methodology rather than one file,
[spec-kit](https://github.com/github/spec-kit) and
[BMAD-METHOD](https://github.com/bmad-code-org/BMAD-METHOD) are good, and free.
Premyz is deliberately smaller.
