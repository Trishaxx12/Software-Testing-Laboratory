### AIM: 
Write a python program to check the number is Armstrong number or not and inspect for failures.

### Algorithm:

1.  Start the program.
2.	Read an integer input number.
3.	Initialize the variables current_digit, sum = 0, and num = number.
4.	Repeat Steps 5 to 7 until num > 0
5.	current_digit = (num % 10).
6.	sum = sum + (current_digit * current_digit * current_digit). 7. Stop the program.
7.	num = num / 10.
8.	Check if sum == number. If true, print "It is an Armstrong Number." Otherwise, print "It is not an Armstrong Number."
9.	Stop the program.

### Program:
```
def binary_search(arr, x):
    low = 0
    high = len(arr) - 1

    while low <= high:
        mid = (high + low) // 2

        if arr[mid] < x:
            low = mid + 1
        elif arr[mid] > x:
            high = mid - 1
        else:
            return mid  # Return the index of the found element

    return -1  # Return -1 if the element is not found

arr = [2, 3, 4, 10, 40]
x = input("Enter the element to be searched: ")

try:
    x = int(x)
    result = binary_search(arr, x)
    
    if result != -1:
        print("Element is present at index", str(result))
    else:
        print("Element is not present in array")
except ValueError:  # Catch specific exception for invalid input
    print("Enter a valid input!")
```













### Output:
![Screenshot (61)](https://github.com/user-attachments/assets/120c44ef-3837-404e-83bd-0f490b6669fe)



### Result:
Thus, the python program to check the number is Armstrong number or not implemented and the output is verified successfully.

