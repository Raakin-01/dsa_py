simple function to print :
```
def nprint(s):
    print(s)


nprint("hi+2")
```

Return statement:
```
def time2(x):
    return x * 2


print(time2(5))
```

copying:
```
from copy import deepcopy

a = [0, 1, 2, 3]
b = deepcopy(a)
print(a)
print(b)
a[0] = 10
print(a)
print(b)
```

output:
```
PS C:\Users\hp\OneDrive\Desktop\dsa_py> python .\pyBasics.py
[0, 1, 2, 3]
[0, 1, 2, 3]
[10, 1, 2, 3]
[0, 1, 2, 3]
```

