# Python Engineering Standards at [CirrusLabs](https://www.cirruslabs.io/)

## Table of Contents
1. [Introduction](#introduction)
2. [Coding Standards](#coding-standards)
   - [Python](#python)

## Introduction
This document outlines the python engineering standards followed at [CirrusLabs](https://www.cirruslabs.io/) to ensure high-quality code, efficient development processes, and a collaborative working environment.

## Coding Standards
- [ ] Use [programming language/tool specific standards](#) for consistent code formatting and style.
- [ ] Follow best practices for error handling, variable naming, and function length.

### Python
1. **Code Formatting**:
   - Use 4 spaces for indentation.
   - Use snake_case for variable and function names.
   - Use CAPITAL_SNAKE_CASE for constants.
   - Limit lines to 79 characters.

2. **Naming Conventions**:
   - Use descriptive names for variables, functions, and classes.
   - Avoid using single-letter variable names except for iterators (e.g., `i`, `j`, `k`).

3. **Comments**:
   - Use comments to explain complex algorithms or to provide context where necessary.
   - Use docstrings to document functions, classes, and modules.

4. **Error Handling**:
   - Use try-except blocks for handling exceptions.
   - Catch specific exceptions rather than using a generic `except:` clause.
   - Always include a meaningful message when raising exceptions.

5. **Best Practices**:
   - Use list comprehensions and generator expressions instead of loops where possible.
   - Use context managers (`with` statement) for resource management.
   - Follow the PEP8 style guide for Python code.
