# Closures, Iterators and Generators

## Closures

No. We aren't talking about the programming language Clojure. A Closure is a function object that remembers values in enclosing scopes regardless of whether those scopes are still present in memory. If you have written a function that returned another function, you probably have used closures without even knowing.

**Example:**

```py
def generate_power_func(n):
    def nth_powah(x):
        return x**n
    return nth_powah
print generate_power_func(10)

# What happens?
```

## Iterators

An iterator is just an object with a state that remembers where it is during iteration. Iterable objects can range from while loops to the actual iter object.

**Example of iter function:**

```py
>>> x = iter([1, 2, 3, 4, 5, 6])
>>> print x
<listiterator object at 0x02B2AB30>
x.next()
1
x.next()
2
x.next()
3
x.next()
4
x.next()
5
x.next()
6
x.next()
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
StopIteration
```

The one we will be using the most is the xrange\(\) function. Below is an iterator, implemented as a class that works like xrange. This is your first major look at classes... don't freak out! Let's break this down.

```py
class yrange:
    def __init__(self, n):
        self.i = 0
        self.n = n

    def __iter__(self):
        return self

    def next(self):
        if self.i < self.n:
            i = self.i
            self.i += 1
            return i
        else:
            raise StopIteration()
            
# using y range
yrange(3)
y.next()
0
y.next()
1
y.next()
2
y.next()
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
  File "<stdin>", line 14, in next
StopIteration
```

As we learned in the Data Types lecture... xrange\(\) loads one at a time. The yrange\(\) class here does the same thing. There is lists, tuples, etc loaded up. Instead, we deal with two variables... i and n. 
