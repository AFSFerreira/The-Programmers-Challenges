# Primes in Pi  

## Introduction  
The number **pi (π)** is one of the most famous and easily recognizable mathematical constants.  
Originally defined as the ratio of a circle’s circumference to its diameter, π is an **irrational number**, meaning its decimal representation is infinite and non-repeating.  

## Challenge Description  
This challenge consists of finding the **longest sequence of prime numbers (between 2 and 9973)** within the first **1 million decimal digits of π**.  

### Details  
- Locate the **longest sequence** (in digits) of prime numbers in the provided file containing the first 1 million decimal digits of π.  
- If multiple sequences of the same length are found, use the one **closest to the decimal point**.  
- Only consider **prime numbers between 2 and 9973** (i.e., primes with 1 to 4 digits).  

---

## Example  

Consider π with 20 decimal places:  

```
3.14159265358979323846
```  

The longest sequence of primes would be:  

```
41 59 2 653 5 89 7 9323
```  

Which results in the concatenated sequence:  

```
4159265358979323
```  

---

## Output Format  
The program must print **a single line** containing the longest sequence found, without spaces.  

**Example:**  
```
4159265358979323
```  

---

## Difficulty  
- **Medium**  

## Scoring  
- This challenge is worth **60 points**.  
