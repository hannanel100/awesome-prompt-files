---
mode: agent
description: Systematically debug errors and issues with step-by-step troubleshooting approach
---

Your task is to help debug errors and issues in the code using a systematic, methodical approach. Analyze the problem, identify potential causes, and provide actionable solutions.

## Debugging Methodology

### 1. Problem Analysis
- **Error Classification**: Identify the type of error (syntax, runtime, logic, performance)
- **Error Message Analysis**: Break down error messages and stack traces
- **Context Understanding**: Analyze the code context where the error occurs
- **Reproduction Steps**: Understand how to reproduce the issue consistently

### 2. Root Cause Investigation
- **Data Flow Analysis**: Trace how data moves through the problematic code
- **State Inspection**: Examine variable states and object properties
- **Execution Path**: Identify the sequence of operations leading to the error
- **Dependencies Check**: Verify external dependencies and their versions

### 3. Solution Development
- **Immediate Fixes**: Quick solutions to resolve the immediate issue
- **Preventive Measures**: Changes to prevent similar issues in the future
- **Testing Strategy**: How to verify the fix works correctly
- **Monitoring**: What to watch for to ensure the fix is effective

## Debugging Output Format

Provide your analysis in this structured format:

```markdown
## Debug Analysis

### Problem Summary
**Error Type**: [Syntax/Runtime/Logic/Performance/Other]
**Severity**: [Critical/High/Medium/Low]
**Affected Components**: [List components/modules involved]

### Error Details
**Error Message**: 
```
[Paste the exact error message]
```

**Stack Trace Analysis**:
- [Line-by-line explanation of the stack trace]
- [Identification of the root cause location]

### Investigation Findings

#### Data State Analysis
- **Variables**: [Current values and expected values]
- **Object States**: [Object properties and their states]
- **Input Data**: [Analysis of input data quality and format]

#### Code Flow Analysis
- **Execution Path**: [Step-by-step execution flow to the error]
- **Branching Logic**: [Analysis of conditional statements]
- **Loop Behavior**: [Analysis of loop conditions and iterations]

### Root Cause
**Primary Cause**: [Main reason for the error]
**Contributing Factors**: [Secondary issues that compound the problem]

### Solutions

#### Immediate Fix
```code
[Provide the corrected code]
```
**Explanation**: [Why this fix resolves the issue]

#### Preventive Measures
1. **Input Validation**: [Add necessary validation]
2. **Error Handling**: [Improve error handling]
3. **Defensive Coding**: [Add protective measures]

#### Testing Verification
```code
// Test cases to verify the fix
[Provide test cases or verification steps]
```

### Additional Recommendations
- **Code Review**: [Areas that need additional review]
- **Monitoring**: [What to monitor going forward]
- **Documentation**: [Documentation updates needed]
```

## Common Debugging Scenarios

### Runtime Errors
- **Null/Undefined References**: Check for null pointer exceptions
- **Type Errors**: Verify data types and conversions
- **Index Out of Bounds**: Validate array/list access
- **Resource Unavailable**: Check file, network, or database connectivity

### Logic Errors
- **Incorrect Calculations**: Verify mathematical operations and formulas
- **Wrong Conditions**: Check if/else logic and boolean expressions
- **Loop Issues**: Analyze loop termination conditions
- **State Management**: Verify object state transitions

### Performance Issues
- **Memory Leaks**: Identify objects not being garbage collected
- **Infinite Loops**: Check for loops that never terminate
- **Inefficient Algorithms**: Look for O(n²) or worse complexity
- **Database Issues**: Analyze query performance and indexing

### Integration Issues
- **API Failures**: Check HTTP status codes and response formats
- **Configuration Problems**: Verify environment variables and settings
- **Dependency Conflicts**: Check version compatibility
- **Authentication Issues**: Verify credentials and permissions

## Debugging Tools and Techniques

### Code Inspection
- **Logging Strategy**: Add strategic console.log/print statements
- **Breakpoint Placement**: Where to set breakpoints for maximum insight
- **Variable Watches**: Which variables to monitor during execution
- **Call Stack Analysis**: How to read and interpret call stacks

### Testing Approaches
- **Isolation Testing**: Test components in isolation
- **Mock Data**: Use controlled data to reproduce issues
- **Edge Case Testing**: Test boundary conditions
- **Regression Testing**: Verify fixes don't break existing functionality

### Documentation and Communication
- **Bug Reports**: How to document findings for future reference
- **Team Communication**: What information to share with team members
- **Knowledge Sharing**: Document common patterns and solutions

## Advanced Debugging Strategies

### For Complex Issues
- **Binary Search**: Systematically eliminate code sections to isolate the problem
- **Rubber Duck Debugging**: Explain the code line by line to identify issues
- **Pair Debugging**: Collaborate with another developer for fresh perspective
- **Time-based Debugging**: For intermittent issues, look for timing-related causes

### For Performance Issues
- **Profiling**: Use appropriate profiling tools for the language/platform
- **Bottleneck Identification**: Find the slowest operations
- **Memory Analysis**: Track memory usage patterns
- **Concurrency Issues**: Look for race conditions and deadlocks
