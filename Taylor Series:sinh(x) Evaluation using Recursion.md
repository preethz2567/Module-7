# 📐 Taylor Series:sinh(x) Evaluation using Recursion in Python

## 🎯 AIM:
To write a Python program to evaluate the value of **sinh(x)** for **n terms** using recursion.

---

## 🧠 ALGORITHM:

1. **Start**
2. Read input for variable `x` (angle or number)
3. Read input for variable `n` (number of terms)
4. Define a function `fact(n)`:
   - If `n <= 1`, return 1
   - Else, return `n * fact(n - 1)` (recursive factorial)
5. Define a function `sinh(x, n)`:
   - If `n == 0`, return `x`
   - Else, return `(pow(x, 2*n + 1) / fact(2*n + 1)) + sinh(x, n - 1)`
6. Call the `sinh(x, n)` function and print the result
7. **Stop**

---

## 💻 PROGRAM:
```
def fact(n):
    if n <= 1:
        return 1
    return n * fact(n - 1)

def sinh(x, n):
    if n == 0:
        return x
    return (pow(x, 2 * n + 1) / fact(2 * n + 1)) + sinh(x, n - 1)

x = float(input("Enter the value of x: "))
n = int(input("Enter the number of terms: "))

result = sinh(x, n)
print("sinh(x) using", n + 1, "terms is:", result)

```

## OUTPUT
![image](https://github.com/user-attachments/assets/fa807e37-3f6c-455b-be1c-5909f091d379)

## RESULT
Therefore the given Python program has been executed successfully and the output has been verified.
