# EX 1B Merge Sort
## DATE:29.04.25
## AIM:
To write a python program for the implementation of merge sort on the given list of values.

## Algorithm
```
Step 1: Start
Step 2: If the list has more than one element, divide it into two halves
Step 3: Recursively sort both halves using Merge Sort
Step 4: Merge the two sorted halves by comparing elements from each half
Step 5: Stop after all elements are merged in sorted order
```  

## Program:
```
/*
Program to implement Merge Sort
Developed by: sreeja.v
Register Number:212222230169  
*/
def merge(l,r):
    i=j=0
    arr=[]
    while i<len(l) and j<len(r):
        if l[i]<r[j]:
            arr.append(l[i])
            i+=1
        else:
            arr.append(r[j])
            j+=1
    arr+=l[i:]+r[j:]            
    return arr    
def mergeSort(arr):
    if len(arr)<=1:
        return arr
    m = len(arr)//2
    l=mergeSort(arr[:m])
    r=mergeSort(arr[m:])
    return merge(l, r)
arr = []
n = int(input())
for i in range(n):
    arr.append(int(input()))
print("Given array is")
for i in range(n):
    print("%d" % arr[i],end=" ")
res=mergeSort(arr)
print("\nSorted array is")
for i in range(n):
    print("%d" % res[i],end=" ")

```

## Output:
![Screenshot 2025-04-29 133559](https://github.com/user-attachments/assets/98510e34-3be2-459e-88c0-197278605fc4)



## Result:
The program successfully sorts the given list of the values.
