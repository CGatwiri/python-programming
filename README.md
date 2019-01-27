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

---

* * *

* [Presentation for Week 5](https://docs.google.com/presentation/d/1FUcFb78FCY9WI3JxZdZJAR-JmhqIJ4gZu3GnRlptivg/edit?usp=sharing)


### Review of Homework

![alt text](/images/python_week5_homework.png)

- name of class should start with upper case
- variables and methods should be all lower case
- Here is an example of the [source code](https://github.com/bellevuecodeschool/python-programming/blob/master/lecture6/shelter.py) for the homework


* * *

### Let's Practice Typing
- Go to [Nitro Type](https://www.nitrotype.com)
- Practice typing for 5 minutes
- Let's measure your typing speed

### Chapter 9 - Python’s Built-in Functions
Launch IDLE

##### input()
```
>>> year = input('Year of birth: ')
Year of birth: 2000
>>> 'You were born in {}'.format(year)
'You were born in 2000'
>>>
```

##### len(), min(), max(), sum()
```
>>> A = [5, 4, 10, 20, 30]
>>> len(A)
5
>>> min(A)
4
>>> max(A)
30
>>> sum(A)
69
```

##### type conversion
```
>>> a = '5.5'
>>> int(a)
Traceback (most recent call last):
  File "<pyshell#42>", line 1, in <module>
    int(a)
ValueError: invalid literal for int() with base 10: '5.5'
>>> float(a)
5.5
>>> bool(a)
True
>>> a = 0
>>> bool(a)
False
>>> a = 10
>>> a = '10'
>>> a + 20
Traceback (most recent call last):
  File "<pyshell#49>", line 1, in <module>
    a + 20
TypeError: must be str, not int
>>> int(a) + 20
30
```

##### abs()
```
abs(-10)
>>> if abs(steps) > 0:
	print('character is moving')
-> Recover (by typing on a line)
```

##### dir(), help()
```
>>> dir('hello')
>>> help('hello'.upper)
>>> 'hello'.upper()
'HELLO'
```

##### eval()
```
eval()
>>> formula = input('Enter formula: ')
Enter formula: 12*52
>>> eval(formula)
624
```

##### File open / write

```
>>> file = open('C:\Users\jason\Documents\hello.txt')
SyntaxError: (unicode error) 'unicodeescape' codec can't decode bytes in position 2-3: truncated \UXXXXXXXX escape
>>> file = open('C:\\Users\\jason\\Documents\\hello.txt')
>>> print(file.read())
fdsfasfsfasfas
>>>
KeyboardInterrupt
>>> file = open('C:\\hello.txt')

>>> file = open('C:\\Users\\jason\\Documents\\hello2.txt', 'w')
>>> file.write('This is a test.')
15
>>> file.close()
```

##### Quiz
```
>>>bool(4)
>>>a, b = 10, ‘20’
>>>a+b
```

### Code Combat
- https://codecombat.com

---

# Week 7

* * *

* [Presentation for Week 7](https://docs.google.com/presentation/d/1FUcFb78FCY9WI3JxZdZJAR-JmhqIJ4gZu3GnRlptivg/edit?usp=sharing)


### Review of Homework


* * *

### Let's Practice Typing
- Go to [Nitro Type](https://www.nitrotype.com)
- Practice typing for 5 minutes
- Let's measure your typing speed

* * *

### Chapter 10 - Useful Python Modules

##### turtle
```
>>> import turtle
```

##### random
```
>>> import random
>>> A = [10, 20, 30, 40, 50]
>>> random.choice(A)
50
>>> random.choice(A)
30
>>> random.choice(A)
50
>>> random.choice(A)
30
>>> random.choice(A)
40
```

##### time
```
>>> import time
>>> time.time()
1511711769.7801137
>>> time.time()
1511711773.4365573
>>> time.asctime()
'Sun Nov 26 07:56:51 2017'
>>> time.localtime()
time.struct_time(tm_year=2017, tm_mon=11, tm_mday=26, tm_hour=7, tm_min=57, tm_sec=12, tm_wday=6, tm_yday=330, tm_isdst=0)
>>> time.localtime()[0]
2017
>>>
```

##### pickle
```
>>> A = [10, 20, 30, 40, 50]
>>> import pickle
>>> pickle.dump(A, open('my_data.p', 'wb'))

# Close IDLE and re-launch IDLE
>>> A = pickle.load(open('my_data.p','rb'))
>>> A
[10, 20, 30, 40, 50]
```

* * *

### Code Combat
- https://codecombat.com

---

# Week 8 

* * *


### Chapter 12 - Using TKinter for Better Graphics

#### GUI Programming

##### Tkinter
```
>>> from tkinter import *
>>> tk = Tk()
>>> btn = Button(tk, text='click here')
>>> btn.pack()
```

* * *

##### Button
```
>>> from tkinter import *
>>> tk = Tk()
>>> def hello():
	print('Hello!')
>>> btn = Button(tk, text='Click here', command=hello)
>>> btn.pack()
```

* * *

##### Button + Messagebox
```
>>> from tkinter import *
>>> from tkinter import messagebox
>>> tk = Tk()
>>> def about():
	messagebox.showinfo('About', 'GUI v1.0')


>>> btn = Button(tk, text='About', command=about)
>>> btn.pack()
```

* * *

##### Canvas
```
>>> from tkinter import *
>>> tk = Tk()
>>> canvas = Canvas(tk, width=500, height=500)
>>> canvas.pack()
>>> canvas.create_line(0, 0, 500, 500)
```

* * *

##### Line, Rectangle, Oval
```
>>> from tkinter import *
>>> tk = Tk()
>>> canvas = Canvas(tk, width=500, height=500)
>>> canvas.pack()
>>> canvas.create_line(0, 100, 200, 0, fill='red', dash=(4, 4))
>>> canvas.create_rectangle(50, 25, 150, 75, fill='blue')
>>> canvas.create_oval(250, 250, 300, 300)
```

* * *

##### Interactive drawing
```
>>> from tkinter import *
>>> tk = Tk()
>>> canvas = Canvas(tk, width=500, height=500)
>>> canvas.pack()
>>> def paint(e):
	canvas.create_oval(e.x - 1, e.y - 1, e.x + 1, e.y + 1, fill='green')
>>> canvas.bind('<B1-Motion>', paint)
>>> def clear(e):
	canvas.delete('all')
>>> canvas.bind('<Button-3>', clear) # Right-click
```

* * *

### Code Combat
- https://codecombat.com

---

# Week 9

### Chapter 12 - Using TKinter for Better Graphics (Cont.)

#### GUI Programming

* * *

##### Text
```
>>> from tkinter import *
>>> tk = Tk()
>>> canvas = Canvas(tk, width=500, height=500)
>>> canvas.pack()
>>> canvas.create_text(150, 100, text='Once upon a time, there lived a wolf under a bridge')
>>> canvas.create_text(150, 200, text='Once upon a time, there lived a wolf under a bridge', font=('Times', 15), fill='red')
```

* * *

##### Polygons
```
>>> from tkinter import *
>>> tk = Tk()
>>> canvas = Canvas(tk, width=500, height=500)
>>> canvas.pack()
>>> points = [0, 0, 500, 250, 0, 500]
>>> canvas.create_polygon(points, outline='green', fill='yellow', width=3)
```

* * *

##### Polygon -> triangle - move
```
import time
from tkinter import *
tk = Tk()
canvas = Canvas(tk, width=400, height=400)
canvas.pack()
canvas.create_polygon(10, 10, 10, 60, 50, 35)
for x in range(0, 60):
    canvas.move(1, 5, 5)
    tk.update()
    time.sleep(0.05)
```

* * *

##### Image
```
>>> from tkinter import *
>>> tk = Tk()
>>> canvas = Canvas(tk, width=400, height=400)
>>> canvas.pack()
>>> img = PhotoImage(file='C:\\Users\\someuser\\Documents\\Projects\\cat.gif')
>>> canvas.create_image(0, 0, anchor=NW, image=img)

>>> canvas.move(1, 5, 0)

>>> def move(e):
	if e.keysym == 'Up':
		canvas.move(1, 0, -3)
	elif e.keysym == 'Down':
		canvas.move(1, 0, 3)
	elif e.keysym == 'Left':
		canvas.move(1, -3, 0)
	else:
		canvas.move(1, 3, 0)

>>> canvas.bind_all('<KeyPress-Up>', move)
>>> canvas.bind_all('<KeyPress-Down>', move)
>>> canvas.bind_all('<KeyPress-Right>', move)
>>> canvas.bind_all('<KeyPress-Left>', move)
```

* * *

### Code Combat
- https://codecombat.com

---

# Week 10

### How to Become a Good Programmer?
- Write a Beautiful Program
- [Type Fast](/topic/how-to-type-fast)
- Focus
- What to do when you are stuck?

### What to Do When You Are Stuck (more than 20 minutes)?
- Search for a clue or answer (Google, Book, etc.)
- [Talk to a rubber duck](https://en.wikipedia.org/wiki/Rubber_duck_debugging)
- Ask for help (Talk to your friend or colleague)
- Take a break (Go to restroom or go for a walk)

### Quiz

1. Guess the outcome of the following code, and then execute each line to verify your guess

```
type('Hello World')
```
```
type(17)
```
```
type(12.5)
```
```
type([1, 3])
```
```
type((1, 3))
```
```
type({'first_name':'James', 'last_name':'Bond'})
```

2. Guess the outcome of the following code, and then execute each line to verify your guess

```
A = list(range(1, 11))
A[2:8]
A[2:]
A[:8]
A[2:8:2]
A[::-1]
```
```
A = [x*2 for x in range(1, 11)]
```
```
from random import *
A = [randint(1, 100) for _ in range(10)]
```

### Exception Handling

* * *

### Code Combat
- https://codecombat.com

---

# Week 11

### How to Become a Good Programmer?
- Write a Beautiful Program
- [Type Fast](/topic/how-to-type-fast)
- Focus
- What to do when you are stuck?
- **Be fluent in Data Structure and Algorithms**

### Violinist's Dying Wish
- An extremely talented violinist who never learned how to read

### Review Homework

### Quiz

1. Guess the outcome of the following code, and then execute each line to verify your guess

```
>>> a = 1
>>> b = 2
>>> def foo():
	b = 10
	c = 3
	return a + b + c

>>> foo()
>>> print(a)
>>> print(b)
>>> print(c)
```

### Q & A


### Chapter 14 - Finishing Your First Game: Bounce!

- Follow the book by typing code and run the programming on each page. Make sure that the program runs successfully. If not, find bugs and fix them.
- Don't type the entire code at the end of the chapter because it is more difficult to find bugs when the code is big.

* * *

### Code Combat
- https://codecombat.com

---

# Week 12

### How to Become a Good Programmer?
- Write a Beautiful Program
- [Type Fast](/topic/how-to-type-fast)
- Focus
- What to do when you are stuck?
- Be fluent in Data Structure and Algorithms
- Be a T-shaped person

### What to Do When You Are Stuck (more than 20 minutes)?
- Search for a clue or answer (Google, Book, etc.)
- [Talk to a rubber duck](https://en.wikipedia.org/wiki/Rubber_duck_debugging)
- Ask for help (Talk to your friend or colleague)
- Take a break (Go to restroom or go for a walk)

### Quiz

1. Guess the outcome of the following code, and then execute each line to verify your guess

```
>>> class Person(object):
	    def say(self):
		    print('I\'m a person')

>>> class Student(Person):
	    pass

>>> bob = Student()
>>> bob.say()
```

2. Guess the outcome of the following code, and then execute each line to verify your guess

```
>>> class Person(object):
	    def say(self):
		    print('I\'m a person.')

>>> class Student(Person):
	    def say(self):
	        print('I\'m a student.')

>>> bob = Student()
>>> bob.say()
```


3. Guess the outcome of the following code, and then execute each line to verify your guess

```
>>> class Person(object):
	    def say(self):
		    print('I\'m a person.')

>>> class Student(Person):
        def say(self):
            super(Student, self).say()
	        print('I\'m a student.')

>>> bob = Student()
>>> bob.say()
```

### Unit Testing


* * *

### Code Combat
- https://codecombat.com

