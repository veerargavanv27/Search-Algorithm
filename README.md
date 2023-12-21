# Linear Search and Binary search
## Aim:
To write a program to perform linear search and binary search using python programming.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
## Linear Search:
1.	Start from the leftmost element of array[] and compare k with each element of array[] one by one.
2.	If k matches with an element in array[] , return the index.
3.	If k doesn’t match with any of elements in array[], return -1 or element not found.
## Binary Search:
1.	Set two pointers low and high at the lowest and the highest positions respectively.
2.	Find the middle element mid of the array ie. arr[(low + high)/2]
3.	If x == mid, then return mid.Else, compare the element to be searched with m.
4.	If x > mid, compare x with the middle element of the elements on the right side of mid. This is done by setting low to low = mid + 1.
5.	Else, compare x with the middle element of the elements on the left side of mid. This is done by setting high to high = mid - 1.
6.	Repeat steps 2 to 5 until low meets high
## Program:
i)	#Use a linear search method to match the item in a list.
```
''' 
Program for linear search method to match the item in a list
Developed by:VEERARAGAVAN V
RegisterNumber: 23004739
'''
def linearSearch(array,n,k):
   # Write your code here for binary search using recursive method
    for i in range(0,n):
        if(array[i]==k):
            return i
    return -1
array = eval(input())
#sort the array
k = eval(input()) 
n=len(array)
array.sort()
print(array)
result=linearSearch(array,n,k)
if result != -1:
    print("Element found at index: ",result)
else:
    print("Element not found")
```
ii)	# Find the element in a list using Binary Search(Iterative Method).
```
''' 
Program to find the element in a list using Binary Search(Iterative Method)..
Developed by:VEERARAGAVAN V
RegisterNumber: 23004739
'''
def binarySearchIter(array, k, low, high):
    # Write your code here to find the middle value and check if the desired item is above or below the middle value
    while low<=high:
        mid=(low+high)//2
        if array[mid]==k:
            return mid
        elif array[mid]<k:
            low=mid+1
        else:
            high=mid-1
    return -1
    
array = eval(input())
array.sort()
# sort the array
k = eval(input()) #k-item to be searched
result=binarySearchIter(array, k,0,len(array)-1)
print(array)
if result != -1:
    print('Element found at index: ',result)
else:
    print("Element not found")
```
iii)	# Find the element in a list using Binary Search (recursive Method).
```
''' 
Program to find the element in a list using Binary Search(Iterative Method)..
Developed by:VEERARAGAVAN V
RegisterNumber: 23004739
'''
def binarySearchIter(array, k, low, high):
    # Write your code here to find the middle value and check if the desired item is above or below the middle value
    while low<=high:
        mid=(low+high)//2
        if array[mid]==k:
            return mid
        elif array[mid]<k:
            low=mid+1
        else:
            high=mid-1
    return -1
    
array = eval(input())
array.sort()
# sort the array
k = eval(input()) #k-item to be searched
result=binarySearchIter(array, k,0,len(array)-1)
print(array)
if result != -1:
    print('Element found at index: ',result)
else:
    print("Element not found")
```
## Output
![Screenshot 2023-12-21 232008](https://github.com/veerargavanv27/Search-Algorithm/assets/138955645/351759a9-7097-4b3b-b9a9-6521f602801d)
![Screenshot 2023-12-21 232033](https://github.com/veerargavanv27/Search-Algorithm/assets/138955645/f68d3691-113b-433b-8535-d69c5fc1a75c)
![Screenshot 2023-12-21 232047](https://github.com/veerargavanv27/Search-Algorithm/assets/138955645/4076b856-2b81-47ea-b3c2-fe640b227e7b)



## Result
Thus the linear search and binary search algorithm is implemented using python programming.
