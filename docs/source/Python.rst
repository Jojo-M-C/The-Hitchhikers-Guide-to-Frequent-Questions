Python Keywords
=======

True, False
-------

Data values from the data type Boolean

.. code:: python
    False == (1 > 2), True == (2 > 1)

and, or, not
----

Logical operators:

(x and y) → both x and y must be True

(x or y) → either x or y must be True

(not x) → x must be false

.. code:: python
    x, y = True, False
    (x or y) == True # True
    (x and y) == False # True
    (not y) == True # True

break
-------

Ends loop prematurely 

.. code:: python
    while(True):
    break # no infinite loop
    print("hello world")

continue
----

Finishes current loop iteration 

.. code:: python
    while(True):
    continue
    print("43") # dead code

class
-----

Defines a new class → a real-world concept
(object oriented programming)

**def**

Defines a new function or class method. For latter,
first parameter (“self”) points to the class object.
When calling class method, first parameter is implicit.

.. code:: python
    class Beer:
        def __init__(self):
            self.content = 1.0
        def drink(self):
            self.content = 0.0
        becks = Beer() # constructor - create class
        becks.drink() # beer empty: b.content == 0


.. code-block :: js

    {
        "mnemonic": "repair derive axis lunch hockey air wealth market detail bicycle mixed shiver"
    }