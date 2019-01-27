# python-programming

- Website: [www.geekdojo.io](http://www.geekdojo.io)

- Lecture node and study materials for the python programming course

- Textbook for this course: [Python for Kids](https://www.amazon.com/Python-Kids-Playful-Introduction-Programming-ebook/dp/B00ADX21Z6/ref=pd_sim_351_1?_encoding=UTF8&psc=1&refRID=D5FGHR1ZQZNJ0QEHG9Z0)

# Python Programming - Week 1
* * *

### Install PyCharm
1. Go to https://www.jetbrains.com/pycharm/download
2. Click the "Download" button for "Community"
(Please ask your parents to install the PyCharm program if you have difficulty)

### Hello World
Write the following code, and run.
```
print("Hello World!)
```

### Hello World using variable 1
Write the following code, and run.
```
message = "Hello World!"
print(message)
```

### Hello World using variable 2
Write the following code, and run.
```
message1 = "Hello"
message2 = "World"
final_message = message1 + " " + message2 + "!"
print(final_message)
```

### Add using variables
Write the following code, and run.
```
a = 1
b = 2
c = a + b
print("Answer is ", c)
```

### Subtract using variables
```
a = 1
b = 2
c = b - a
print("Answer is ", c)
```

### Multiply using variables
```
a = 2
b = 4
c = a * b
print("Answer is ", c)
```


### Divide using variables
```
a = 8
b = 4
c = a // b
print("Answer is ", c)
```

### Accepting user's Input 1
```
name = input("What's your name?")
message = "Hello, " + name
print(message)
```

### Accepting user's Input 2
```
first_name = input("What's your first name?")
last_name = input("What's your last name?")
message = "Your first name is " + first_name + " and last name is " + last_name + "."
print(message)
```

### Accepting user's Input 3
```
first_name = input("What's your first name?")
last_name = input("What's your last name?")
print("Your first name is {} and last name is {}".format(first_name, last_name))
```

### Accepting number as input 1
```
a = input("a:")
b = input("b:")
c = a + b
print(c)
```

### Accepting number as input 2
```
a = int(input("a:")) #convert input to integer
b = int(input("b:")) #convert input to integer
c = a + b
print(c)
```

### if ...
```
a = 15
if a % 5 == 0: # % is a 'mod' operator.
    print("{} is multiples of 5.".format(a))
```

### if ... else ...
```
a = 15
if a % 5 == 0: # % is a 'mod' operator.
    print("{} is multiples of 5.".format(a))
else:
    print("{} is not multiples of 5.".format(a))
```

### if... elif ... else
```
a = 2000
if a >= 1000:
    print('high')
elif a >= 100 and a < 1000:
    print('medium')
else:
    print('low')
```

---

# Python Programming - Week 2

* * *

* Type all examples in chapter #3  (Strings, Lists, Tuples, and Maps)

* Type all examples in chapter #6 (Going Loopy)

* CodeCombat!!!

* * *

<a name="practice"></a>
### Practices
#### Chapter 3
Solve the three programming puzzles in page#41 and #42
<br /><br />

#### Chapter 6
Solve the four programming puzzles in page#78, 79 and 80.
<br /><br />

#### FizzBuzz
Print from 1 to 100, but replace multiples of 3 with "Fizz" and multiples of 5 with "Buzz" and multiples of both with "FizzBuzz".
<br /><br />

#### Data compression
Data compression is used everywhere. Video encoding, audio encoding, image files and zip files are all using data compression algorithms. Let's write our own. Write a program that compresses a string and say the compressed string.

Examples: If the substring is a sequence of 3 'a'("aaa"), it will be represented as "a3".

Example: "abcaaabbb" -> print "abca3b3"

Example: "abcd" -> print "abcd"

Example: "aaabaaaa" -> print "a3ba4"

Example: "ab" -> print "ab"

Example: "aaabbbcd" -> print "a3b3cd"

---

# Python Programming - Week 3

* * *

### Answers to Last Week's Homework
#### Chapter 3
##### #1: Favorites
```
games = ['baseball', 'football']
foods = ['yogurt', 'steak']
favorites = games + foods
print(favorites)
```

##### #2: Counting Combatants
```
res = (3*25)+(2*40)
print(res)

```

#### #3: Greetings!
```
first_name, last_name = 'John', 'Doe'
str_template = 'Hi there, %s %s!'
print(str_template % (first_name, last_name))

```
* * *

#### Chapter 6
##### #1: The Hello Loop
It will print 'hello 0.'

##### #2: Event Numbers
```
age = int(input("Enter your age: "))
start = 2 if age % 2 == 0 else 1
for x in range(start, age + 1, 2):
    print(x)
```

#### #3: My Five Favorite Ingredients
```
ingredients = ['snails', 'leeches', 'gorilla belly-button lint',
               'caterpillar eyebrows', 'centipede toes']
for i, item in enumerate(ingredients):
    print('%s %s' % (i + 1, item))
```

#### #4: Your Weight on the Moon
```
start = int(input("Enter your weight in kilogram: "))
for w in range(start, start + 16):
    print(w * 0.165)
```

* * *

#### FizzBuzz
```
for i in range(1, 101):
    if i % 15 == 0:
        print('FizzBuzz')
    elif i % 5 == 0:
        print('Buzz')
    elif i % 3 == 0:
        print('Fizz')
    else:
        print(i)
```

* * *

#### Data compression
```
input_str = input('Enter string:')
prev, res, length = '', '', 0


def build_result(s, n, output):
    if n > 1:
        return output + s + str(n)
    else:
        return output + s


for cur in input_str:
    if prev == cur:
        length += 1
    else:
        if length > 0:
            res = build_result(prev, length, res)
        length = 1
    prev = cur
res = build_result(prev, length, res)
print(res)
```
* * *

#### Two Sum - Using bruit force
```
A = [5, 3, 7, 8, 1]
k = 11

res = None
for i in range(len(A)):
    for j in range(i+1, len(A) - i):
        if A[i] + A[j] == k:
            res = [A[i], A[j]]
            break
    if res:
        break
print(res if res else "Not found")
```

#### Two Sum - Using dictionary
```
A = [5, 3, 7, 8, 1]
k = 11

dict = {}
for num in A:
    if num in dict:
        print(k - num, num)
    else:
        dict[k - num] = num
```

#### Two Sum - Using sorting
```
A = [5, 3, 7, 8, 1]
k = 11

A = sorted(A)
i, j = 0, len(A) - 1
while i < j:
    sum = A[i] + A[j]
    if sum < k:
        i += 1
    elif sum > k:
        j -= 1
    else:
        print(A[i], A[j])
        break
```

* * *
* * *
<a name="practice"></a>
### Practices

#### Chapter 7
* Type all examples in chapter #7  (Recycling Your Code With Functions And Modules)

* * *

#### Calculator - Create a calculator that accepts three inputs (a, b and op) where a and b are integers, and op is a string with one of following values: +, -, \*, / or q. If op is 'q', quit program. Use the template below as a skeleton code:

```

def add(a, b):
    pass

def minus(a, b):
    pass

def multiply(a, b):
    pass

def divide(a, b):
    pass

def calculate(a, b, op):
    pass

if __name__ == "__main__":
    op = ''
    while op != 'q':
        a = int(input('Enter a:'))
        b = int(input('Enter b:'))
        op = input('Enter +,-,*,/ or q (q for quit)')
        res = calculate(a, b, op)
        print('{} {} {} is {}'.format(a, op, b, res))

```


#### CodeCombat!!!
Play for 20 minutes

* * *

---

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

---


# Python Programming - Lecture 5

* * *

* [Presentation for Week 5](https://docs.google.com/presentation/d/1FUcFb78FCY9WI3JxZdZJAR-JmhqIJ4gZu3GnRlptivg/edit?usp=sharing)


* * *

### Let's Practice Typing
- Go to [Nitro Type](https://www.nitrotype.com)
- Practice typing for 5 minutes
- Let's measure your typing speed

* * *

### Object Oriented Programming (OOP)

- Please refer to the presentation
- [Source code for Crazy Giraffe](./crazygiraffe.py)

* * *

### Homework for this week
![alt text](./homework.png)

