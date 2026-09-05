# Premyz

*(pronounced "PREM-iz")*

**Your coding agent starts writing before it knows what you want.**

You describe a feature. The agent starts writing files in thirty seconds. Ten minutes
later you have four hundred lines that solve a slightly different problem, on an
architecture nobody chose, and you can't tell which of your original constraints
survived. The bug isn't code quality — it's that intent was never written down, so
there was nothing to check the output against.

Premyz is a set of Claude Code commands that make an agent understand a codebase
before it changes one.

## Built for the repo you already have

Most tools in this space assume you're starting fresh: write a spec, then build.
Almost nobody works that way. Real work happens in a repo that already exists, has no
documentation, and whose intent lives in one person's head or nowhere at all.

That means there are **two sources of truth, and they disagree**:
