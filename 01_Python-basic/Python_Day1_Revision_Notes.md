# Python Day 1 Revision Notes (AI Engineer Track)

## 1. What is Programming?

Programming is the process of writing instructions that a computer can
execute.

### Why Python?

-   Easy to learn
-   Used in AI, ML, Data Science, Web Development, Automation
-   Huge ecosystem of libraries
-   Industry standard for AI Engineers

------------------------------------------------------------------------

# 2. Variables and Data Types

``` python
name = "Priyesh"      # str
age = 21             # int
height = 5.9         # float
is_student = True    # bool
```

### Rules for Identifiers

✅ Can contain letters, numbers, underscore

✅ Cannot start with a number

❌ Cannot use keywords

Examples:

``` python
user_name = "Pri"
age2 = 21
```

------------------------------------------------------------------------

# 3. Python Keywords

Examples:

``` python
if
else
for
while
True
False
None
class
def
return
```

Keywords have special meaning and cannot be used as variable names.

------------------------------------------------------------------------

# 4. Input and Output

``` python
name = input("Enter name: ")
print(name)
```

### f-Strings

``` python
name = "Priyesh"
age = 21

print(f"My name is {name} and I am {age}")
```

------------------------------------------------------------------------

# 5. Operators

## Arithmetic

``` python
+  -  *  /  //  %  **
```

Example:

``` python
10 // 3
10 % 3
2 ** 3
```

## Comparison

``` python
==
!=
>
<
>=
<=
```

## Logical

``` python
and
or
not
```

## Assignment

``` python
=
+=
-=
*=
/=
```

## Membership

``` python
in
not in
```

## Identity

``` python
is
is not
```

## Bitwise

``` python
&
|
^
<<
>>
```

------------------------------------------------------------------------

# 6. Operator Precedence

Remember:

``` python
()
**
* / // %
+ -
Comparison
not
and
or
```

Example:

``` python
2 + 3 * 4 ** 2
```

------------------------------------------------------------------------

# 7. Type Casting

## Implicit

``` python
5 + 2.5
```

Python converts automatically.

## Explicit

``` python
int("10")
float("10")
str(10)
bool(1)
```

Common Interview Question:

``` python
int(45.8)
```

Output:

``` python
45
```

------------------------------------------------------------------------

# 8. Mutable vs Immutable

## Mutable

Can be changed after creation.

Examples:

``` python
list
dict
set
```

``` python
nums = [1,2,3]
nums[0] = 10
```

## Immutable

Cannot be changed after creation.

Examples:

``` python
int
float
bool
str
tuple
```

``` python
name = "Moon"
# name[0] = "P"
```

Raises error.

------------------------------------------------------------------------

# 9. Conditional Statements

## if

``` python
if age >= 18:
    print("Eligible")
```

## if-else

``` python
if age >= 18:
    print("Eligible")
else:
    print("Not Eligible")
```

## if-elif-else

``` python
if marks >= 90:
    print("A")
elif marks >= 75:
    print("B")
else:
    print("C")
```

## Ternary Operator

``` python
result = "Adult" if age >= 18 else "Minor"
```

------------------------------------------------------------------------

# 10. Loops

## for Loop

``` python
for i in range(5):
    print(i)
```

## while Loop

``` python
count = 0

while count < 5:
    print(count)
    count += 1
```

## break

``` python
break
```

Stops loop.

## continue

``` python
continue
```

Skips current iteration.

------------------------------------------------------------------------

# 11. Important Built-in Functions

``` python
print()
input()
len()
type()
range()
int()
float()
str()
bool()
sum()
max()
min()
```

------------------------------------------------------------------------

# 12. Python Collections (Very Important)

## List

``` python
nums = [1,2,3]
```

Mutable.

## Tuple

``` python
data = (1,2,3)
```

Immutable.

## Set

``` python
nums = {1,2,3}
```

Unique values only.

## Dictionary

``` python
student = {
    "name": "Priyesh",
    "age": 21
}
```

Key-value storage.

------------------------------------------------------------------------

# 13. Type Annotations (Important for AI Engineers)

``` python
name: str = "Priyesh"
age: int = 21
```

Functions:

``` python
def square(x: int) -> int:
    return x * x
```

Benefits: - Cleaner code - Better IDE support - Easier debugging -
Industry standard

------------------------------------------------------------------------

# 14. Common Beginner Mistakes

1.  Mixing int and str accidentally
2.  Forgetting indentation
3.  Using = instead of ==
4.  Infinite while loops
5.  Modifying immutable objects
6.  Ignoring error messages

------------------------------------------------------------------------

# 15. Mini AI Engineer Checklist

You should be able to:

-   Create variables
-   Use all basic data types
-   Take input and print output
-   Use operators correctly
-   Convert data types
-   Write if-else statements
-   Write for and while loops
-   Understand mutability
-   Use lists and dictionaries
-   Read simple error messages
-   Write type annotations

If you can solve the assessment notebooks comfortably, you are ready
for: - Functions - Strings - Lists - Dictionaries - Basic Problem
Solving
