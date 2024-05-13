# Unit Testing - Standard Procedure

Unit testing is a fundamental practice in software development aimed at verifying that individual units or components of a software system work as expected. Here's a standard procedure for unit testing:

1. **Identify Units:** Determine the smallest testable parts of your codebase, typically functions, methods, or classes.

2. **Write Test Cases:** For each unit, create a set of test cases that cover various scenarios, including normal inputs, boundary conditions, and error cases. Test cases should be independent, isolated, and repeatable.

3. **Choose a Testing Framework:** Select a unit testing framework compatible with your programming language or technology stack. Examples include JUnit for Java, NUnit for .NET, pytest for Python, and Jasmine, Mocha, and Jest for JavaScript.

4. **Write Test Code:** Implement test methods or functions for each test case using the chosen testing framework. Each test method should execute the unit under test with specific inputs and verify the expected behavior using assertions.

5. **Arrange-Act-Assert (AAA):** Structure each test method into three phases:
   - **Arrange:** Set up the preconditions and inputs for the test.
   - **Act:** Invoke the unit under test with the arranged inputs.
   - **Assert:** Verify that the actual output matches the expected behavior.

6. **Run Tests:** Execute the test suite using the testing framework's runner or command-line interface. Ensure that all tests pass successfully.

7. **Analyze Results:** Review the test results to identify any failed tests or unexpected behavior. Investigate and debug failures to understand the root cause.

8. **Refactor and Repeat:** Refactor your code as needed to improve testability and maintainability. Update test cases to accommodate changes in requirements or code implementation.

9. **Automate Testing:** Integrate unit tests into your continuous integration (CI) or build pipeline to automate test execution on code changes. This ensures that tests are run consistently and frequently.

10. **Coverage Analysis:** Use code coverage tools to measure the percentage of code exercised by your unit tests. Aim for high code coverage to ensure thorough testing of your codebase. Examples include Istanbul, Jest, SonarQube, etc.

11. **Review and Documentation:** Review unit tests with team members to ensure clarity and effectiveness. Document test cases, especially for complex or critical components, to facilitate understanding and future maintenance.

12. **Regression Testing:** Periodically rerun unit tests, especially after code changes or updates, to catch regressions and ensure that existing functionality remains intact.

Let's go through a simple example of writing unit tests for a JavaScript function using the Jest testing framework. 
In this example, we'll create a function that adds two numbers together and then write unit tests to verify its behavior.

### Example: Writing Unit Tests with Jest

#### `mathFunctions.js`

// Function to add two numbers
export function add(a, b) {
    return a + b;
}

Now, let's write the corresponding unit tests using Jest. Create a file named mathFunctions.test.js in the same directory: 

#### `mathFunctions.test.js`

import { add } from './mathFunctions';

describe('add function', () => {
    test('adds two numbers correctly', () => {
        expect(add(1, 2)).toBe(3);
        expect(add(-1, 1)).toBe(0);
        expect(add(0, 0)).toBe(0);
    });
});

### Explanation of test file

In the test file:

1. **Importing the add function from mathFunctions.js:**
   
   This is typically how you bring in the function you want to test into your test file.

2. **Using Jest's describe function to group related test cases:**
   
   `describe` is used to group related test cases together, providing better organization and readability to your test suite.

3. **Each test function defines an individual test case:**
   
   Each test function typically focuses on testing a specific behavior or scenario of the unit under test.

4. **Calling the add function with specific inputs and using Jest's expect function to assert the result:**
   
   This is the essence of a test case - you provide inputs to the function you're testing and then use assertions to verify that the function behaves as expected.

5. **Installing Jest via npm:**
   
   To use Jest for testing, you need to install it as a development dependency in your project. The command you provided is correct (`npm install --save-dev jest`).

6. **Running tests with the default React script:**
   
   The command to run tests with the default React script is `npm test` (or `yarn test` if you're using Yarn). This command will execute the test runner configured in your `package.json` file, which is typically Jest in React projects created with Create React App.
