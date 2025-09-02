# Exp.No:30  
## overloading operator

---

### AIM  
To Write a Python program for simply using the overloading operator for adding two objects.
class name : fruits
object name :  apple, mango, a and b

---

### ALGORITHM
1. Begin the program.
2. Create a class `fruit`:
   - Define the `__init__()` method to initialize the attribute `x`.
   - Define the `__add__()` method to return the sum or concatenation of `self.x` and `u.x`.
3. Accept two integer inputs and create objects `a` and `b` of the `fruit` class.
4. Print the result of `a + b` as the sum of the two integers.
5. Accept two string inputs and create objects `s` and `r` of the `fruit` class.
6. Print the result of `s + r` as the concatenation of the two strings.
7. Terminate the program.


### PROGRAM

```
class fruit:
    def __init__(self,x):
        self.x=x
    def __add__(self,u):
        return self.x + u.x

a = fruit(int(input()))
b = fruit(int(input()))
print("apple and mango mixed:", a+b)
s = fruit(str(input()))
r = fruit(str(input()))
print("fruit mix: ", s+r)
```

### OUTPUT
<img width="781" height="227" alt="image" src="https://github.com/user-attachments/assets/fa3179cd-6224-4cfe-8638-325138bb30d9" />


### RESULT
Thus a Python program for simply using the overloading operator for adding two objects has been executed successfully.
