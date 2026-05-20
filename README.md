# ⚠️ Python Exception Handling

Simple and visual explanation of Exception Handling in Python with examples and outputs.

---

# 📘 What is Exception Handling?

Exception Handling is used to handle runtime errors in a program without crashing the application.

It makes programs:
- Safer
- More user-friendly
- Easier to debug

---

# 🔹 Common Exceptions in Python

| Exception | Meaning |
|-----------|----------|
| ZeroDivisionError | Dividing by zero |
| ValueError | Invalid value |
| IndexError | Invalid index |
| TypeError | Wrong data type |
| FileNotFoundError | File does not exist |

---

# 🔹 try and except

## Example

```python
try:
    num = 10 / 0
except ZeroDivisionError:
    print("Cannot divide by zero")
Output
Python
Cannot divide by zero
  🔹 finally Block
The finally block always executes.
Example
Python
try:
    print("Inside try block")
except:
    print("Error")
finally:
    print("Execution completed")
Output
Python
Inside try block
Execution completed
🔹 Multiple Exceptions
Example
Python
try:
    num = int(input("Enter number: "))
    result = 10 / num
except ValueError:
    print("Invalid input")
except ZeroDivisionError:
    print("Cannot divide by zero")
