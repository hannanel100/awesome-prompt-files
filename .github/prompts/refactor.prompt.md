---
mode: agent
description: Analyze code and suggest refactoring improvements following SOLID principles
---

Your task is to analyze the selected code and suggest refactoring improvements to enhance code quality, maintainability, and adherence to best practices.

## Analysis Focus Areas
 
### Code Structure
- Identify overly complex functions or classes that should be broken down
- Look for code duplication and suggest extraction opportunities
- Analyze coupling between components and suggest decoupling strategies

### SOLID Principles Compliance
- **Single Responsibility**: Check if classes/functions have multiple responsibilities
- **Open/Closed**: Identify areas that could benefit from extension points
- **Liskov Substitution**: Review inheritance hierarchies for proper substitutability
- **Interface Segregation**: Look for overly broad interfaces that should be split
- **Dependency Inversion**: Suggest dependency injection opportunities

### Code Quality Improvements
- Identify magic numbers, strings, and suggest constants
- Look for nested conditionals that could be simplified
- Suggest better naming for variables, functions, and classes
- Identify potential performance improvements

## Output Format

Provide your analysis in this structure:

```markdown
## Refactoring Analysis

### Current Issues Identified
- [List specific issues found in the code]

### Recommended Improvements

#### 1. [Issue Category]
**Problem**: [Describe the issue]
**Solution**: [Explain the refactoring approach]
**Benefit**: [Explain why this improves the code]

```code
[Show the refactored code example]
```

#### 2. [Next Issue Category]
[Repeat the pattern]

### Priority Recommendations
1. **High Priority**: [Most critical refactoring needs]
2. **Medium Priority**: [Important but not urgent improvements]
3. **Low Priority**: [Nice-to-have improvements]

### Implementation Notes
- [Any specific considerations for implementing these changes]
- [Potential risks or breaking changes to watch for]
```

## Guidelines
- Focus on practical, actionable improvements
- Explain the reasoning behind each suggestion
- Consider the existing codebase patterns and conventions
- Prioritize changes by impact and effort required
- Suggest incremental refactoring steps when dealing with large changes
