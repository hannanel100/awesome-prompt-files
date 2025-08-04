# Awesome Prompt Files [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of awesome prompt files for Visual Studio Code that enhance your coding experience with AI assistants.

## Contents

- [Official Resources](#official-resources)
- [Git Workflow Prompts](#git-workflow-prompts)
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
