List comprehension offers a shorter syntax when you want to create a new list based on the values of an existing list.
instead of :
```
fruits = ["apple", "banana", "cherry", "kiwi", "mango"]  
newlist = []  
  
for x in fruits:  
  if "a" in x:  
    newlist.append(x)  
  
print(newlist)
```

u can write :
```
fruits = ["apple", "banana", "cherry", "kiwi", "mango"]  
  
newlist = [x for x in fruits if "a" in x]  
  
print(newlist)
```

The _condition_ is like a filter that only accepts the items that evaluate to "True"
