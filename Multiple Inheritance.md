# Exp.No:5.e
## Multiple Inheritance

### AIM  
To Write a Python program to Get the name, roll no and 4 marks of a student and find & display the total marks and Average using Multilevel inheritance.
### ALGORITHM

start

Define a base class name:

It has an _init_ method that accepts and stores the student’s name (a) and roll number (b)

Define a derived class roll that inherits from name:

Its _init_ method accepts the name, roll number, and marks list (c)

It calls the parent constructor using super()._init_(a, b) to initialize name and roll number

It defines:

A method total() to calculate and return the sum of marks

A method average() to calculate and return the average of marks

Define another derived class result that inherits from roll:

Its _init_ method calls the roll class constructor using super()._init_(a, b, c)

It defines a method disp() to:

Call total() and average()

Print the student's name, roll number, total marks out of 400, and average marks

Input the student's name a

Input the student's roll number b

Input 4 subject marks into a list c

Create an object stu of class result using the input data

Call stu.disp() to display the results

End

### PROGRAM
class name:

    def _init_(self,a,b):
        self.a=a
        self.b=b
class roll(name):

    def _init_(self,a,b,c):
        super()._init_(a,b)
        self.c=c
    def total(self):
        return sum(self.c)
    def average(self):
        return self.total()/len(self.c)
class result(roll):

    def _init_(self,a,b,c):
        super()._init_(a,b,c)
    def disp(self):
        tot=self.total()
        avg=self.average()
        print(f"Name:  {self.a} Rollno:  {self.b} Total Marks out of 400:  {tot}")
        print(f"Average : {avg:.2f}")
a=input().strip()

b=int(input().strip())

c=[int(input().strip()) for _ in range(4)]

stu=result(a,b,c)

stu.disp()

### OUTPUT
 ![image](https://github.com/user-attachments/assets/89a98120-070c-4dcb-9687-e4a038229f88)

### RESULT
Thus, Python program to Get the name, roll no and 4 marks of a student and find & display the total marks and Average using Multilevel inheritance was implemented successfully.
