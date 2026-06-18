## basic list:

```
grocery_list = ["apple", "banana"]
print(grocery_list)
grocery_list.append("mangoes")
print(grocery_list)
```

output:
```
PS C:\Users\hp\OneDrive\Desktop\dsa_py> python .\pyBasics.py
['apple', 'banana']
['apple', 'banana', 'mangoes']
```

## Appending:

```
l = [1, 2, 3]
l.append(4)
print(l)

```

## Inserting:

```
l = [1, 2, 3]
l.insert(0, "hi")
print(l)

```

Output:
```
PS C:\Users\hp\OneDrive\Desktop\dsa_py> python .\pyBasics.py
['hi', 1, 2, 3]
```

## Counting:

```
l = [1, 2, 3]
l.insert(0, "hi")
print(l)
print(l.count("hi"))

```
 output:
```
 PS C:\Users\hp\OneDrive\Desktop\dsa_py> python .\pyBasics.py
['hi', 1, 2, 3]
1
```

## Reversing and Removing:

```
l = [1, 2, 3]
l.insert(0, "hi")
print(l)
print(l.count("hi"))
print(l)
l.reverse()
print(l)
l.remove(3)
print(l)

```

output:
```
PS C:\Users\hp\OneDrive\Desktop\dsa_py> python .\pyBasics.py
['hi', 1, 2, 3]
1
['hi', 1, 2, 3]
[3, 2, 1, 'hi']
[2, 1, 'hi']
```

