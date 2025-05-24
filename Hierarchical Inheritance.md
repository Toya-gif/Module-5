# Exp.No:5.c 
## Hierarchical Inheritance

---

### AIM  
To write a Python program to efficiently manage and display the details of doctor and patient records using object-oriented programming (OOP). 

### ALGORITHM

Start

Define a class Details:

Define the _init_ method to initialize id, name, gender, hospital, and department

Define the display_details method to print all the details of the object

Define a class Doctor that inherits from Details:

Define the _init_ method to initialize the doctor's details using the super() function

Define the display method to print "Doctor Object" and call display_details method

Define a class Patient that inherits from Details:

Define the _init_ method to initialize the patient's details using the super() function

Define the display method to print "Patient Object" and call display_details method

Input the doctor's details (id, name, gender, hospital, department)

Create an object doctor of the Doctor class and call doctor.display() to display the doctor's details

Input the patient's details (id, name, gender, hospital, department)

Create an object patient of the Patient class and call patient.display() to display the patient's details

End

### PROGRAM
class Details:

    def _init_(self, id, name, gender, hospital, department):
        self.id = id
        self.name = name
        self.gender = gender
        self.hospital = hospital
        self.department = department

    def display_details(self):
        print(f"Id:  {self.id}")
        print(f"Name:  {self.name}")
        print(f"Gender:  {self.gender}")
        print(f"Hospital:  {self.hospital}")
        print(f"Department:  {self.department}")

class Doctor(Details):

    def _init_(self, id, name, gender, hospital, department):
        super()._init_(id, name, gender, hospital, department)
    
    def display(self):
        print("Doctor Object")
        self.display_details()

class Patient(Details):

    def _init_(self, id, name, gender, hospital, department):
        super()._init_(id, name, gender, hospital, department)
    
    def display(self):
        print("\nPatient Object")
        self.display_details()


d_id = int(input())

d_name = input()

d_gender = input()

d_hospital = input()

d_department = input()

doctor = Doctor(d_id, d_name, d_gender, d_hospital, d_department)

doctor.display()

p_id = int(input())

p_name = input()

p_gender = input()

p_hospital = input()

p_department = input()

patient = Patient(p_id, p_name, p_gender, p_hospital, p_department)

patient.display()


### OUTPUT  

![image](https://github.com/user-attachments/assets/45eb296d-2482-46c4-bb4b-101902677925)
 


### RESULT
Thus, to efficiently manage and display the details of doctor and patient records using object-oriented programming (OOP) was implemented successfully.
