# Big Base Challenge  

## Description  
Write a program that reads a text file where each line contains **three values**:  

```
input_base output_base input_number
```  

The program must convert the given number (in `input_base`) into its equivalent representation in `output_base`.  

### Example Input  

```
10 16 1500
36 10 GOODBYE
36 16 HELLOWORLD
10 2 32452867
2 10 1234
```  

### Example Output  

```
5DC
36320638406
647B8839EB1B1
1111011110011000100000011
???
```  

## Rules & Considerations  

1. **Supported bases:**  
   - Conversions must work for any base between **2 and 62** (inclusive).  

2. **Errors:**  
   - If any error is detected, print `???`.  
   - Errors include:  
     - Invalid base (must be between 2 and 62).  
     - Negative numbers.  
     - Numbers too large (see limit below).  
     - Invalid digits for the given base.  

3. **Character set for bases > 10:**  
   ```
   0123456789ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz
   ```
   - Here, `z = 61`.  
   - For hexadecimal (base 16), letters must be **uppercase**.  

4. **Large numbers:**  
   - The program must handle very large inputs.  
   - The upper limit is the value of:  
     ```
     zzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzz (in base 62)
     ```  

5. **Implementation restriction:**  
   - You must implement the conversion algorithm yourself.  
   - Do **not** use built-in conversion routines provided by your programming language.  

## Difficulty  
- **Medium**  

## Scoring  
- This challenge is worth **30 points**.  
