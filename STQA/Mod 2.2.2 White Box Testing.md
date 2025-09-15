## Definition
White Box Testing, also known as **glass box**, **clear box**, or **structural testing**, is a software testing technique that examines the internal structure, logic, and workings of an application. Unlike black box testing, it involves knowledge and access to the source code. It is typically performed at various levels such as unit, integration, and system testing.

## Focus Areas of White Box Testing
- **Code Logic and Flow:** Verifying that the logic implemented in code modules such as conditions, loops, and cases operate correctly.
- **Code Coverage:** Ensuring testing covers the code thoroughly. Coverage includes:
    - **Statement Coverage:** Every line of code is executed at least once.
    - **Branch Coverage:** All decision branches (true/false) are covered.
    - **Path Coverage:** All logical code paths are exercised.
- **Data Flow and Variable Usage:** Verifying variables and data are initialized, defined, used, and deactivated properly.
- **Boundary Conditions:** Testing how code behaves under minimum, maximum, or edge cases of input.
- **Error and Exception Handling:** Ensuring graceful handling of errors and exceptions.
- **Unit Functions/Methods:** Testing individual units or methods for correct functionality.
- **Security Vulnerabilities:** Detecting issues such as hard-coded credentials or insecure validation.

## White Box Testing Process
1. **Preparation:**
    - Gather documentation: requirements, design documents, and source code.
    - Analyze risks to identify critical modules or areas.
    - Prepare test cases focused on internal structures—cover loops, decisions, data flow, etc.
2. **Designing Test Cases:**
    - Utilize control flow graphs and calculate cyclomatic complexity to identify independent paths.
    - Develop test cases to cover statement, branch, path, and condition coverage.
3. **Execution:**
    - Run tests, trace program execution.
    - Observe and record defects.
4. **Analysis and Debugging:**
    - Analyze failures and debug code.
    - Fix defects and re-run tests.
5. **Optimization:**
    - Refactor code to remove redundancies, improve clarity and performance.

## White Box Testing Techniques
- **Statement Coverage:** Tests designed to ensure every code statement is executed.
- **Branch (Decision) Coverage:** Ensures both true and false outcomes of each decision point are tested.
- **Condition Coverage:** Tests all logical conditions inside decisions.
- **Path Coverage:** All possible execution paths are tested; very thorough but often impractical for large programs.
- **Basis Path Testing:** Uses cyclomatic complexity to identify essential paths to test.
- **Loop Testing:** Focus on loops, including boundary iterations and infinite loops.
- **Data Flow Testing:** Focus on variable definition, usage, and abnormal states.
- **Mutation Testing:** Introducing small changes/mutants in code to check if test cases detect faults; measures test effectiveness.

## Advantages of White Box Testing
- Thorough verification of internal logic and code structure.
- Early detection of hidden defects and logical errors.
- Helps in code optimization by identifying redundant code.
- High coverage improves confidence in software correctness.
- Supports automation due to clear testable units.
- Efficient for unit and integration testing.

## Disadvantages of White Box Testing
- Requires detailed knowledge of programming and code.
- Time-consuming and costly for complex systems.
- May miss missing functionality since it focuses on existing code.
- Risk of tester bias due to familiarity with code.
- High maintenance overhead: test cases need updates with code changes.
- Not suitable for testing user interface or non-functional issues alone.