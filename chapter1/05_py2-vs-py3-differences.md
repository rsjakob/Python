# Python 2 and 3 Differences

Python 2 and 3 are similar but **NOT COMPATIBLE! **Python 3 does break compatibility. We will be focusing on Python 2.7.13 but will cover 3.6.X along side the entire course.

## Print

Python 3 replaced Python 2's print statement with a print function\(\). While Python 2 will be happy as is or with parantheses... Python 3 will throw an error if the parantheses are not included.

#### Python 2

```py
print 'Hello World!' # outputs: Hello World!
mystr = 'Goodbye World!'

print mystr # outputs: Goodbye World!
print("This works too") # This works too!
```

#### Python 3

```py
print("Hello World!") # Hello World!
mystr = 'Goodbye World!'

print(mystr) # Goodbye World!
```

## Integer Division

Python 2 treats numbers without a decimal as integers, whereas Python 3 will treat them as float if it applies. Python 2 Division with integers truncate the remainder! Setting one number as a real number will yield the correct result.

#### Python 2

```py
print 3/2 # 1
print 3.0/2 # 1.5
```

#### Python 3

```py
print 3/2 # 1.5
```

## Other Major Differences

#### Unicode:

Python 2 has ASCII **str\(\) **type, separate **unicode\(\) **type.. but no **byte** type.

Python 3 has Unicode \(**utf-8\)** **str -**ings and two byte classes: **byte and bytearray. **

We will cover both in later lectures.

#### Input\(\) vs raw\_input\(\):

* Python 3 **input\(\)** always stores userinput as **str **objects. This is good.
* Python 2 **input\(\)** on the other hand fully evaluates the code the user gives it. **This is dangerous! **This gives the full power of Python to the user... and can be used in a malicious way. Instead, we use **raw\_input\(\) **in Python 2... which converts user input to a string. 

There are more differences between the two major releases. It's encouraged to look up the differences for better understanding.

