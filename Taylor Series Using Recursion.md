# 📐 Taylor Series Using Recursion in Python

## 🎯 AIM:
To write a Python program to evaluate a **Taylor Series** using **recursion**, where values of `x` and `n` are taken from the user.

## 🧠 ALGORITHM:

1. **Start**
2. Create variables `x` and `n`
3. Get values for `x` and `n` from the user
4. Define a recursive function `series(x, n)`
   - **Base case:** If `n == 0`, return 1
   - **Recursive case:** Return `x**n / n + series(x, n-1)`
5. Print the result
6. **Stop**

## 💻 PROGRAM:
```
def series(x, n):
    if n == 0:
        return 1
    return (x**n) / factorial(n) + series(x, n - 1)

def factorial(k):
    if k == 0:
        return 1
    return k * factorial(k - 1)

x = float(input("Enter the value of x: "))
n = int(input("Enter the number of terms (n): "))

result = series(x, n)
print("Result of the Taylor series:", result)

```
## OUTPUT
![image](https://github.com/user-attachments/assets/ba33793e-369b-42d0-8f39-ed8b1f94f7e0)

## RESULT
Therefore the given Python program has been executed successfully and the output has been verified.
