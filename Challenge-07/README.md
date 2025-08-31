# TAC Challenge  

## Description  
In Unix (and Linux), the `cat` command prints the contents of a text file to standard output.  
A similar, but less known command is `tac`, which displays the file **in reverse order**, printing the last line first and the first line last.  

## Problem Statement  
Implement the **tac** command in your preferred programming language and libraries.  

### Requirements  

1. The program must:  
   - Read a file from disk specified on the command line.  
   - Print the file **line by line**, starting from the last line and ending with the first.  

   **Example:**  

   ```bash
   $ cat file.txt
   This is the first line
   This is the second line
   This is the third line
   This is the last line

   $ tac file.txt
   This is the last line
   This is the third line
   This is the second line
   This is the first line
   ```

2. The program must handle files of **any size**, while respecting a **512MB memory limit**.  
   - Reading the entire file into memory at once is **not allowed**.  

## Verification  

If running on Linux, you can test memory usage with:  

```bash
ulimit -v 524288
```

This restricts the process to **512MB** of memory. Your program must work correctly under these conditions with files of any size.  

### Test File  

1. Download the test file (≈308 MB).  
2. Decompress it locally:  

```bash
gzip -d 1GB.txt.gz
```

3. Run your program using the decompressed file as input and check the **md5sum**:  

```bash
$ your_program 1GB.txt | md5sum
2b4fd25f11d75c285ec69ecac420bd07
```

⚠️ The computed `md5sum` must **match exactly** the value above.  

## Difficulty  
- **Easy / Medium**  

## Scoring  
- This challenge is worth **50 points**.  
