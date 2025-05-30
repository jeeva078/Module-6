# Ex.No:6C Encapsulation

## AIM  
To write a class student with members name ,age,rollno and an user defined function show() to display the details of the student ,use the getter and setter method Information Hiding and conditional logic for setting an object attributes

## ALGORITHM

1. Define a class Student with an __init__() constructor having name, private roll_no, and age.
2. Create a show() method to display the student's name and private roll_no.
3. Define a getter method get_roll_no() to retrieve the private roll_no.
4. Define a setter method set_roll_no() that validates the roll number (ensures it is less than or equal to 50).
5. Create an object jessa of class Student with name, roll number, and age.
6. Call show() to display the initial details.
7. Attempt to change the roll number using the setter method to an invalid value and a valid value.
8. Call show() again to display updated details.
9. End the program.

## PROGRAM
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

# before Modify
jessa.show()# call show()
# changing roll number as 120 using setter


jessa.set_roll_no(120)
jessa.set_roll_no(25)
jessa.show()
```
## OUTPUT
![Screenshot 2025-04-28 160756](https://github.com/user-attachments/assets/3510ac59-4861-4fba-9d9c-15da5bfcb18b)

## RESULT
Thus a class student with members name ,age,rollno and an user defined function show() to display the details of the student ,use the getter and setter method Information Hiding and conditional logic for setting an object attributes has been implemented successfully.

