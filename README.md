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
Developed by:ARHAM S
RegisterNumber: 212222110005
'''
def linear_search(list1,n,key):
    for i in range(0,n):
      if(list1[i]==key):
        return i
    return -1

  
list1 =eval(input())
key =eval(input())
n =len(list1)
list1.sort()
result = linear_search(list1,n,key)
if(result==-1):
   print(list1)
   print("Element not found")
else:
  print(list1)
  print("Element found at index: ",result)




```
ii)	# Find the element in a list using Binary Search(Iterative Method).
```
''' 
Program to find the element in a list using Binary Search(Iterative Method)..
Developed by:ARHAM S
RegisterNumber:212222110005
'''
def binarySearch(array, k, low, high):
    while low<=high:
        mid = low + (high-low)//2
        if array[mid] ==k:
            return mid
        elif array[mid] < k:
            low = mid +1
        else:
            high = mid -1
    return -1



array = eval(input())
k = eval(input())
length = len(array)
low = 0
high = length-1
array.sort()
result = binarySearch(array,k,low,high)
if(result==-1):
    print(array)
    print("Element not found")
else:
    print(array)
    print('Element found at index: ',result)




```
iii)	# Find the element in a list using Binary Search (recursive Method).
```
''' 
Program to find the element in a list using Binary Search(Iterative Method)..
Developed by:ARHAM S
RegisterNumber:212222110005
'''
def binarySearch(array, k, low, high):
    while low<=high:
        mid = low + (high-low)//2
        if array[mid] ==k:
            return mid
        elif array[mid] < k:
            low = mid +1
        else:
            high = mid -1
    return -1



array = eval(input())
k = eval(input())
length = len(array)
low = 0
high = length-1
array.sort()
result = binarySearch(array,k,low,high)
if(result==-1):
    print(array)
    print("Element not found")
else:
    print(array)
    print('Element found at index: ',result)




```
## Sample Input and Output:
![exp3 1](https://github.com/arhamshajahan/Search-Algorithm/assets/127313881/51777f51-a6d5-4671-9ff6-b919c2314373)
![exp3 2](https://github.com/arhamshajahan/Search-Algorithm/assets/127313881/2709b429-4698-43ad-8a19-62444ad8190d)
![exp3 3](https://github.com/arhamshajahan/Search-Algorithm/assets/127313881/35f0ab13-2731-4cd7-9006-bb2e5f539a0a)







## Result
Thus the linear search and binary search algorithm is implemented using python programming.
