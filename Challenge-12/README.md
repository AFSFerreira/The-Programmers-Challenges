# Powers of 2 Challenge  

## Introduction  
Base 2 is one of the most commonly used number systems in computing.  
Numbers in base 2 can be represented as powers of 2:  

```
2^0 = 1
2^1 = 2
2^2 = 4
2^3 = 8
...
```

## Challenge Description  
This challenge consists of:  

1. Reading a file containing numbers (one per line).  
2. For each number:  
   - If the number is a **power of 2**, print the number followed by `true` and the exponent such that `2^exponent = number`.  
   - If the number is **not** a power of 2, print the number followed by `false`.  

---

## Example  

**Input file:**  
```
1
140
128
137
65535
65536
17179869184
```

**Output:**  
```
1 true 0
140 false
128 true 7
137 false
65535 false
65536 true 16
17179869184 true 34
```

---

## Difficulty  
- **Easy**  

## Scoring  
- This challenge is worth **30 points**.  
