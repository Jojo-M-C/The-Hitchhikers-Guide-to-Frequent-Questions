Basic and Complex Data Types
==========

Integer, Float
---------

An **integer** is a positive or negative number
without floating point (e.g. 3). 

A **float** is a
positive or negative number with floating point
precision (e.g. 3.14159265359).

The ‘//’ operator performs integer division.
The result is an integer value that is rounded
toward the smaller integer number
(e.g. 3 // 2 == 1).

.. code-block:: python
    x, y = 3, 2
    print(x + y) # = 5
    print(x - y) # = 1
    print(x * y) # = 6
    print(x / y) # = 1.5
    print(x // y) # = 1
    print(x % y) # = 1s
    print(-x) # = -3
    print(abs(-x)) # = 3
    print(int(3.9)) # = 3
    print(float(3)) # = 3.0
    print(x ** y) # = 9


String
-------

Python Strings are sequences of characters.
The four main ways to create strings are the
following.

1. Single quotes

``'Yes'``

2. Double quotes

``"Yes"``

3. Triple quotes (multi-line)

``"""Yes
We Can"""
``
4. String method

``str(5) == '5' # True``

5. Concatenation

``"Ma" + "hatma" # 'Mahatma'``

These are whitespace characters in strings.

- Newline ``\n``
- Space ``\s``
- Tab ``\t``

.. code-block:: python

    # 4. Indexing and Slicing
    s = "The youngest pope was 11 years old"
    print(s[0]) # 'T'
    print(s[1:3]) # 'he'
    print(s[-3:-1]) # 'ol'
    print(s[-3:]) # 'old'
    x = s.split() # creates string array of words
    print(x[-3] + " " + x[-1] + " " + x[2] + "s")
    # '11 old popes'
    
    ## 5. Most Important String Methods
    y = " This is lazy\t\n "
    print(y.strip()) # Remove Whitespace: 'This is lazy'
    print("DrDre".lower()) # Lowercase: 'drdre'
    print("attention".upper()) # Uppercase: 'ATTENTION'
    print("smartphone".startswith("smart")) # True
    print("smartphone".endswith("phone")) # True
    print("another".find("other")) # Match index: 2
    print("cheat".replace("ch", "m")) # 'meat'
    print(','.join(["F", "B", "I"])) # 'F,B,I'
    print(len("Rumpelstiltskin")) # String length: 15
    print("ear" in "earth") # Contains: True

