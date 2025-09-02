# Exp.No:29  
## Encapsulation

---

### AIM  
To Create a class student with members name ,age,rollno and an user defined function show() to display the details of the student ,use the getter and setter method Information Hiding and conditional logic for setting an object attributes

---

### ALGORITHM

1. **Start the Program.**
2. **Define the `Student` class.**
   - Inside the `Student` class, define the `__init__` method to initialize `name` and the private member `__age`.
3. **Define a getter method** `get_age` to return the value of the private member `__age`.
4. **Define a setter method** `set_age` to set a new value to the private member `__age`.
5. **Create an object `stud`** of the `Student` class with the name 'Jessa' and age 14.
6. **Print the name and the age** of `stud` using the getter method.
7. **Use the setter method** `set_age` to change the age of `stud` to 16.
8. **Print the name and the updated age** of `stud` using the getter method.
9. **End the program.**

---

### PROGRAM

```
class Student:
    def __init__(self, name, roll_no, age):
        # private member
        self.name = name
        # private members to restrict access
        # avoid direct data modification
        self.__roll_no = roll_no
        self.__age = age

    def show(self):
        print('Student Details:', self.name, self.__roll_no)

    # getter methods
    def get_roll_no(self):
        return self.__roll_no

    # setter method to modify data member
    # condition to allow data modification with rules
    def set_roll_no(self, number):
        if number > 50:
            print('Invalid roll no. Please set correct roll number')
        else:
            self.__roll_no = number

jessa = Student('Jessa', 10, 15)
jessa.show()
jessa.set_roll_no(120)
jessa.set_roll_no(25)
jessa.show()


```

### OUTPUT
<img width="1040" height="291" alt="image" src="https://github.com/user-attachments/assets/e1d2e633-bdfb-471e-a4de-333c812e09c8" />


### RESULT:
Thus a class student with members name ,age,rollno and an user defined function show() to display the details of the student ,use the getter and setter method Information Hiding and conditional logic for setting an object attributes has been created and executed sccessfully.


