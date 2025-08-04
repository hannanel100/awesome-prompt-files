---
mode: agent
description: Generate comprehensive unit tests for selected code with edge cases and proper test structure
---

Your task is to generate comprehensive unit tests for the selected function, class, or module. Create tests that cover all scenarios including edge cases, error conditions, and typical usage patterns.

## Test Generation Requirements

### Test Coverage
- **Happy Path**: Test normal, expected behavior with valid inputs
- **Edge Cases**: Test boundary conditions, empty inputs, null/undefined values
- **Error Cases**: Test invalid inputs, exceptions, and error handling
- **State Changes**: For classes, test how methods affect object state
- **Integration Points**: Test interactions with dependencies (using mocks/stubs)

### Test Structure
- Use descriptive test names that explain what is being tested
- Follow the Arrange-Act-Assert (AAA) pattern
- Group related tests using describe/context blocks
- Include setup and teardown when needed

### Test Quality
- Each test should focus on one specific behavior
- Tests should be independent and able to run in any order
- Use appropriate assertions that provide clear failure messages
- Mock external dependencies appropriately

## Analysis Process

1. **Analyze the code structure** to understand:
   - Function/method signatures and parameters
   - Return types and possible return values
   - Dependencies and external calls
   - Side effects and state changes
   - Error conditions and exceptions

2. **Identify test scenarios** including:
   - All code paths and branches
   - Boundary conditions for numeric inputs
   - Empty, null, or invalid inputs
   - Different object states (for classes)
   - Interaction with mocked dependencies

## Output Format

Generate tests using the project's existing testing framework (detect from codebase) or use these common patterns:

```javascript
// For JavaScript/TypeScript (Jest/Vitest)
describe('[Function/Class Name]', () => {
  describe('[specific behavior]', () => {
    it('should [expected behavior] when [condition]', () => {
      // Arrange
      // Act  
      // Assert
    });
  });
});
```

```python
# For Python (pytest/unittest)
class Test[ClassName]:
    def test_[behavior]_when_[condition]_should_[expected_result](self):
        # Arrange
        # Act
        # Assert
```

## Test Generation Guidelines

### Test Data
- Create realistic test data that represents actual usage
- Use both typical and extreme values
- Include invalid data to test error handling
- Consider using test data factories for complex objects

### Mocking Strategy
- Mock external dependencies (APIs, databases, file systems)
- Use dependency injection where possible
- Mock time-dependent functions for consistent testing
- Preserve the interface contracts when mocking

### Assertions
- Use specific assertions rather than generic ones
- Test both the result and any side effects
- Verify mock interactions when testing integration points
- Include assertions for error messages and types

### Additional Considerations
- Add performance tests for critical functions if relevant
- Include integration tests for complex workflows
- Consider property-based testing for functions with complex input spaces
- Add regression tests for previously found bugs
