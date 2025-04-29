# EX 1A Reverse a String
## DATE:29.04.25
## AIM:
To write a program to  print factorial of a number recursively.



## Algorithm:
```
Step 1: Start the program
Step 2: Read the number `n` from the user
Step 3: Define a recursive function `factorial(n)`
        - If n is 0 or 1, return 1
        - Else return n * factorial(n - 1)
Step 4: Call the function with the given number and store the result
Step 5: Print the result and Stop
```

## Program:
```
/*
Program to implement Reverse a String
Developed by: sreeja.v
Register Number:  212222230169
*/
def factorial(n):
    if n == 0 or n == 1:
        return 1
    else:
        return n * factorial(n - 1)
num = int(input(""))

if num < 0:
    print("Factorial is not defined for negative numbers.")
else:
    result = factorial(num)
    print(f"Factorial of number {num} = {result}")

```


## Output:

![Screenshot 2025-04-29 133158](https://github.com/user-attachments/assets/7ace2b0c-7c5b-4fde-890f-50524fa01708)



## Result:
The program successfully print the factorial of the number recursively.
