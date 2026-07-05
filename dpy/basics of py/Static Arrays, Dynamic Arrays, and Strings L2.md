
Static Arrays, Dynamic Arrays, and Strings - Big O Complexity

## Arrays:

**Append:**
```
A = [1, 2, 3, 4, 5]
# Append = Insert element at the end of array. on average O(1)
A.append(6)
print(A)

```

**Pop:**
```
A = [1, 2, 3, 4, 5]
# pop =deletes the last element .average O(1).
A.pop()
print(A)
```

**Insert:**
```
A = [1, 2, 3, 4, 5]
# Insert not at end of array. Average O(n)
A.insert(3, 20)
print(A)

```

**Modify:**
```
A = [1, 2, 3, 4, 5]
# Modify the array. Average O(1)
A[0] = 12
print(A)

```

Accessing:
```
A = [1, 2, 3, 4, 5]
# Accessing elements given index . Average i-O(1)
print(A[2])

```

Checking elements:
```
A = [1, 2, 3, 4, 5]
# Checking elements in array . Average O(1)
if 3 in A:
    print(True)
```

## Strings:

appending:
```
# Append to end of string . Average O(1)
a = "Hello"
b = a + "z"
print(b)

```

Checking a String:
```
# Check if something is in  string . Average O(1)
a = "Hello"
if "H" in a:
    print(True)

```

