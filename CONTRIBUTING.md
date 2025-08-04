# Contributing to Awesome Prompt Files

Thank you for your interest in contributing to Awesome Prompt Files! This repository aims to collect high-quality prompt files that enhance the VS Code development experience with AI assistants.

## How to Contribute

### 1. Fork and Clone
1. Fork this repository
2. Clone your fork locally
3. Create a new branch for your contribution

```bash
git clone https://github.com/YOUR_USERNAME/awesome-prompt-files.git
cd awesome-prompt-files
git checkout -b add-my-prompt
```

### 2. Add Your Prompt File
- Place your prompt file in the `.github/prompts/` directory
- Use the `.prompt.md` extension
- Follow the naming convention: `descriptive-name.prompt.md`

### 3. Update the README
- Add your prompt to the appropriate section in `README.md`
- Include a brief description of what your prompt does
- Follow the existing format and style

### 4. Submit a Pull Request
1. Commit your changes using conventional commit format
2. Push to your fork
3. Create a pull request with a clear description

## Prompt File Guidelines

### File Structure
```markdown
---
mode: agent
---
Your prompt instructions here...
```

### Frontmatter Requirements
- Include `mode: agent` for prompts that should run automatically
- Omit frontmatter or use `mode: chat` for interactive prompts

### Content Guidelines
- **Clear Purpose**: Each prompt should have a specific, well-defined purpose
- **Actionable Instructions**: Provide clear, step-by-step instructions for the AI
- **Context Awareness**: Include necessary context about the task or environment
- **Output Format**: Specify the expected output format when relevant

### Quality Standards
- **Tested**: Test your prompt with VS Code Copilot Chat before submitting
- **Documented**: Include comments or descriptions for complex logic
- **Focused**: Each prompt should do one thing well
- **Reusable**: Prompts should work across different projects and contexts

## Prompt Categories

We organize prompts into the following categories:

### Git Workflow Prompts
Prompts that automate Git-related tasks:
- Commit message generation
- Code review automation
- Pull request descriptions
- Branch management

### Development Workflow Prompts
Prompts that enhance general development tasks:
- Code refactoring
- Documentation generation
- Testing assistance
- Project setup

### Code Quality Prompts
Prompts focused on improving code quality:
- Code review checklists
- Security audits
- Performance optimization
- Best practices enforcement

## Example Contributions

### Good Prompt Example
```markdown
---
mode: agent
---
Generate unit tests for the selected function or class. 

Requirements:
- Use the same testing framework as existing tests in the project
- Include edge cases and error scenarios
- Follow the project's testing conventions
- Add descriptive test names and comments
```

### What Makes a Good Prompt
- **Specific**: Clearly defines what should be done
- **Contextual**: Considers the project environment
- **Flexible**: Works across different codebases
- **Professional**: Follows best practices

## Code of Conduct

- Be respectful and inclusive in all interactions
- Provide constructive feedback on pull requests
- Help maintain the quality and usefulness of the collection
- Follow GitHub's community guidelines

## Questions and Support

- **Discussions**: Use [GitHub Discussions](../../discussions) for questions and ideas
- **Issues**: Report bugs or request features via [GitHub Issues](../../issues)
- **Wiki**: Check the [Wiki](../../wiki) for additional documentation

## Review Process

1. **Automated Checks**: PRs are automatically checked for basic formatting
2. **Community Review**: Other contributors may review and provide feedback
3. **Maintainer Review**: Final review by repository maintainers
4. **Merge**: Approved PRs are merged and the contributor is credited

## Recognition

Contributors are recognized in several ways:
- Listed in the repository contributors
- Mentioned in release notes for significant contributions
- Added to the project's acknowledgments

## License

By contributing to this repository, you agree that your contributions will be licensed under the same [CC0 1.0 Universal](LICENSE) license as the project.

---

Thank you for helping make VS Code development better for everyone! 🚀
