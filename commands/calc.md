---
description: Perform a basic arithmetic calculation
argument-hint: <expression>
allowed-tools: [Bash]
---

# Calculator Command

Perform a basic arithmetic calculation.

## Arguments

The user provided the following expression: $ARGUMENTS

## Instructions

1. Parse the mathematical expression from the arguments
2. Use Bash to evaluate the expression:
   ```bash
   echo "scale=4; $ARGUMENTS" | bc -l
   ```
3. Display the result to the user in a clear format:
   - Show the original expression
   - Show the result
