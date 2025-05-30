# Ex.No:6D Method Overriding

## AIM  
To write a Python program to create a Parent class `Bird` and inherit two child classes `Sparrow` and `Ostrich` from the `Bird` class with the same method `flight()`. Create an object for each class and call the methods of the class which will print the name of the bird that is flying.

## ALGORITHM

1. **Begin the program.**
2. **Define the Bird class**:
   - Create a method `intro()` to print "There are many types of birds."
   - Create a method `flight()` to print "Most of the birds can fly but some cannot."
3. **Define the Sparrow class**, which inherits from `Bird`:
   - Override the `flight()` method.
   - Call the `intro()` method from the parent class.
   - Print "Sparrows can fly."
4. **Define the Ostrich class**, which inherits from `Bird`:
   - Override the `flight()` method.
   - Call the `intro()` method from the parent class.
   - Print "Ostriches cannot fly."
5. **Create an object `obj_bird`** of the `Bird` class.
6. **Create an object `obj_spr`** of the `Sparrow` class.
7. **Create an object `obj_ost`** of the `Ostrich` class.
8. **Print the general message** "There are many types of birds."
9. **Call the `flight()` method** on each object (`obj_bird`, `obj_spr`, `obj_ost`) to display the respective messages.
10. **Terminate the program.**

## PROGRAM
```
class Bird:
    def intro(self):
        print("There are many types of birds.")
	
    def flight(self):
        print("Most of the birds can fly but some cannot.")

class sparrow(Bird):
    def intro(self):
        print("Sparrows can fly.")
    def flight(self):
        print("There are many types of birds.")
	
class ostrich(Bird):
    def intro(self):
        print("Ostriches cannot fly.")
    def flight(self):
        print("There are many types of birds.")
	
obj_bird = Bird()
obj_spr = sparrow()
obj_ost = ostrich()
obj_bird.intro()
obj_bird.flight()
obj_bird.intro()
obj_spr.intro()
obj_spr.flight()
obj_ost.intro()
```

## OUTPUT
![Screenshot 2025-04-28 165006](https://github.com/user-attachments/assets/4ec2f690-60a4-4b8d-8e64-029698544090)

## RESULT
Thus a Python program to create a Parent class `Bird` and inherit two child classes `Sparrow` and `Ostrich` from the `Bird` class with the same method `flight()` has been implemented successfully.
