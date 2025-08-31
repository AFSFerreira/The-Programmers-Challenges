# Numerical Expressions Challenge  

## Introduction  
**Numerical expressions** are sequences of two or more operations that must be evaluated in a specific order.  
To ensure consistent results, we follow well-defined rules of precedence and grouping.  

Examples:  
- `12 + 3 * 5 = 27`  
- `2 * (5 - 1) = 8`  
- `2^2 + 8 / 2 = 8`  
- `2^(3 - 1) = 4`  

---

## Challenge Description  
This challenge consists of:  

1. Reading a file of expressions, where each line contains a single mathematical expression.  
2. Printing the numeric result of each expression.  
3. Handling errors gracefully:  
   - If a **division by zero** occurs, print:  
     ```
     ERR DIVBYZERO
     ```  
   - If a **syntax error** occurs in the expression, print:  
     ```
     ERR SYNTAX
     ```  
4. No external libraries for expression parsing or evaluation may be used.  

---

## Example  

**Input file:**  
```
1 + 3
2 - 3 * 2
2 ^ 3 / 4
0 * 5 * (4 + 1)
5 + 5 / 0
5 + + 1
5 + ( 465 + 1
```

**Expected Output:**  
```
4
-4
2
0
ERR DIVBYZERO
ERR SYNTAX
ERR SYNTAX
```

---

## Notes  
- The program must respect **operator precedence** and parentheses.  
- Exponentiation (`^`) is included in the operations.  
- The implementation must be done without relying on third-party libraries.  

---

## Difficulty  
- **Easy / Medium**  

## Scoring  
- This challenge is worth **40 points**.  
