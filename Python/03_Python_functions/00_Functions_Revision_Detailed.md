# 00_Functions_Revision

# Python Functions, Iterators, Generators, Lambda, Map, Filter & Reduce
## AI Engineer Day 3 Revision Notes

---

# 1. Functions

A function is a reusable block of code that performs a specific task.

Instead of writing the same code multiple times, we write it once inside a function and call it whenever needed.

## Syntax

```python
def greet():
    print("Hello")
```

Calling:

```python
greet()
```

---

## Why Functions Matter

- Reusability
- Cleaner code
- Easier debugging
- Better organization
- Industry standard

Bad:

```python
print("Hello Priyesh")
print("Hello Moon")
print("Hello World")
```

Better:

```python
def greet(name):
    print(f"Hello {name}")
```

---

# 2. Parameters vs Arguments

## Parameters

Variables defined in function definition.

```python
def add(a, b):
    return a + b
```

a and b are parameters.

## Arguments

Values passed during function call.

```python
add(2, 3)
```

2 and 3 are arguments.

---

# 3. Return vs Print

## print()

Displays output.

```python
print(5)
```

## return

Returns a value for future use.

```python
def add(a, b):
    return a + b
```

```python
result = add(2, 3)
```

### Interview Question

```python
print(add(2,3))
```

prints value.

```python
x = add(2,3)
```

stores value.

---

# 4. Default Arguments

Allows a parameter to have a default value.

```python
def greet(name="Guest"):
    return f"Hello {name}"
```

```python
greet()
```

Output:

```python
Hello Guest
```

---

# 5. Scope

## Local Variable

Exists only inside function.

```python
def test():
    x = 10
```

## Global Variable

Exists outside function.

```python
x = 10
```

---

# 6. *args

Used when number of arguments is unknown.

```python
def total(*args):
    return sum(args)
```

```python
total(1,2,3,4)
```

Output:

```python
10
```

Important:

```python
args
```

is stored as a tuple.

---

# 7. **kwargs

Used when number of keyword arguments is unknown.

```python
def profile(**kwargs):
    print(kwargs)
```

```python
profile(name="Priyesh", age=21)
```

Output:

```python
{'name': 'Priyesh', 'age': 21}
```

Important:

```python
kwargs
```

is stored as a dictionary.

---

# 8. Iterators

Iterator is an object that remembers its current position.

Functions:

```python
iter()
next()
```

Example:

```python
nums = [10,20,30]

it = iter(nums)

print(next(it))
```

Output:

```python
10
```

Next call:

```python
next(it)
```

Output:

```python
20
```

---

# 9. Iterable vs Iterator

## Iterable

Can be looped over.

Examples:

```python
list
tuple
set
dict
string
```

## Iterator

Created using:

```python
iter()
```

and accessed using:

```python
next()
```

---

# 10. Generators

Generator is a special function that uses:

```python
yield
```

instead of:

```python
return
```

Example:

```python
def count():
    yield 1
    yield 2
    yield 3
```

Usage:

```python
g = count()

next(g)
```

Output:

```python
1
```

---

# 11. yield vs return

return:

```python
return 5
```

Function ends immediately.

yield:

```python
yield 5
```

Function pauses and remembers state.

---

# 12. Why Generators Matter

Normal function:

```python
return [1,2,3,4,5]
```

Stores everything in memory.

Generator:

```python
yield
```

Creates values only when needed.

Benefits:

- Less memory
- Faster for huge datasets
- Used in ML pipelines
- Used in data streaming

---

# 13. Lambda Functions

Anonymous one-line functions.

Syntax:

```python
lambda arguments: expression
```

Example:

```python
square = lambda x: x*x
```

Usage:

```python
square(5)
```

Output:

```python
25
```

---

# 14. Lambda vs Normal Function

Normal:

```python
def square(x):
    return x*x
```

Lambda:

```python
lambda x: x*x
```

Use lambda for small operations.

---

# 15. map()

Transforms every element.

Example:

```python
nums = [1,2,3]

list(map(lambda x:x*x, nums))
```

Output:

```python
[1,4,9]
```

Think:

"Change every item."

---

# 16. filter()

Keeps matching elements.

Example:

```python
nums = [1,2,3,4,5,6]

list(filter(lambda x:x%2==0, nums))
```

Output:

```python
[2,4,6]
```

Think:

"Keep only matching items."

---

# 17. reduce()

Located in:

```python
from functools import reduce
```

Combines many values into one.

Example:

```python
reduce(lambda x,y:x+y,[1,2,3,4])
```

Output:

```python
10
```

Think:

"Many → One"

---

# 18. Quick Comparison

map()
- Transform items

filter()
- Select items

reduce()
- Combine items

---

# 19. AI Engineer Relevance

You will see these constantly in:

- NumPy
- Pandas
- Data Processing
- Machine Learning Pipelines
- Feature Engineering
- Data Cleaning

Especially:

- Functions
- Lambda
- Generators
- map/filter

---

# 20. Interview Questions

1. Difference between print and return?
2. Difference between args and kwargs?
3. Difference between iterable and iterator?
4. Difference between yield and return?
5. Why are generators memory efficient?
6. When should lambda be used?
7. Difference between map, filter and reduce?

If you understand everything in this file, you're ready for the Day 3 assessment notebooks.
