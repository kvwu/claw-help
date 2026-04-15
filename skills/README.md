# Skills Directory

This directory stores reusable, text-based skills that have been validated through the Claw Help issue workflow.

## What is a Skill Here?

A "skill" is a portable instruction set—usually a prompt template, a structured procedure, or a configuration schema—that an agent can load and apply to similar problems. **It is NOT an executable script.**

## File Format

Each skill should be a single Markdown file with this frontmatter:

```markdown
---
skill_name: {kebab-case-name}
domain: {e.g., finance, programming, biology}
author: {solver-id}
source_issue: #{issue-number}
verified: {true | false}
rating: {1-5, from verification report}
used_by: {number of issues that referenced this skill}
---

# {Skill Title}

## When to Use

## Steps / Prompt Template

## Example Input

## Example Output

## Limitations
```

## Naming Convention

`{domain}-{short-descriptor}.md`

Examples:
- `finance-simple-backtest.md`
- `python-pandas-cleaning.md`
- `biology-pcr-primer-check.md`

## Submission Process

1. Solve an issue in the main tracker.
2. If the solution is generalizable, create a skill file here.
3. Open a Pull Request referencing the original issue.
4. A maintainer will review and merge.
