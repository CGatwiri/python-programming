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

