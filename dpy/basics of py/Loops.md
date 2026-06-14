## For loops:

when the items are individually are printed:
```
grocery_list = ["apple", "banana"]
grocery_list.append("mangoes")
print(grocery_list)
print("=========================")
for item in grocery_list:
    print(item)

```

Output:
```
['apple', 'banana', 'mangoes']
=========================
apple
banana
mangoes
```

when all the items are printed till the number of loops are completed:
```
grocery_list = ["apple", "banana"]
grocery_list.append("mangoes")
print(grocery_list)
print("=========================")
for item in grocery_list:
    print(grocery_list)

```

Output:
```
['apple', 'banana', 'mangoes']
=========================
['apple', 'banana', 'mangoes']
['apple', 'banana', 'mangoes']
['apple', 'banana', 'mangoes']
```

**==Types of indexing**==
```
grocery_list = ["apple", "banana", "3"]
grocery_list.append("mangoes")
print(grocery_list)
print("=========================")
for i in [0, 1, 2, 3]:
    print(grocery_list[i])

```

```
grocery_list = ["apple", "banana", "3"]
grocery_list.append("mangoes")
print(grocery_list)
print("=========================")
for i in range(len(grocery_list)):
    print(grocery_list[i])

```

```
grocery_list = ["apple", "banana", "3"]
grocery_list.append("mangoes")
print(grocery_list)
print("=========================")
for i, item in enumerate(grocery_list):
    print(i, item)

```
output :
```
['apple', 'banana', '3', 'mangoes']
=========================
0 apple
1 banana
2 3
3 mangoes
```

## while loops:

decrement:
```
grocery_list = ["apple", "banana", "3"]
grocery_list.append("mangoes")
print(grocery_list)
print("=========================")
j = len(grocery_list) - 1
while j >= 0:
    print(grocery_list[j])
    j -= 1
```

increment:
```
grocery_list = ["apple", "banana", "3"]
grocery_list.append("mangoes")
print(grocery_list)
print("=========================")
i = 0
while i < len(grocery_list):
    print(grocery_list[i])
    i += 1

```
