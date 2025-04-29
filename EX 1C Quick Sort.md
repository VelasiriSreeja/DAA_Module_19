# EX 1C Quick Sort
## DATE:29.04.25
## AIM:
To write a python program to implement the quick sort using recursion.

## Algorithm
```
Step 1: Start the program
Step 2: Select a pivot element from the list
Step 3: Partition the list into two sublists: elements less than pivot and elements greater than pivot
Step 4: Recursively apply quick sort to both sublists
Step 5: Combine the sorted sublists and pivot to get the final sorted list, then Stop
```   

## Program:
```
/*
Program to implement implement quick sort using the last element as pivot on the list of float values.
Developed by: sreeja.v
Register Number:  212222230169
*/
def partition(arr, low, high):
    pivot = arr[high]
    i = low - 1
    for j in range(low, high):
        if arr[j] <= pivot:
            i += 1
            arr[i], arr[j] = arr[j], arr[i]
    arr[i + 1], arr[high] = arr[high], arr[i + 1]
    return i + 1

def quick_sort(arr, low, high):
    if low < high:
        pi = partition(arr, low, high)
        print("pivot: ", arr[pi])
        quick_sort(arr, low, pi - 1)
        quick_sort(arr, pi + 1, high)

# Example usage:
if __name__ == "__main__":
    list1=[]
    n=int(input())
    for i in range(n):
        list1.append(int(input()))
    quick_sort(list1, 0, len(list1) - 1)
    print(list1)

    

```

## Output:

![Screenshot 2025-04-29 133855](https://github.com/user-attachments/assets/c64f084e-cdab-41e8-b372-a1ebd6666afc)



## Result:
The program successfully sorts the input array using the QuickSort algorithm.
