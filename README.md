# Python Genius

A cheat sheet for Python programmers.

## Math Operators

`+` is for addition (`3 + 2 = 5`).

`-` is for subtraction (`3 - 2 = 1`).

`*` is for multiplication (`3 * 2 = 6`).

`/` is for division (`3 / 2 = 1.5`).

`//` is for integer division (`3 // 2 = 1`).

`**` is for exponentiation (`3 ** 2 = 9`).

`%` is for calculating remainders (`3 % 2 = 1`).

## Built-In Data Types

### Text Types
`str` is a string (`'you', 'know', 'python', '3', '!'`).

### Numeric Types
`int` is an integer (`... -3, -2, -1, 0, 1, 2, 3 ...`).

`float` is a floating-point number (`... -1.0, -0.5, 0, 0.5, 1.0 ...`).

`complex` is a complex number (`a + bi`).

### Sequence Types
`list` is a list of objects (`[1, '2', 3.0, 'four']`).  Lists are mutable.

`tuple` is a tuple of objects (`(1, '2', 3.0, 'four')`).  Tuples are immutable.

`range` is a range (`range(10)`).

### Mapping Types
`dict` is a dictionary (`{'key': 'value'}`).

### Set Types
`set` is a set of objects (`{1, 2, 3}`).  Sets are mutable.

`frozenset` is a set of objects (`frozenset(1, 2, 3)`).  Frozen sets are immutable.

### Boolean Type
`bool` is a boolean value (`true` or `false`).

### Binary Types
`bytes` are byte objects (`b'test "this" out'`).  Only ASCII characters are allowed.  Bytes are immutable.

`bytearray` is a bytearray object(`bytearray(10)`).  Byte arrays are mutable.

`memoryview` is a memoryview object (`memoryview(b'abcde')`).

## Variable Assignment

Variables can be assigned using an equals sign (`x = 'some value'`).

Variable reassignment is done by assigning a new value to an existing variable (`x = 'some new value'`).

Chained variable assignment is also possible (`x = y = z = 'same value'`).

## Conditional Statements

Conditional logic allows for decision making.  Python uses the `if`, `elif`, and `else` operators for this.

`if` tests if a logical statement evaluates to true.  If it does, the code inside the `if` block is executed.  

If not, the next `elif` block will be executed, if one exists.

If the `if` and all `elif` statements evaluate to false, the `else` block will be executed, if one exists.

```
number = 5

if number < 0:
    print('the number is negative')
elif number % 2 == 0:
    print('the number is even')
else:
    print('the number is odd')
```

## Loops

Python has two loop commands: `for` and `while`.

`for` loops are used for iterating over a sequence.
```
for i in range(10):
    print(i)
```
`while` loops are used for iterating as long as a condition is true.
```
i = ['foo', 'bar', 'baz']
while i:
    i.pop(-1)
```

`break` allows you to exit a loop.

`continue` allows you to skip over an iteration in a loop.

`pass` is a null statement that can be used as a placeholder for loops and functions.

## Functions

Functions are a block of reusable code designed to carry out a particular task.  

Functions make your code more modular and readable.

The `def` statement is used to define a function.
```
def func():
    pass
```

Functions can be called using the function name followed by parenthesis.
```
func()
```

Functions are assignable.
```
x = func()
```
Functions can be created to accept arguments by adding the argument name(s) in the parenthesis after the function definition.
```
def func(some_argument):
    pass
```

There is no limit to the number of arguments you can define as part of a function.

Functions support several types of arguments including:

* Keyword arguments (`def func(this)`).
* Keyword arguments with defaults (`def func(that="this")`).
* Arbitrary arguments (`def func(*args)`).
 * Arbitrary keyword arguments (`def func(**kwargs)`).

Any combination of these types of arguments can be used, but must be in the order above.
```
def func(this, that="this", *args, **kwargs)
```