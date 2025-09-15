### Overview
Decision Table Testing is a systematic black-box technique for designing test cases, especially when dealing with complex logical decisions and multiple input combinations. A decision table represents conditions (inputs) and corresponding actions (outputs). It consists of: **Condition Stub** (list of conditions), **Condition Entry** (possible values like Yes/No or True/False), **Action Stub** (list of possible outputs), and **Action Entry** (marks indicating which actions are triggered for a condition combination). Each column in the table is a rule or test case.
### Process
1. Identify conditions and actions.
2. Define possible values for each condition.
3. Create all possible combinations of conditions.
4. Map actions to each combination (rules).
5. Simplify by removing irrelevant or impossible combinations.
6. Generate test cases from each rule.
### Types of Decision Tables
- **Limited Entry Table:** Conditions with only True/False values.
- **Extended Entry Table:** Conditions with multiple values.
- **Don’t Care Entries:** Marked with “I” when a condition does not affect the outcome.
### Advantages
- Models complex business logic precisely.
- Provides systematic coverage of input combinations.
- Helps in identifying missing conditions or rules.
- Easy to communicate test scenarios with stakeholders.
- Useful for both manual and automated test design.
### Disadvantages
- May cause combinatorial explosion when many conditions exist.
- Requires complete understanding of all input conditions and interactions.
- Designing tables for complex systems is time-consuming and error-prone.
- Risk of redundant or irrelevant test cases if not simplified.
- Interdependent conditions complicate accurate table construction.
- Does not guarantee structural code coverage.
- Limited to functional testing scope.

### Example
**Scenario:** Overtime pay calculation. Rules: If hours ≤ 48 → normal salary. If hours > 48 on working day → 1.25 × salary. If hours > 48 on holiday/Sunday → 2 × salary.

| Condition            | Rule 1 | Rule 2 | Rule 3 |
| -------------------- | ------ | ------ | ------ |
| Hours over 48 (Y/N)  | I      | N      | Y      |
| Holiday/Sunday (Y/N) | Y      | N      | N      |
| **Actions**          |        |        |        |
| Normal Salary        | X      | X      |        |
| Overtime 1.25×       |        |        | X      |
| Overtime 2×          |        |        |        |
**Derived Test Cases:** (1) Hours=48, Day=Monday → Normal Salary. (2) Hours=50, Day=Tuesday → 1.25× Salary. (3) Hours=52, Day=Sunday → 2× Salary.
