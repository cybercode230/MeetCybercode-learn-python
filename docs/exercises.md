
## 🧩 PART 1 — Complete Explanation of All Concepts

Here’s a **clear breakdown** of each concept you mentioned. Read it carefully and then use it to guide your practice challenges in Part 2.

---

### 🔹 1. Working with Primitive Data Types

Primitive data types are the basic building blocks in Python:

- `int` – integer numbers (e.g., `10`)
    
- `float` – decimal numbers (e.g., `3.14`)
    
- `bool` – logical True/False values
    
- `str` – text data
    
- `NoneType` – represents “nothing” or null
    

🧠 _Key Idea:_ Everything in Python is an **object**, even primitive types.

---

### 🔹 2. Multiple Assignment Statements

Python allows assigning multiple variables in one line:

```python
x, y, z = 1, 2, 3
x, y = y, x  # swap values
```

This improves readability and helps when unpacking sequences.

---

### 🔹 3. Converting Types in Python

Use built-in functions like:

- `int("5")`, `float("3.14")`
    
- `str(100)`, `list("hello")`
    
- `bool(0)` → `False`
    

🧠 Conversion is often used when reading input (which is always a string).

---

### 🔹 4. Creating, Modifying, Sorting, and Slicing Lists

Lists are **ordered, mutable** collections.

```python
fruits = ["apple", "banana", "cherry"]
fruits.append("orange")
fruits[0] = "mango"
fruits.sort()
fruits.reverse()
print(fruits[1:3])  # slicing
```

---

### 🔹 5. Operators and Precedence

Operators perform actions:

- Arithmetic: `+ - * / // % **`
    
- Comparison: `> < == !=`
    
- Logical: `and or not`
    
- Assignment: `+= -= *=`
    

🧠 Precedence defines the **order** of evaluation:  
`*` and `/` are done before `+` and `-`.

---

### 🔹 6. Conditional Statements

```python
if x > 0:
    print("Positive")
elif x < 0:
    print("Negative")
else:
    print("Zero")
```

Compound conditions:

```python
if age > 18 and country == "Rwanda":
    print("Allowed")
```

---

### 🔹 7. Loops (For, While, Nested)

```python
for i in range(5):
    print(i)

while x < 10:
    x += 1

for i in range(3):
    for j in range(2):
        print(i, j)
```

🧠 _Nested loops_ are often used for matrix operations or pattern generation.

---

### 🔹 8. Reading and Copying Files

```python
with open("data.txt", "r") as f:
    content = f.read()

with open("copy.txt", "w") as c:
    c.write(content)
```

---

### 🔹 9. Merging Mails (File & String Templates)

Using templates:

```python
template = "Hello {name}, welcome to {course}"
message = template.format(name="Alice", course="Python 101")
```

---

### 🔹 10. Reading Console Inputs & Command Line Args

```python
name = input("Enter your name: ")
```

Command-line:

```python
import sys
print(sys.argv)  # list of arguments
```

---

### 🔹 11. Functions & Arguments

```python
def greet(name="Guest"):
    print(f"Hello, {name}")

greet("Cybercode")
```

Keyword and positional:

```python
def add(a, b): return a + b
print(add(b=3, a=2))
```

---

### 🔹 12. Handling Exceptions

```python
try:
    x = int(input("Enter number: "))
except ValueError:
    print("Invalid number")
finally:
    print("Done")
```

---

### 🔹 13. Math, Random, Datetime, and File Metadata

```python
import math, random, os, datetime

print(math.sqrt(25))
print(random.randint(1, 10))
print(datetime.datetime.now())
print(os.getcwd())  # working directory
print(os.stat("file.txt"))  # metadata
```

---

## ⚔️ PART 2 — 3-DAY CHALLENGE SET (Progressively Hard)

You’ll get **challenging exercises** that push your logic, data manipulation, and problem-solving.  
Try to solve them **without AI** first.  
Each challenge connects multiple concepts.

---

### **📅 DAY 1 — Core Python Logic & Data**

Focus: Primitive types, operators, lists, conditions.

1. **Temperature Converter**
    
    - Ask for temperature in Celsius and convert to Fahrenheit.
        
    - Display both formatted to 2 decimal places.
        
2. **Even-Odd Counter**
    
    - Input a list of numbers from the user.
        
    - Count how many are even and how many are odd.
        
3. **List Transformer**
    
    - Create a list of 10 random integers between 1–100.
        
    - Sort it ascending, reverse it, and print only elements at even indexes.
        
4. **Math Operator Simulator**
    
    - Ask user for two numbers and an operator (+, -, *, /).
        
    - Compute manually using `if` statements — no `eval()` allowed.
        

---

### **📅 DAY 2 — Files, Loops, and Functions**

Focus: loops, file I/O, string formatting, functions.

5. **Student Score Report**
    
    - Read student names and scores from a file.
        
    - Compute average, highest, lowest.
        
    - Write a new file `report.txt` with formatted results.
        
6. **Mail Merge Automation**
    
    - Given a file `names.txt` with names and a message template:
        
        ```
        Dear [name], you are selected for the DTP program.
        ```
        
    - Generate personalized letters for each student.
        
7. **Guessing Game**
    
    - Generate a random number between 1–50.
        
    - Let the user guess until they win, tracking attempts.
        
    - Give hints ("too high", "too low").
        

---

### **📅 DAY 3 — Advanced Concepts & Error Handling**

Focus: exceptions, command-line args, nested loops, date/time.

8. **Command-Line Calculator**
    
    - Run program as:
        
        ```
        python calc.py 10 + 20
        ```
        
    - Use `sys.argv` to parse and compute.
        
9. **File Copier with Error Handling**
    
    - Copy file content to another file.
        
    - Handle cases: file not found, permission denied, etc.
        
10. **Pattern Generator**
    

- Using nested loops, print:
    
    ```
    *
    * *
    * * *
    * * * *
    ```
    

11. **Daily Log Timestamp**
    

- Each time program runs, append a timestamp entry to a file:
    
    ```
    Log started at: 2025-11-10 10:00
    ```
    

12. **Random Password Generator**
    

- Ask length, use `random` and `string` to create strong passwords.
    
- Include uppercase, lowercase, digits, symbols.
    

---

### 🧠 BONUS HARD CHALLENGES (Optional)

For pushing yourself further.

13. **File Analyzer**
    

- Read a `.txt` file, count total words, lines, characters.
    
- Display top 5 most frequent words.
    

14. **Mini Student Database**
    

- Store students in a list of dictionaries.
    
- Allow user to add, delete, update, and display records via menu.
    

15. **To-Do CLI App**
    

- Manage tasks using command-line arguments:
    
    ```
    python todo.py add "Buy milk"
    python todo.py list
    python todo.py done 1
    ```
