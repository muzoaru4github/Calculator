Software Engineering Graduate Course


Check list:

Open new repository on git …

Make sure that actions button is pressed to log commits

ensure there is a articulated description and link to your implementation of the design patterns you use


Add short Explanation of Exponential function (calculation command) and Modulus function (calculation command for returning the remainder of the divided variables) in description 

You need to explain and link to how you are using logging .

You need to link to and explain how you are using try/catch / exceptions to illustrate "Look Before You Leap" (LBYL) and "Easier to Ask for Forgiveness than Permission" (EAFP)

Certainly! Let's break down the two programming paradigms, "Look Before You Leap" (LBYL) and "Easier to Ask for Forgiveness than Permission" (EAFP), and how they relate to using try/catch or exceptions in code.

### Look Before You Leap (LBYL)
- **Concept**: LBYL is a programming style where you check for potential issues before performing an operation.
- **Example**: Before performing a division, you check if the divisor is zero to avoid an error.
- **Code Illustration**:

```python
def safe_modulus(x, y):
    # LBYL: Check if y is zero before performing the modulus operation
    if y == 0:
        return "Error: Modulus by zero is not allowed."
    return x % y
```

In the `safe_modulus` function above, we use an `if` statement to check if `y` is zero before performing the modulus operation. This avoids the risk of an error.

### Easier to Ask for Forgiveness than Permission (EAFP)
- **Concept**: EAFP is a programming style where you perform an operation directly and handle exceptions if something goes wrong.
- **Example**: You try to perform a division and catch any errors that occur due to division by zero.
- **Code Illustration**:

```python
def safe_modulus_eafp(x, y):
    try:
        # EAFP: Try performing the modulus operation directly
        return x % y
    except ZeroDivisionError:
        # Handle the exception if y is zero
        return "Error: Modulus by zero is not allowed."
```

In the `safe_modulus_eafp` function, we use a `try` block to perform the modulus operation directly. If `y` is zero, a `ZeroDivisionError` is raised, which we catch in the `except` block and handle appropriately.

### Summary
- **LBYL** checks conditions before performing operations to avoid exceptions.
- **EAFP** assumes the operation will succeed and catches exceptions if they occur.

Both paradigms have their use cases. LBYL can be more readable and avoid the cost of handling exceptions, but it may result in more checks. EAFP can lead to cleaner and more straightforward code, especially in cases where errors are expected to be rare and the cost of handling exceptions is low.

Add readme.md file and add 3-5 min video demonstration of using the calculator and running commands (producing calculations)

Submit a link to your repository to Canvas.

Keep your repository private while working on it, so people don't copy your work. Make the repository public within a day of the project being due, so we can grade it.

Reminder keep GitHub actions open
