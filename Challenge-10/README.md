# Turing Machine Challenge  

## Introduction  
A **Turing Machine** is a mathematical model of computation that defines an abstract machine.  
This machine manipulates symbols on a tape according to a set of simple rules.  

Despite its simplicity, a Turing Machine can simulate **any computational algorithm**.  

## How It Works  

- A Turing Machine reads data from an **infinite tape**, one character (symbol) at a time.  
- The machine is always in a given **state** (the initial state is `"0"`).  
- Rules define actions to be executed based on a `(state, symbol)` pair.  

Possible actions include:  
- Writing a new symbol at the current tape position.  
- Moving the tape head **left** or **right**.  
- Changing the machine’s current state.  

The process continues until either:  
1. No matching rule exists for the current `(state, symbol)` pair → **abort program**.  
2. A rule transitions into a state starting with `halt` → **terminate program**.  

The tape is infinite in both directions:  
- Moving beyond the end appends a blank space.  
- Moving left before the first symbol prepends a blank space.  

### Example  

**Input tape:**  
```
A/B/C/D@
```

**Rules:**  
```
0 @ . * halt
0 * * r 0
0 / x r y
y @ . * halt
y * * r y
y / y r 0
```

**Output:**  
```
AxByCxD.
```

---

## Input Format  

### Data File  
The **data file** contains two comma-separated fields per line:  
```
rules_file,input_data
```  

**Example:**  
```
prime.tur,101
prime.tur,102
pali.tur,1001001
```

This means:  
- Run `prime.tur` with input `101`.  
- Then run `prime.tur` with input `102`.  
- Then run `pali.tur` with input `1001001`.  

### Rules File  
The **rules file** defines the set of rules to be applied.  
Each line has 5 space-separated fields:  

```
current_state current_symbol new_symbol direction new_state
```

#### Field Definitions  

- **current_state**: Must match the current machine state.  
  - `*` → match any state.  

- **current_symbol**: Must match the current tape symbol.  
  - `*` → match any symbol.  
  - `_` → matches a blank space.  

- **new_symbol**: Symbol to write in place of the current symbol.  
  - `_` → write a blank space.  
  - `*` → do not replace the current symbol.  

- **direction**: Movement of the tape head.  
  - `l` → move left.  
  - `r` → move right.  
  - `*` → do not move.  
  - Any other value → error.  

- **new_state**: The new machine state.  
  - Any alphanumeric string is valid.  
  - Any state beginning with `halt` causes termination.  

#### Rule Matching Priority  
- More specific rules override generic ones (`*`).  
- If multiple generic rules apply, the **first one** should be used.  

#### Comments  
- Empty lines or lines starting with `;` are ignored.  
- Inline comments (after `;`) are also ignored.  

**Example Rules:**  
```
0 @ . * halt
0 * * r 0
0 / x r y
y @ . * halt
y * * r y
y / y r 0
```

---

## Output Format  

The program must print **one line per execution**, containing three comma-separated fields:  

```
rules_file,input_data,output_data
```  

**Example:**  
```
foo.tur,100,001
foo.tur,101,101
bar.tur,1001,:)
meh.tur,9999,ERR
```

- If an error occurs during execution, print only `ERR` in the output field.  

---

## Difficulty  
- **Hard**  

## Scoring  
- This challenge is worth **60 points**.  
