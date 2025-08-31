# Palindromic Numbers Challenge  

## Description  
A **palindrome** is a word or expression that can be read from left to right or right to left while maintaining the same meaning.  
For example, the word *“reviver”* is a palindrome.  

In this challenge, the goal is to print all **palindromic numbers** between two given numbers.  
Just like words, palindromic numbers remain the same when read backwards.  

- The initial and final numbers must be included in the results if they are also palindromes.  

### Examples  

**Example 1**  
- Input: initial = 1, final = 20  
- Output: `1, 2, 3, 4, 5, 6, 7, 8, 9, 11`  

**Example 2**  
- Input: initial = 3000, final = 3010  
- Output: `3003`  

**Example 3**  
- Input: initial = 101, final = 121  
- Output: `101, 111, 121`  

## Rules & Constraints  

- Only **positive integers** can be used as boundaries.  
- **Single-digit numbers** are palindromes by definition.  
- Maximum number: `(1 << 64) - 1` (the maximum 64-bit unsigned integer).  

### Bonus Challenge  
If the problem seems too easy, implement a **custom data type** to handle numbers with arbitrary precision (limit: up to 100,000 digits per number).  
> ⚠️ Note: The use of external arbitrary-precision math libraries will **not** be considered a valid solution.  

## Difficulty  
- **Easy**  

## Scoring  
- This challenge is worth **20 points**.  
