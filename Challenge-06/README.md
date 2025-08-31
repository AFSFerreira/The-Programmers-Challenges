# Anagrams Challenge  

## Description  
An **anagram** is a word or phrase formed by rearranging all the letters of another word or phrase (with no letters missing or left over).  

### Examples  
- The word **“barco”** is an anagram of **“cobra”** (all letters used).  
- The word **“mar”** is **not** an anagram of **“roma”** (the letter “o” was not used).  
- The word **“sal”** is **not** an anagram of **“mal”** (the letter “s” is missing).  

## Problem Statement  
Write a program, in the programming language and libraries of your choice, that:  

1. **Reads an expression** (a word or phrase) from the command line.  
   - Only letters **A–Z** should be considered.  
   - Ignore spaces.  
   - Convert all lowercase letters to **uppercase**.  
   - If invalid characters are found (numbers, punctuation, accented letters, etc.), return an error and abort execution.  

2. **Reads a list of valid words** from the file `words.txt`.  
   - The file is formatted with one word per line.  
   - The list contains words in English. *(Note: no clean Portuguese word list was found.)*  

3. **Generates and prints all possible anagram combinations**, without repetition.  
   - Each anagram must consist only of valid words from the dictionary file.  
   - The output must contain multiple lines (one anagram per line).  
   - Inside each line, words must be printed in **alphabetical order**.  

4. **Performance requirements**:  
   - The program must compute and print all possible anagrams of an expression with up to **16 characters** in under **60 seconds**.  

### Examples  

**Expression as a word**:  

```bash
$ ./anagram "vermelho"
ELM HO REV
ELM OH REV
OHM REVEL
LEVER OHM
ELM HOVER
HOLM VEER
HELM OVER
HELM ROVE
```

**Expression as a phrase** (ignore spaces, convert to uppercase):  

```bash
$ ./anagram "oi gente"
GO I TEEN
GENE I TO
GET I ONE
EON GET I
ENG I TOE
GEE I TON
GEE I NOT
EGO I NET
EGO I TEN
GEE IT NO
GEE IT ON
GO IN TEE
GEE IN TO
GENIE TO
GONE TIE
GEE OINT
GEE INTO
GEE TONI
GINO TEE
GENE ITO
EGO TINE
```

## Tips  

- For simplicity, only **alphabetical characters (A–Z)** should be considered.  
- This is a classic case for a **recursive algorithm**.  
- Brute-force approaches will not work efficiently.  
- This challenge is considered **medium/difficult**. Discuss doubts with admins or other participants in the *OsProgramadores* Telegram group.  

⚠️ **Important**: When submitting your PR with the solution, **do not include the dictionary file** (`words.txt`). Only submit your solution files.  

## Difficulty  
- **Medium / Hard**  

## Scoring  
- This challenge is worth **70 points**.  
