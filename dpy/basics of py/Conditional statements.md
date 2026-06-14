```
print("calculator:")
print("enter the operation to be performed:[+,-,*,/]")
x = str(input("enter the symbol:"))
a = int(input("enter the number:"))
b = int(input("enter the another number:"))
if x == "+":
    print("you chose addition")
    y = a + b
    print("the value is ", y)
elif x == "-":
    print("You chose subtraction")
    y = a - b
    print("the value is ", y)
elif x == "*":
    print("You chose multiplication ")
    y = a * b
    print("the value is ", y)
elif x == "%":
    print("You chose division ")
    y = a / b
    print("the value is ", y)

```
