# Simple Fractions Challenge  

## Description  
Write a program that reads a text file containing a list of fractions in ASCII format (**one per line**) and outputs the **simplified version** of each fraction.  

### Rules  
- Simple numbers are assumed to have denominator **1** (just print the number).  
- Integer divisions such as `81/9` must output the integer `9`.  
- If an error occurs in the input (e.g., division by zero), print `ERR` in uppercase.  

### Example  

**Input:**  
```
14/3
3/8
4/8
4/3
5
10/0
48/12
```

**Output:**  
```
4 2/3
3/8
1/2
1 1/3
5
ERR
4
```

## Validation  

1. Download the test file.  
2. Decompress it locally:  

```bash
gzip -d frac.txt.gz
```

3. Run your program using the file as input.  
4. Once you are satisfied with the results, go to the **challenge validation page**.  
   - Select the challenge number.  
   - Enter your GitHub username.  
   - Paste your solution.  
5. If everything is correct, the validation page will issue a **token**.  
6. Create a text file called `.valid` in your solution directory containing the token on the first line.  
7. Add this file to your commit and submit the PR.  

### PR Verification  

- After submitting the PR, check the PR page to ensure all tests pass.  
- If a test fails, click on **Details** in the test results page for more information.  

⚠️ The use of external libraries that simplify fractions (e.g., Python’s `fractions` module or `fraction.js`) is **not allowed**.  

## Difficulty  
- **Easy**  

## Scoring  
- This challenge is worth **30 points**.  
