# Ex.No:6B COUNTER CLASS

## AIM  
To write  Counter class which  has one attribute called current which defaults to zero. And it has three methods:
- increment() increases the value of the current attribute by one.
- value() returns the current value of the current attribute
- reset() sets the value of the current attribute to zero
create a new instance of the Counter class and calls the increment() method three times before showing the current value of the counter to the screen

## ALGORITHM

1. Begin the program.
2. Define the Counter class:
3. Initialize the current attribute to 0 in the __init__ method.
4. Define the increment method to increase current by 1.
5. Define the value method to return the current value of current.
6. Define the reset method to set current to 0.
7. Create an instance of the Counter class.
8. Call the increment method three times to increase the counter's value.
9. Call the value method to print the current value of the counter.
10. Terminate the program.

## PROGRAM
```
class Counter:
    def __init__(self):
        self.current = 0

    def increment(self):
        self.current += 1

    def value(self):
        return self.current

    def reset(self):
        self.current = 0

counter = Counter()
counter.increment()
counter.increment()
counter.increment()

print(counter.value())
```

## OUTPUT
![Screenshot 2025-04-28 161903](https://github.com/user-attachments/assets/a66c0a9f-d0fe-4620-aff6-5216e7cd8680)

## RESULT
Thus Counter class which  has one attribute called current which defaults to zero has been implemented successfully.
