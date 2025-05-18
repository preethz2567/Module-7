# PYTHON PROGRAMMING MODULE 07
## NAME : PREETHI D
## REGISTER NUMBER: 212224040250

# EX 01 -  Types of Recursion: Head Recursion in Python

##  AIM:
To write a Python program to demonstrate **Head Recursion** by finding and printing the sequence based on the sum of all digits (even or odd adjusted input).

##  ALGORITHM:

1. **Start**
2. Define a recursive function `fun(n)`
3. In the function:
   - Create a recursive call at the **beginning** (Head Recursion)
   - Print the result after the recursive call
4. Take input from the user
5. If input is odd, convert it to the next even number
6. Call the recursive function
7. **Stop**

##  PROGRAM:
```
def fun(n):
    if n > 0:
        fun(n - 2)
        print(n, end=' ')

num = int(input("Enter a number: "))
if num % 2 != 0:
    num += 1

fun(num)

```

## OUTPUT
![image](https://github.com/user-attachments/assets/2c4bf39a-cd4e-4923-86cd-6ffda7a50ebd)

## RESULT
Therefore the given Python program has been executed successfully and the output has been verified.

# EX 02 -  Recursion:Palindrome Checker Using Recursion in Python

##  AIM:
To write a Python program to check whether a given string is a **palindrome** using **recursion**.

---

##  ALGORITHM:

1. **Start**
2. Define a recursive function `is_palindrome(word)`
   - **Base Case:** If the string length is less than 1, return `True`
   - **Recursive Case:** If the first and last characters match, call the function recursively on the substring without first and last characters
   - Else, return `False`
3. Get input from the user
4. Call the recursive function
5. Print whether the string is a palindrome
6. **Stop**

---

##  PROGRAM:
```
def is_palindrome(word):
    if len(word) < 1:
        return True
    if word[0] == word[-1]:
        return is_palindrome(word[1:-1])
    return False

text = input("Enter a string: ")

if is_palindrome(text):
    print("The string is a palindrome.")
else:
    print("The string is not a palindrome.")

```
## OUTPUT
![image](https://github.com/user-attachments/assets/b9ff8dd7-eed1-4ae5-ab0e-b3368319a058)

## RESULT
Therefore the given Python program has been executed successfully and the output has been verified.
