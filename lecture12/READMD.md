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
