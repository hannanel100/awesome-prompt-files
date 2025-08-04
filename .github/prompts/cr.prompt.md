---
mode: agent
description: Comprehensive code review analysis for branch changes against main/master
---

Your task is to run a code review on the code in the current branch that is not in the main/master branch (use `git branch -a` to find the main/master branch). Only review code that is not in the main branch. If there is no code to review, return "No code to review".

## Code Review Instructions
- Review the code changes in the current branch
- Focus on the quality, functionality, performance, and security of the code
- Provide constructive feedback and suggestions for improvement
- Ensure that the code adheres to best practices and coding standards
- Give a summary of the changes made in the code
- If the code is ready for merging, approve it with a comment

## Code Review Checklist
- **Code Quality**: Is the code clean, readable, and maintainable?
- **Functionality**: Does the code work as intended? Are there any bugs or issues?
- **Performance**: Are there any performance issues or optimizations that can be made?
- **Security**: Are there any security vulnerabilities or concerns?