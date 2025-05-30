# Ex.No:6E Operator Overloading

## AIM  
To write a python program to perform subtraction of two complex number using binary '+' operator overloading ,class name : complex
Ob1 = complex(1, 2) and Ob2 = complex(2, 3)

## ALGORITHM

1. Define a class complex with an __init__() method to initialize the complex numbers a and b.
2. Define the __add__() method to handle the addition operation for two complex objects.
3. The __add__() method should return a tuple of the difference of real and imaginary parts.
4. Create two objects ob1 and ob2 of the complex class with specified real and imaginary values.
5. Add the two complex objects (ob1 and ob2) using the + operator.
6. Print the result of the addition (the tuple returned by the __add__() method).
7. End the program.

## PROGRAM
```
class complex:
    def __init__(self,a,b):
        self.a=a
        self.b=b
    def __add__(self,other):
        return self.a-other.a,self.b-other.b
ob1=complex(1,2)
ob2=complex(2,3)
ob3=ob1+ob2
print(ob3)
```
## OUTPUT
![Screenshot 2025-04-28 161328](https://github.com/user-attachments/assets/64ec294b-51e5-442a-ac2b-f2e4f20c248b)

## RESULT
Thus a python program to perform subtraction of two complex number using binary '+' operator overloading has been implemented successfully.

