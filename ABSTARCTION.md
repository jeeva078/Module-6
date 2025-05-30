# Ex.No:6A Abstraction

## AIM  
To Write an abstract method course () and a method print) visible to the user. The inherited class here is demo class and learn and has their course () method. The objects are created for the respective class and invoke the course () method for both of the classes. 

## ALGORITHM

1. Import ABC and abstractmethod from abc module.
2. Define an abstract class educlass with a method print() and an abstract method course().
3. Create a class testclass that inherits from educlass and defines the course() method.
4. Create a class democlass that inherits from educlass and defines the course() method.
5. Create an object t1 of testclass and call its course() method.
6. Create an object ex of democlass and call its course() method.
7. Check if t1 is an instance of educlass and print the result.
8. Check if ex is an instance of educlass and print the result.
9. End the program.

## PROGRAM
```
from abc import ABC, abstractmethod
class educlass(ABC):
    def print(self,a):
        print("The value is:  ", a)
    @abstractmethod
    def course(self):
        pass
    def print(self,a):
        print(f"The value is:  {a}")
class testclass(educlass):
    def course(self):
        print("This is test class")
        self.print(500)
class democlass(educlass):
    def course(self):
        print("This is demo class")
        self.print(850)
t1=testclass()
t1.course()
ex=democlass()
ex.course()
print("t1 is instance of educlass? ", isinstance(t1, educlass))
print("ex is instance of educlass? ", isinstance(ex, educlass))

```
## OUTPUT
![Screenshot 2025-04-28 155854](https://github.com/user-attachments/assets/4146aab5-d451-49b2-92df-6b5291ab0f04)

## RESULT
Thus an abstract method course () and a method print) visible to the user. The inherited class here is demo class and learn and has their course () method. The objects are created for the respective class and invoke the course () method for both of the classes has been implemented successfully.
