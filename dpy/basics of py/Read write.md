
## Read: 
To read the contents of a file:
```
p = "a_test.txt"
with open(p, "r") as f:
    print(f.readlines())

```

output:
```
PS C:\Users\hp\OneDrive\Desktop\dsa_py> python .\pyBasics.py
['hello there\n', '42\n', '35\n', '76\n', 'this,is,the,end\n']
```

another way to read files:
```
p = "a_test.txt"
with open(p, "r") as f:
    print(f.read())

```
output:
```
PS C:\Users\hp\OneDrive\Desktop\dsa_py> python .\pyBasics.py
hello there
42
35
76
this,is,the,end
```

While both `f.read()` and `f.readlines()` are used to read data from a file in Python, the main difference is **how they format and return that data**.

Here is the quick breakdown of the difference:

### The Quick Summary

- **`f.read()`** treats the entire file as **one giant string**.
    
- **`f.readlines()`** splits the file by line breaks and returns a **list of strings**.
    

### Detailed Comparison

Imagine you have a text file named `groceries.txt` that looks like this:

Plaintext

```
Apples
Bananas
Milk
```

#### 1. Using `f.read()`

This reads the entire file into a single string variable. It includes the invisible newline characters (`\n`) that create the line breaks.

Python

```
with open("groceries.txt", "r") as f:
    content = f.read()
    print(content)
    print(repr(content))  # Shows the raw string with hidden characters
```

**Output:**

Plaintext

```
Apples
Bananas
Milk

'Apples\nBananas\nMilk'
```

- **Best for:** When you need the entire text as a single block (like reading an entire essay, a JSON string, or a configuration file).
    
- **Memory Warning:** If you call `.read()` on a massive 10GB file, Python will try to load all 10GB into your computer's RAM at once, which might crash your program.
    

#### 2. Using `f.readlines()`

This reads the entire file and automatically cuts it up into a list, where each line is an individual item in that list.

Python

```
with open("groceries.txt", "r") as f:
    content = f.readlines()
    print(content)
```

**Output:**

Python

```
['Apples\n', 'Bananas\n', 'Milk']
```

- **Best for:** When you want to immediately loop through lines or look up specific lines by their index (e.g., `content[0]`).
    
- **Notice the `\n`:** It keeps the newline character at the end of each string, so you often have to use `.strip()` later to clean them up.
    

### Summary Table

|**Feature**|**f.read()**|**f.readlines()**|
|---|---|---|
|**Return Type**|String (`str`)|List of Strings (`list`)|
|**Structure**|One continuous block of text|Array elements broken up by line|
|**How to access a part**|By slicing string: `text[0:10]`|By index: `lines[2]`|

### 💡 Pro-Tip: The "Pythonic" Alternative

If your goal is to read a file line-by-line, you actually shouldn't use either of these functions. Instead, you can **loop directly over the file object**.

Python

```
with open("groceries.txt", "r") as f:
    for line in f:
        print(line.strip())
```

**Why this is better:** Python will smart-load only **one line at a time** into memory. This means your code can read a 50GB file perfectly without breaking a sweat or slowing down your computer.

## Write:

to create a new file
```
with open("new_test.txt", "w") as f:
    f.write("hello there")

```

every time you write something it creates a new file , to make sure this does not happen use append

to add stuff in the already created file:
```
with open("new_test.txt", "a") as f:
    f.write("\nBuddy !!!")

```

