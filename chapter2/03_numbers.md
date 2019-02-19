# Numbers

### Prefixes

Prefixes convert types like **binary, hex and octal **into int.

* No prefix for decimal​

* Prefix with 0b, B for binary \(ex. 0b10 == 2\)​

* Prefix with 0x, X for hex \(ex. 0xF == 15\)​

* Prefix with 0o, O for octal \(ex. 0o100 == 64\)​

![](/assets/Screen Shot 2017-09-27 at 1.09.39 PM.png)

## Types

* int \(integer\)
  * Equivalent to C-Longs in Python 2 and non-limited in Python 3
* Long

  * Long integers of non-limited length. Exist only in Python 2

* Float \(decimal, hex, octal\)

  * Floating point numbers. Equivalent to C-Doubles

* Complex

  * Complex numbers, ex:

  ```py
  x = 1.5 + j
  y = 2
  z = x + y
  print z
  #Output: (3.5+5j)
  ```

### Numbers are IMMUTABLE!

Numbers cannot be modified in place. Be sure to either reassign your current variable or assign the number to a new variable.

![](/assets/Screen Shot 2017-09-28 at 2.00.11 PM.png)

## Bool \(True or False\)

Bools are a subclass of int. This was done around Python 2.2 to allow previous implementations of bools \(0 and 1\) to continue working… especially so with C code that utilizes Pylint\_Check\(\)

#### Truth Value Testing

* The following will evaluate to False:

  * False
  * zero numeric type- 0 0.0 0
  * None
  * empty sequence – ‘’ \(\) \[\]
  * empty mapping- {}
  * instances of user defined classes \(will get into later\)​

* The following will evaluate to True: Everything else, not limited to but including–

  * True, 1

  * any number that is less than or greater than 0... but not 0

  * non-empty sequence/mapping, etc

## Operators

There are some differences between Python and many other languages that need to be brought to light. Increment operators **\(x++, y--, etc\) **do not exist in Python. To increment in Python, **you can use shorthand: a += 1, x -= 5, z \*= 2, etc**

| Operator | Description | Example | Result |
| :--- | :--- | :--- | :--- |
| + | Addition | 4 + 5 | 9 |
| - | Subtraction | 10 - 5 | 5 |
| \* | Multiplication | 4 \* 2 | 8 |
| / | Division\* | 3 / 2 | Py2\(1\) Py3\(1.5\) |
| // | Floor Division | 3.0 // 1.0 | 1 \(~int division\) |
| % | Modulus \(remainder\) | 4 % 2 | 0 |
| \*\* | Exponentiation | 4 \*\* 2 | 16 |

**\*3.0 / 2 will return 1.5 for both Python 2 and Python 3**

### Order of Operations

| Operation | Precedence | Extra |
| :--- | :--- | :--- |
| \(\) | 1 | Anything in brackets is first |
| \*\* | 2 | Exponentiation |
| -x, +x | 3 |  |
| \*, /, %, // | 4 | Will evaluate left to right |
| +, - | 5 | Will Evaluate left to right |
| &lt;, &gt;, &lt;=, &gt;=, !=, == | 6 | Relational Operators |
| Logical Not | 7 |  |
| Logical And | 8 |  |
| Logical Or | 9 |  |

### Type Conversion

```py
int(‘x’, base) # Returns x as base integer​
float(x) # Returns x as float​
complex(real, imag) # Returns complex number​
chr(x) # Returns string of one character for x as ASCII​
ord(x) # Returns ASCII value for x as string of one char​
hex(x) # Returns x as hex​
oct(x) # Returns x as octal​
```

_There are some differences between Python 2 and Python 3 numbers. The biggest difference being the removal of the Long Type in Python 3._

# 

# Lab 2B and 2C

Download the following files and follow the instructions within.

* 2A: numbers.py
* 2B: tax\_calc.py



