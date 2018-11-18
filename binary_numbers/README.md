# Binary Numbers

## Integer to Binary and Binary to Integer

### Convert integer to binary

```python
>>> format(8, 'b') # Output in binary number
'1000'
>>> '{0:b}'.format(8) # Another way for formatting number in binary format
'1000'
>>> bin(7) #Yet another way
'0b111'
>>> bin(7)[2:] # Remove '0b'
'111'
```

### Convert binary to integer

```python
>>> int('101', 2)
5
>>> int('1000', 2)
8
```

Let's create our own method for converting integer to binary
```python
>>> # Add 8 leading zeros
>>> def b(num):
...     print(format(num, '08b'))
...
>>> b(3)
00000011
>>> b(8)
00001000
```

#### Quiz

1. What is the value of `format(6, 'b')`?
2. What is the value of `format(5, 'b')`?
3. What is the value of `int(111, 2)`?
4. What is the value of `int(11011, 2)`?

---

## And(`&`), Or(`|`), Xor(`^`), Not(`~`)

#### AND (`&`)

```python
>>> b(3)
00000011
>>> b(1)
00000001
>>> b(3&3)
00000011
```

### OR (`|`)

```python
>>> b(4)
00000100
>>> b(1)
00000001
>>> b(4|1)
00000101
```

### XOR(`^`)

```python
>>> b(4)
00000100
>>> b(5)
00000101
>>> b(4^5)
00000001
```

#### Quiz

1. What is the value of `3 & 5`?
2. What is the value of `3 | 5`?
3. What is the value of `3 ^ 5`?
4. What is the value of `4 & 8`?
5. What is the value of `5 & 7`?
6. What is the value of `8 | 7`?
7. What is the value of `9 ^ 8`?
8. Write an expression to check if an integer is even or odd using `&` operator.
9. Swap two integers without using additional variables.

### Left Shift(`<<`)

```python
>>> b(1)
00000001 # 1 or pow(2, 0)
>>> b(1 << 1)
00000010 # 2 or pow(2, 1)
>>> b(1 << 2)
00000100 # 4 or pow(2, 2)
>>> b(1 << 3)
00001000 # 8 or pow(2, 3)
>>> b(1 << 4)
00010000 # 16 or pow(2, 4)
>>> b(1 << 5)
00100000 # 32 or pow(2, 5)
>>> b(3)
00000011 # 3
>>> b(3 << 1)
00000110 # 6
>>> b(3 << 2)
00001100 # 12
```

### Right Shift (`>>`)

```python
>>> b(5)
00000101 
>>> b(5 >> 1)
00000010 # 2
>>> b(5 >> 2)
00000001 # 1
>>> b(5 >> 3)
00000000 # 0
```

#### Quiz
1. Write a function that converts a 10 digit integer to a binary number.
2. Write a function that converts a binary number to 10 digit integer
