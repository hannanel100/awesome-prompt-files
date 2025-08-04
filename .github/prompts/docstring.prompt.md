---
mode: agent
description: Generate comprehensive docstrings and documentation for functions, classes, and modules
---

Your task is to generate comprehensive, well-structured documentation for the selected code. Create docstrings that follow language-specific conventions and provide clear, useful information for developers.

## Documentation Standards

### Content Requirements
- **Purpose**: Clear, concise description of what the code does
- **Parameters**: Document all parameters with types and descriptions
- **Return Values**: Describe return types and possible values
- **Exceptions**: List exceptions that may be raised and when
- **Examples**: Provide usage examples for complex functions
- **Side Effects**: Note any side effects or state changes

### Documentation Style
Follow the appropriate style guide for the language:
- **Python**: Google, NumPy, or Sphinx style
- **JavaScript/TypeScript**: JSDoc format
- **Java/C#**: JavaDoc/XML documentation comments
- **Go**: Standard Go documentation format
- **Rust**: Rust documentation comments

## Language-Specific Formats

### Python (Google Style)
```python
def function_name(param1: type, param2: type) -> return_type:
    """Brief description of the function.
    
    Longer description if needed. Explain the purpose, behavior,
    and any important implementation details.
    
    Args:
        param1 (type): Description of param1.
        param2 (type): Description of param2.
    
    Returns:
        return_type: Description of return value.
    
    Raises:
        ExceptionType: Description of when this exception is raised.
    
    Example:
        >>> result = function_name("value1", 42)
        >>> print(result)
        expected_output
    """
```

### JavaScript/TypeScript (JSDoc)
```javascript
/**
 * Brief description of the function.
 * 
 * Longer description if needed. Explain the purpose, behavior,
 * and any important implementation details.
 * 
 * @param {type} param1 - Description of param1
 * @param {type} param2 - Description of param2
 * @returns {return_type} Description of return value
 * @throws {Error} Description of when this error is thrown
 * 
 * @example
 * const result = functionName("value1", 42);
 * console.log(result); // expected_output
 */
```

### Java (JavaDoc)
```java
/**
 * Brief description of the method.
 * 
 * Longer description if needed. Explain the purpose, behavior,
 * and any important implementation details.
 * 
 * @param param1 Description of param1
 * @param param2 Description of param2
 * @return Description of return value
 * @throws ExceptionType Description of when this exception is thrown
 * 
 * @since version
 * @author author_name
 */
```

## Documentation Guidelines

### Writing Quality
- **Be Concise**: Clear and to the point, avoid unnecessary verbosity
- **Be Specific**: Use precise language, avoid vague terms
- **Be Consistent**: Follow the same style throughout the codebase
- **Be Helpful**: Focus on what developers need to know to use the code

### Technical Details
- **Parameter Types**: Always specify parameter types and constraints
- **Return Values**: Describe not just the type but the meaning
- **Edge Cases**: Document behavior for edge cases and special conditions
- **Dependencies**: Note any important dependencies or requirements

### Examples and Usage
- **Realistic Examples**: Use examples that reflect actual usage patterns
- **Multiple Scenarios**: Show different ways to use the function if applicable
- **Expected Output**: Include expected results for examples
- **Error Examples**: Show how to handle errors when relevant

## Special Considerations

### Classes and Methods
- Document the class purpose and main responsibilities
- Explain the relationship between methods
- Document important properties and their meanings
- Include information about object lifecycle if relevant

### Complex Algorithms
- Provide high-level explanation of the algorithm
- Document time and space complexity when relevant
- Explain any mathematical concepts or formulas used
- Reference papers or resources for complex algorithms

### Configuration and Options
- Document all configuration options and their effects
- Provide default values and valid ranges
- Explain the impact of different settings
- Include configuration examples

## Analysis Process

1. **Analyze the code** to understand:
   - Function/method purpose and behavior
   - Parameter types, constraints, and usage
   - Return values and their meanings
   - Possible exceptions or error conditions
   - Dependencies and side effects

2. **Determine complexity level**:
   - Simple functions: Basic docstring with parameters and return
   - Complex functions: Detailed explanation with examples
   - Public APIs: Comprehensive documentation with multiple examples
   - Internal utilities: Focus on implementation details for maintainers

3. **Generate appropriate documentation** that matches the code's:
   - Complexity level
   - Intended audience (public API vs internal)
   - Language conventions
   - Project documentation standards
