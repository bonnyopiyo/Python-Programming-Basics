# Python Fundamentals

Variables and Data Types

Operators

Control Statements

Functions

Classes and Objects

Collecting Data

Slicing and Dicing

Boxplot

Scatterplot

Visualisation

## 1. Variables and Data Types

What Are Variables in Python?

How to declare variables

Data Types in Python


```python
A = 10
a = 10
#variable is declared as the value 10 is assigned to it
```

## Data types in Python

### Numerical Data Types

1. Integers

2. Float

3. Complex Numbers

4. Boolean

### 1. Integers


```python
x = 89
y = 234
type(x)
type(y)
# it will be the integer as long as the value is a whole number.
```




    int



### 2. Float


```python
x = 10.45
y = 12.34
type(x)
```




    float



### 3. Complex


```python
x = 10 + 5j
type(x)
```




    complex



### 4. Boolean


```python
num = 6 < 5
#num is the boolean variable
type(num)
#the output will be a bool
print(num)
#this will print False
```

    False
    

### 5. Strings


```python
name = 'Cybercrafts'
name[3]
#this will give us the output as 'e'
```




    'e'



#### Command line input for strings


```python
x = input()
print('Hello', x)
```

    Bonface Osindi
    Hello Bonface Osindi
    

#### Operations using strings


```python
school  = 'cybercrafts'
school.upper()
#this will mke the letters to uppercase.
school.lower()
#this will transfrom to lowercase
school.replace('r', 'R')
#this will replace a letter r with R
name[1:4]
#this will return the strings starting at index 1 until index 4
```




    'ybe'



# Lists


```python
mylist = [10,20,30,40,45,56, 'cybercrafts']
```

## Accessing values from a list


```python
mylist [2:6]
#this will get the values from index 2 until index 6.
```




    [30, 40, 45, 56]



## Adding/Replacing values in a list


```python
mylist[6] = 'python'
#this will replace the value at the index 6 
print(mylist)
```

    [10, 20, 30, 40, 45, 56, 'python']
    


```python
mylist.append('Web Programming')
#this will add the value at the end  of the list
print(mylist)
```

    [10, 20, 30, 40, 45, 56, 'python', 'Web Programming']
    


```python
mylist.insert(5, 'data science')
#this will add the value at the index 5
print(mylist)
```

    [10, 20, 30, 40, 45, 'data science', 56, 'python', 'Web Programming']
    

clear()  removes all the elements from the list

copy() returns a copy of the list

extend() add the elements of the list to the end of the current list

count() retruns the number of elements of the specified value

### Assignment

specify the functions they perform and do an example in each

Submit your assignments through the email

index(), pop(), remove(), sort(), reverse()



```python
a = [10, 20, 30]
b = [60, 50 , 40, a]
#to access a value from the list a we can write

b[3][2]
# this will return 30 as output
```




    30



# Tuples


```python
mytupple = (10,10,20,30,40,50)
#to count the number of elements
print(mytupple)
mytupple.count(10)
#the output here is 2
#to find the index
mytupple.index(50)
#the output will be 5, since the index number at 50 is 5
```

    (10, 10, 20, 30, 40, 50)
    




    5



# Sets


```python
myset = { 10, 20, 30, 40, 50}
myset
```




    {10, 20, 30, 40, 50}




```python
for x in myset:
    print(x)
    #this will get all the values
```

    40
    10
    50
    20
    30
    


```python
20 in myset
#this will return true if the value is in the set
```




    True




```python
#to add a value in a set
myset.add('Bonnie')
print(myset)
```

    {40, 10, 'Bonnie', 50, 20, 30}
    

# Dictionary


```python
mydictionary = { 'python': 'data science', 'machine learning': 'tensorflow','artficial intelligence':'keras'}
```


```python
mydictionary['machine learning']
#this will give the output as 'tensorflow'
```




    'tensorflow'




```python
mydictionary.get('python')
#this serves the same purpose to access the value.
```




    'data science'



### Data Manipulation in a dictionary


```python
#add a new value
mydictionary['analysis'] = 'matplotlib'
print(mydictionary)
```

    {'python': 'data science', 'machine learning': 'tensorflow', 'artficial intelligence': 'keras', 'analysis': 'matplotlib'}
    


```python
#replacing a value
mydictionary['analysis'] = 'pandas'
mydictionary
```




    {'python': 'data science',
     'machine learning': 'tensorflow',
     'artficial intelligence': 'keras',
     'analysis': 'pandas'}




```python
#deleting a value
mydictionary.pop('analysis')
print(mydictionary)
```

    {'python': 'data science', 'machine learning': 'tensorflow', 'artficial intelligence': 'keras'}
    

# Range 


```python
for x in range(12):
    print(x)
    #this will print numbers from 0-10. Range will have the numbers from 0-10
```

    0
    1
    2
    3
    4
    5
    6
    7
    8
    9
    10
    11
    

# Type casting


```python
a = [10, 20, 30, 40]
#to change this list into a tuple l can simply write
tuple(a)
#now the list will change to a tuple
```




    (10, 20, 30, 40)



# 2 Operators

What is an operator

Types of operators

## Types of Operators

Arithmetic Operators

Assignment Operators

Comparison Operators

Logical Operators

Membership Operators

Identity Operators

Bitwise Operators

## Arithmetic Operators 


```python
x = 10
y= 14
#addition
x+y
#subtracion
x-y
#multiplication
x*y
#division
x/y
#floor division
x//y
#modulus
x%y
#exponentiation
x ** y
```




    100000000000000



## Comparison Operators


```python
x = 5
y = 3

#equal
x == 5
y == 4

x != 5
```




    False



## Logical Operators


```python
#logical and
5 > 3 and 5 > 4
#it will return true, since both statements are true
5 > 3 or 5 < 2
#it will return true, since one of the statements is true
not(5>2 and 5<3)
#it will return true, even when  logical and will return false

```




    True



# Identity Operators


```python
a = [10, 20, 30]
b = [10, 20, 30]
x = b
z = a
#is operator
x is a
#this will return false
x is z
a is b
```




    False



## Assignment 2

Identify the use and examples of these Operators in Python 

Membership Operators

Identity Operators

Bitwise Operators

# Control Statements 

Syntax


```python
if (test_expresson):
    #statement to be executed
    elif(test_expression 2):
        #statement of elif block
        else:
            #final statement
```


```python
x = 10
if x % 2 == 0:
  print('even number')
elif x % 2 == 1:
  print('odd number')
else:
  print('enter a number')
```

    even number
    


```python
x = 9
for i in range (2,x):
 if i % 2 == 0:
    print('not a prime number')
 else:
    print ('prime number')
```

    not a prime number
    prime number
    not a prime number
    prime number
    not a prime number
    prime number
    not a prime number
    

# Introduction to Python Fucntions

## Types of Functions in Python

1. Built-in Functions

2. Recursion Functions

3. Lambda Functions

4. User-defined Functions

## Python Built-in Functions

### Pyhton abs() Function

Syntax

abs(num)


```python
#random integer
integer = -20
print('Absolute value of -20 is', abs(integer))
```

    Absolute value of -20 is 20
    


```python
#random floating
floating = -30.33
print('Absolute value of -30.33 is:', abs(floating))
```

    Absolute value of -30.33 is: 30.33
    

### Python all() Function

Syntax

all(iterable)


```python
l = [1,2,3,4,5]
print(all(l))
```

    True
    


```python
l = [0, False]
print(all(l))
```

    False
    

#### Assignment on Python Functions

ascii()

bin()

compile()

dict()

enumerate()

eval()

...........find more functions Built in Functions

# Classes and Objects 


```python
#Syntax
class Class_name:
    statement_1
    .
    .
    statement_N
```


```python
class employee:
    pass
# no attributes and methods
emp_1 = employee()
emp_2 = employee()
#instance variable can be created manually
emp_1.first = 'Bonface'
emp_1.last = 'Osindi'
emp_1.email = 'bonfaceosindi@gmail.com'
emp_1.pay = 10000

emp_2.first = 'Esther'
emp_2.last = 'Mwau'
emp_2.email = 'esthermwau@gmail.com'
emp_2.pay  = 10000

print(emp_1.email)
print(emp_2.email)

print(emp_1.last)
```

    bonfaceosindi@gmail.com
    esthermwau@gmail.com
    Osindi
    


```python
class employee:
    def _init_(self, first, last, sal):
        self.fname = first
        self.lname = last
        self.sal = sal
        self.email = first + '.' + last + '@company.com'
        


```


```python
class MyClass:
 def func(self):
  print('Hello Cyber Crafts Academy')

```
