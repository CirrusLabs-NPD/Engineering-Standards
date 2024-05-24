# Java Engineering Standards at [CirrusLabs](https://www.cirruslabs.io/)

1. **Code Formatting**:

   - Use a consistent indentation style (e.g., 4 spaces).
   - Use braces for all control structures, even if they are optional.
   - Limit lines to 80-120 characters.

2. **Naming Conventions**:

   - Use meaningful and descriptive names for variables, methods, and classes.
   - Use camelCase for variables and methods, and UpperCamelCase for class names.

3. **Comments**:

   - Use comments to explain complex code or to provide context where necessary.
   - Follow Javadoc conventions for documenting classes, methods, and parameters.

4. **Error Handling**:

   - Use try-catch blocks for handling exceptions.
   - Catch specific exceptions rather than general ones where possible.
   - Always include a meaningful message when throwing exceptions.

5. **Concurrency**:

   - Use synchronization or concurrent data structures for thread safety.
   - Avoid using `synchronized` on large blocks of code; use it only where necessary.

6. **Best Practices**:
   - Use interfaces and abstract classes to define contracts.
   - Minimize the use of static methods and variables.
   - Use enums for representing a fixed set of constants.
