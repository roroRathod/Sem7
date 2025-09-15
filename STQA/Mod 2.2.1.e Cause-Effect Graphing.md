Cause-Effect Graphing is a testing technique used for designing test cases that address combinations of input conditions, which traditional methods like boundary value analysis and equivalence partitioning do not handle comprehensively. It uses cause-effect graphs combined with decision tables.

## Main Process of Cause-Effect Graphing

- **Divide the specification** into manageable parts.
    
- **Identify causes and effects**, where causes represent distinct input conditions or their equivalence classes, and effects represent output conditions.
    
- **Build a Boolean graph** (cause-effect graph) linking causes to effects with logical operators and constraints.
    
- **Convert the graph into a decision table**, mapping all valid combinations of causes to corresponding effects.
    
- **Derive test cases** from the decision table columns.
    

## Logical Operators and Constraints Used

- Identity: output = input
    
- NOT: output is the negation of input
    
- OR: output is true if any inputs are true
    
- AND: output is true only if all inputs are true
    
- Exclusive: inputs cannot be true together
    
- Inclusive: At least one input must be true
    
- Require: One input requires another to be true
    
- Mask: One input masks another (forces it false)
    

## Example (from the book)

- Problem: Determine the nature of roots of a quadratic equation with inputs a, b, c.
    
- Causes: a ≠ 0, b = 0, c = 0, Discriminant D > 0, D < 0, D = 0, a = b = c, a = c = b/2.
    
- Effects: Not a quadratic, Real roots, Imaginary roots, Equal roots.
    
- The cause-effect graph represents these with logical relations, which are then converted to decision tables for test case design.
    

## Handling Don't-Care / Immaterial Conditions

- Some conditions in rules may be immaterial (don't-care), meaning their value does not affect the outcome.
    
- Expanding immaterial cases by testing all values (true and false) can reveal hidden defects.
    
- This is done by elaborating rules in the decision table.