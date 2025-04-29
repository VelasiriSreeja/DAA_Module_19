# EX 1D Linear search
## DATE:29.04.25
## AIM:
To write a a python program to implement the quick sort using recursion.

## Algorithm
```
Step 1: Start 
Step 2: Select a pivot element from the list
Step 3: Partition the list into two sublists: elements less than pivot and elements greater than pivot
Step 4: Recursively apply quick sort to both sublists
Step 5: Combine the sorted sublists and pivot to get the final sorted list, then Stop
```
## Program:
```
/*
Program to implement a search function with parameter list name and the value to be searched using string values.
Developed by: sreeja.v
Register Number: 212222230169
*/
def search(a,n):
    for i in range(len(a)):
        if(a[i]==n):
            return True
    return False

n1=int(input())
a=[]
for i in range(n1):
    element=int(input())
    a.append(element)
tuple(a)
n=int(input())

if(search(a,n))==True:
    print("Tuple: {} found".format(n))
else:
    print("Tuple: {} not found".format(n))
```

## Output:
![Screenshot 2025-04-29 134300](https://github.com/user-attachments/assets/c67cfd16-51b1-4a3c-b46e-ae9fb9535d65)



## Result:
The program to implement the quick sort was executed successfully
