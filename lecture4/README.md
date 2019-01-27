# Python Programming - Week 4

* * *

### Answers to Last Week's Homework

#### Calculator
```
def add(a, b):
    return  a + b

def minus(a, b):
    return  a - b

def multiply(a, b):
    return  a * b

def divide(a, b):
    a //b

def calculate(a, b, op):
    if op == '+':
        return add(a, b)
    elif op == '-':
        return minus(a, b)
    elif op == '*':
        return multiply(a, b)
    elif op == '/':
        return divide(a, b)
    elif op == 'q':
        exit(0)
    raise ValueError('Invalid operation')


if __name__ == "__main__":
    op = ''
    while op != 'q':
        a = int(input('Enter a:'))
        b = int(input('Enter b:'))
        op = input('Enter +,-,*,/ or q (q for quit)')
        res = calculate(a, b, op)
        print('{} {} {} is {}'.format(a, op, b, res))
```

* * *


### Import
- What if I want to use PI? Answer: Use import math, and use math.pi
- What if I want to organize my project by moving the calculator as a separate file?

### Object Oriented Programming (Chapter 8)
- Using class

```
class Thing:
    pass


class Animal(Thing):
    pass


class Dog(Animal):
    def __init__(self, name):
        self.name = name

    def bark(self):
        print('woof woof!')


dog = Dog('Corgi')
print(dog.name)
dog.bark()
```
* * *

<a name="practice"></a>
### Practices
- Can you convert the calculator to a class?
- Can you import the calculator as a module?

### Object Oriented Programming (Chapter 8)
Solve the two programming puzzles in page#107 and #108.
