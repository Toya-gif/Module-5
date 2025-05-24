# Exp.No:5.a
## Constructors - Parameterized Constructor


### AIM  
To write a Python code to create a class for a person with a parameterized constructor, which will take the name and userid of the person as parameters and print the userid of the person.

### ALGORITHM

1. Begin the program.  
2. Define a person class.  
3. The person class should have a parameterized __init__ method that accepts two parameters: name and userid.  
4. Inside the __init__ method, assign the name to self.name and the userid to self.userid.  
5. Print the self.userid.  
6. Prompt the user to enter their name (string) and userid.  
7. Create an instance s1 of the person class by passing the entered name and userid to the constructor.  
8. Terminate the program.

### PROGRAM
class Person: 

    def _init_(self, namee, idd):
    
        self.namee = namee
        self.idd = idd 

    def ID(self):
        return self.idd 

namee = input() 

idd = input()

s = Person(namee, idd)  

p = s.ID()  

print(p) 

### OUTPUT
![image](https://github.com/user-attachments/assets/60e37b93-7bf9-471e-a265-446d5c16e1b6)


### RESULT
Thus, Python code to create a class for a person with a parameterized constructor, which will take the name and userid of the person as parameters and print the userid of the person was implemented successfully.
