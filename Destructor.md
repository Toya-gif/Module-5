# Exp.No:5.b
## Destructor

### AIM  
To Write a python code to implement destructor in given code.


### ALGORITHM

1. Begin the program.  
2. Define the student class.  
3. Inside the student class, define the __init__ method (constructor) and the __del__ method (destructor).  
4. Create an object s2 of the student class. When the object s2 is created, the __init__ method is called, and its print statements are executed.  
5. Use the del statement to delete the object s2. This triggers the __del__ method (destructor), and the respective print statements are executed.  
6. Terminate the program.

---

### PROGRAM
class Type:

    def _new_(cls,args,*kwargs):
        print("new executing")
        return super()._new_(cls)
    def _init_(self):
        print("init executing")
    def _del_(self):
        print("del executing")
obj1=Type()

obj2=Type()

del obj1

del obj2

print("end of program")

### OUTPUT
![image](https://github.com/user-attachments/assets/bf9d37d2-0f71-41d1-b4a3-7fe39fa8746f)


### RESULT
Thus, python code to implement destructor is successfully implemented.
