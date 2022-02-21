# Bubble Sort

<img src="./img/bubbleimage.png" style="width:400px;" class="center"/>

## Table of Contents

- [Problem Statement](#problem-statement)
- [Python Code](#python-code)
- [Sample Output](#Sample-Output)
- [Replit Link](#replit-link)
- [PythonTutor Link](#pythontutor-link)


## Problem Statement

<div align="justify"> <p> A bubble sort compares pairs of adjacent elements and swaps those elements if they are not in order. It is commonly implemented in Python to sort lists of unsorted numbers. ... Starting from the first element in a list, a bubble sort will compare the first and second elements
  </div></p>

<img src="./img/bubbleimage.png" style="width:600px;" class="center"/>



## Python Code



```python
# This function takes last element as pivot, places
# the pivot element at its correct position in sorted
# array, and places all smaller (smaller than pivot)
# to left of pivot and all greater elements to right
# of pivot


def bubblesort(alist):
  print(alist)
  indexes = range(len(alist))
  for idx in indexes:
    for nidx in indexes[idx:]:
        if alist[idx] > alist[nidx]:
            alist[idx], alist[nidx] = alist[nidx], alist[idx]
        print("inter", alist)
  return alist


alist=list(map(int,(input("Enter the list of elements : ").split())))
sorted_list=bubblesort(alist)
print(f"Largest number in a list is : {sorted_list[-1]}")
```

## Sample Output
<img src="./img/bubblesorts.png" style="width:400px;" class="center"/>

## Replit Link
https://tinyurl.com/44fa4ums

## PythonTutor Link

https://tinyurl.com/yckju63n
