# Selection sort and Insertion sort

## Aim:
To write a program to perform selection sort and insertion sort using python programming.

## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm:

## Selection Sort Algorithm:

1.	Set the first unsorted element as the minimum

2.	For each of the unsorted elements, check if the element < current minimum.

3.	If yes, set the element as the new minimum.

4.	Swap minimum with first unsorted position.

5.	Repeat the steps 2 and 3 for all the elements in the array.

## Insertion Sort Algorithm:

1.	Set the first element as sorted element j.

2.	For each unsorted element X, check if current sorted element j >X.

3.	If yes, move sorted element to the right by 1.

4.	Break the loop and insert X.

5.	Repeat the steps 2 to 4 for sorting all the elements in the array.



## Program:

i)	Selection Sort

```
Program to sort the elements in the list using the Selection Sort algorithm.
Developed by:Maheswaran.K
Register Number: 212222110023

def selection_sort(nums):
    for i in range (len(nums)):
        low=i
        for j in  range(i+1,len(nums)):
            if nums[j]<nums[low]:
                low=j
        nums[i],nums[low]=nums[low],nums[i]
    print(nums)
list_of_nums = eval(input())
selection_sort(list_of_nums)

```

ii)	Insertion Sort

```
Program to sort the elements in the list using the Insertion Sort algorithm.
Developed by:Maheswaran.K
Register Number: 212222110023

def insertion_sort(nums):
    for i in range (1,len(nums)):
        insert=nums[i]
        j=i-1
        while j>=0 and nums[j]>insert:
            nums[j+1]=nums[j]
            j-=1
        nums[j+1]=insert
    print(nums)
list_of_nums = eval(input())
insertion_sort(list_of_nums)

```

## Output:

i)	Selection Sort

<img width="928" alt="Screenshot 2023-06-04 at 10 24 47 PM" src="https://github.com/MAHESWARAN2004/Sorting-Algorithm/assets/119478181/73c492d1-7be0-40d3-b206-f97815054e9d">

ii)	Insertion Sort

<img width="921" alt="Screenshot 2023-06-04 at 10 25 00 PM" src="https://github.com/MAHESWARAN2004/Sorting-Algorithm/assets/119478181/e8ee065c-38b2-431f-aa6c-717ffc1e42dd">


## Result:
Thus the program is written to perform selection sort and insertion sort using python programming.
