# Awesome Prompt Files [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of awesome prompt files for Visual Studio Code that enhance your coding experience with AI assistants.

## Contents

- [Official Resources](#official-resources)
- [Git Workflow Prompts](#git-workflow-prompts)
- [Code Quality & Analysis Prompts](#code-quality--analysis-prompts)
- [Testing & Documentation Prompts](#testing--documentation-prompts)
- [Tools & Utilities](#tools--utilities)
- [Community](#community)
- [Contributing](#contributing)

## Official Resources

- [VS Code Prompt Files Documentation](https://code.visualstudio.com/docs/copilot/copilot-customization#_prompt-files-experimental) - Official Microsoft documentation on prompt files
- [GitHub Copilot Prompt Engineering Guide](https://docs.github.com/en/copilot/using-github-copilot/prompt-engineering-for-github-copilot) - Best practices for prompt engineering

## Git Workflow Prompts

These prompts automate common Git workflow tasks using AI assistance in VS Code:

- [commit.prompt.md](.github/prompts/commit.prompt.md) - Automated commit message generation using conventional commit format
- [cr.prompt.md](.github/prompts/cr.prompt.md) - Comprehensive code review analysis for branch changes
- [pr.prompt.md](.github/prompts/pr.prompt.md) - Pull request description generation from commit messages

### Commit Automation
The `commit.prompt.md` file helps create proper conventional commits by:
- Analyzing changed files and grouping related changes
- Generating descriptive commit messages following conventional commit standards
- Ensuring commits are logically separated by domain/functionality

### Code Review Assistant
The `cr.prompt.md` file provides thorough code review by:
- Comparing current branch changes against main/master branch
- Evaluating code quality, functionality, performance, and security
- Providing constructive feedback and improvement suggestions
- Following a comprehensive review checklist

### Pull Request Generator
The `pr.prompt.md` file streamlines PR creation by:
- Extracting commit messages from the current branch
- Generating well-formatted markdown PR descriptions
- Automatically identifying the target main/master branch

## Code Quality & Analysis Prompts

These prompts help improve code quality, maintainability, and security:

- [refactor.prompt.md](.github/prompts/refactor.prompt.md) - Analyze code and suggest refactoring improvements following SOLID principles
- [security-audit.prompt.md](.github/prompts/security-audit.prompt.md) - Comprehensive security audit to identify vulnerabilities and suggest improvements
- [debug-assistant.prompt.md](.github/prompts/debug-assistant.prompt.md) - Systematic debugging with step-by-step troubleshooting approach

### Code Refactoring Assistant
The `refactor.prompt.md` file helps improve code quality by:
- Analyzing code structure and identifying improvement opportunities
- Checking compliance with SOLID principles
- Suggesting better naming, structure, and design patterns
- Prioritizing refactoring efforts by impact and complexity

### Security Audit Tool
The `security-audit.prompt.md` file provides comprehensive security analysis by:
- Identifying common vulnerabilities (OWASP Top 10)
- Analyzing input validation, authentication, and data protection
- Providing actionable security recommendations
- Creating implementation roadmaps for security improvements

### Debug Assistant
The `debug-assistant.prompt.md` file streamlines debugging by:
- Systematic error analysis and root cause identification
- Step-by-step troubleshooting methodology
- Solution development with preventive measures
- Testing strategies to verify fixes

## Testing & Documentation Prompts

These prompts enhance code testing coverage and documentation quality:

- [unit-test.prompt.md](.github/prompts/unit-test.prompt.md) - Generate comprehensive unit tests with edge cases and proper test structure
- [docstring.prompt.md](.github/prompts/docstring.prompt.md) - Create comprehensive docstrings and documentation for functions and classes

### Unit Test Generator
The `unit-test.prompt.md` file creates thorough test coverage by:
- Generating tests for happy path, edge cases, and error conditions
- Following testing best practices and framework conventions
- Creating realistic test data and proper mocking strategies
- Ensuring tests are independent and maintainable

### Documentation Generator
The `docstring.prompt.md` file improves code documentation by:
- Creating comprehensive docstrings following language conventions
- Documenting parameters, return values, and exceptions
- Providing usage examples and implementation notes
- Maintaining consistency across the codebase

## Tools & Utilities

- [VS Code Prompt Files Documentation](https://code.visualstudio.com/docs/copilot/copilot-customization#_prompt-files-experimental) - Official Microsoft documentation on prompt files
- [GitHub Copilot Prompt Engineering Guide](https://docs.github.com/en/copilot/using-github-copilot/prompt-engineering-for-github-copilot) - Best practices for prompt engineering

### How to Use These Prompts

1. **Copy prompt files** to your VS Code workspace in a `.github/prompts/` directory
2. **Reference prompts** in VS Code by typing `/promptFileName` in the chat
3. **Customize prompts** to match your specific project needs and conventions
4. **Use agent mode** (specified in the prompt frontmatter) for automated task execution

## Community

- [Discussions](../../discussions) - Community discussions and Q&A
- [Issues](../../issues) - Bug reports and feature requests
- [Wiki](../../wiki) - Additional documentation and guides

## Contributing

Contributions are welcome! Please read our [Contributing Guidelines](CONTRIBUTING.md) before submitting a pull request.

### How to Contribute

1. Fork this repository
2. Create a new branch for your prompt file
3. Add your prompt file to the `.github/prompts/` directory
4. Update this README with a link to your prompt
5. Submit a pull request

### Prompt File Guidelines

- Use the `.prompt.md` extension for VS Code prompt files
- Include frontmatter with `mode: agent` for automated tasks
- Provide clear task descriptions and expected behaviors
- Test your prompts with VS Code Copilot Chat
- Use descriptive filenames that indicate the prompt's purpose

## License

[![CC0](https://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, the contributors have waived all copyright and
related or neighboring rights to this work.
