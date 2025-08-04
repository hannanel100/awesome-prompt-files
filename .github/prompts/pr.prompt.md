---
mode: agent
description: Generate comprehensive pull request description following industry best practices
---

Your task is to create a comprehensive PR description from the current branch to the main/master branch (use `git branch -a` to find the main/master branch).

## Instructions
Analyze the commit messages and code changes from the current branch, then generate a well-structured PR description following the template below.

## PR Description Template

Use this exact structure and format for the output:

```markdown
## What?
[Explain the changes you've made in explicit prose. Reference any relevant tickets but don't just reference them - explain what the change is first. Be concise but descriptive. If needed, ask the user for more information about the ticket or context.]

## Why?
[Explain the business or engineering goal this change achieves. What problem does it solve? What objective does it move forward? Connect the technical change to the bigger picture.]

## How?
[Highlight significant design decisions and implementation approach. Why did you choose this particular solution? Draw attention to important architectural or technical choices.]

## Testing?
[Describe how the changes were tested. Include information about:
- What tests were added or modified
- How to test the changes locally if needed
- Any edge cases or conditions not tested and why
- Results of manual testing if applicable]

## Screenshots (optional)
[Include screenshots for UI changes, CLI output, or any visual results that help reviewers understand the impact]

## Anything Else?
[Optional section for:
- Technical debt considerations
- Future improvements or optimizations
- Architecture implications
- Challenges encountered
- Alternative approaches considered]
```

## Guidelines
- Be explicit and use complete sentences with active voice
- Keep descriptions concise but informative - aim for clarity over brevity
- Focus on helping the reviewer understand both the technical changes and business context
- Use conversational, prose-like language rather than terse fragments
- If referencing tickets, explain the change first, then reference the ticket
- Highlight any security, performance, or architectural considerations