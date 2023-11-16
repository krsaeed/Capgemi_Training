# Loops in Python (for and while)

## Introduction

Loops are a fundamental concept in programming, and they allow you to perform repetitive tasks efficiently. In Python, there are two primary types of loops: "for" and "while."

## For Loop

The "for" loop is used to iterate over a sequence (such as a list, tuple, string, or range) and execute a set of statements for each item in the sequence. The loop continues until all items in the sequence have been processed.

**Syntax:**

```python
for variable in sequence:
    # Code to be executed for each item in the sequence
```
for iterator_var in sequence:
    statements(s)

**Example:**

```python
fruits = ["apple", "banana", "cherry"]
for fruit in fruits:
    print(fruit)
```

**Output:**

```
apple
banana
cherry
```

In this example, the loop iterates over the "fruits" list, and in each iteration, the "fruit" variable takes on the value of the current item in the list.


# Python program to illustrate
# Iterating over range 0 to n-1

n = 4
for i in range(0, n):
	print(i)

Example with List, Tuple, string, and dictionary iteration using For Loops in Python
We can use for loop to iterate lists, tuples, strings and dictionaries in Python.


# Python program to illustrate
# Iterating over a list
print("List Iteration")
l = ["geeks", "for", "geeks"]
for i in l:
	print(i)

# Iterating over a tuple (immutable)
print("\nTuple Iteration")
t = ("geeks", "for", "geeks")
for i in t:
	print(i)

# Iterating over a String
print("\nString Iteration")
s = "Geeks"
for i in s:
	print(i)

# Iterating over dictionary
print("\nDictionary Iteration")
d = dict()
d['xyz'] = 123
d['abc'] = 345
for i in d:
	print("%s %d" % (i, d[i]))

# Iterating over a set
print("\nSet Iteration")
set1 = {1, 2, 3, 4, 5, 6}
for i in set1:
	print(i),

#### While Loop

The "while" loop continues to execute a block of code as long as a specified condition is true. It's often used when you don't know in advance how many times the loop should run.

**Syntax:**

```python
while condition:
    # Code to be executed as long as the condition is true
```

**Example:**

```python
count = 0
while count < 5:
    print(count)
    count += 1
```

**Output:**

```
0
1
2
3
4
```

In this example, the "while" loop continues to execute as long as the "count" is less than 5. The "count" variable is incremented in each iteration.

while expression:
    statement(s)

While…Else

while condition:
     # execute these statements
else:
     # execute these statements

# Python program to illustrate
# combining else with while
count = 0
while (count < 3):
	count = count + 1
	print("Hello Geek")
else:
	print("In Else Block")

Nested Loops
Python programming language allows to use one loop inside another loop. Following section shows few examples to illustrate the concept. 
for iterator_var in sequence:
   for iterator_var in sequence:
       statements(s)
   statements(s)





# Python program to illustrate
# nested for loops in Python
from __future__ import print_function
for i in range(1, 5):
	for j in range(i):
		print(i, end=' ')
	print()
