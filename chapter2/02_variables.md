# Variables

## EVERYTHING IN PYTHON IS AN OBJECT!

This is the single, most important thing I can teach you. The sooner you have an understanding of Object Oriented Programming, the quicker everything else falls into place.

Data types are dynamic based on the variable stored. To check type, use:

#### **type\(**var**\)**

```py
x = 10
type(x)
#output: <class 'int'>
```

Notice the output is &lt;**class** 'int'&gt;... once again, everything in Python is an object!

Multiple assignment is allowed and types can be the same or different:

```py
a = b = c = 100
c = 200 # will only reassign variable c
print 'a = {} b = {} c = {}'.format(a, b, c)
#output: a = 100 b = 100 c = 200

a,b,c = 100, 'hello', {} # will change all three variables
print 'a = {} b = {} c = {}'.format(a, b, c)
#output: a = 100 b = hello c = {}
```

## Data Types

* **Numbers**
* **Strings**
* **Lists**
  * Think array
* **Tuples**
  * Think constant array
* **Dictionaries**
  * Think associative array

### Data Types: Immutable

**Immutable objects** are those that can't be changed without reassigning. Such as int or str. **Mutable objects** are those that can be changed. Such as list or dict. Below is a table with all types and their mutability.

![](/assets/Screen Shot 2017-09-27 at 12.54.54 PM.png)

# LAB 2A: Variable Types

Find the type of the following variables. Feel free to experiement with other variables and such.

**Type of:​**

* 10​

* 10.5​

* "10"​

* "Hello!"​

* ""​

* True​

* 0​

* type​

* object​

* b"10101101"  \*\*Try in Py2 and Py3 ​

* 0b10101101​

* \[1,2,3\]​

* \(1,2,3\)​

* {1,2,3}​

* {'one':1}​

* 5j​



