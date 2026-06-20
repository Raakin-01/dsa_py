
```
t = (1, 2)
print(t)

```

Output:
```
PS C:\Users\hp\OneDrive\Desktop\dsa_py> python .\pyBasics.py
(1, 2)
```

Tuples are immutable
```
t = (1, 2)
print(t)
t[0] = 5
print(t)

```

Output:
```
PS C:\Users\hp\OneDrive\Desktop\dsa_py> python .\pyBasics.py
(1, 2)
Traceback (most recent call last):
  File "C:\Users\hp\OneDrive\Desktop\dsa_py\pyBasics.py", line 3, in <module>
    t[0] = 5
    ~^^^
TypeError: 'tuple' object does not support item assignment
```
->the elements present inside the tuples cannot be changed .
