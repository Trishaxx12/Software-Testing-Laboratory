# Ex.No: 1 Write programs in Python Language to demonstrate the working of followingconstructs with possible test cases: a) do…while b) while…do c) if …else d) switch e) for 

### DATE:                                                                            
### REGISTER NUMBER : 212221040173

### AIM:  
To write python programs for do…while, while, for, switch and if…else and test with possible test 
Cases 

### Algorithm:
1. Start the program.
2. Create separate files for each given program.
3. Write simple program for each construct.
4.  the program with possible test cases.
5. Stop the program.
### Program:
```
a) do....while
def display():
  start=input("Enter a positive value for START: ")
  end=input("Enter a positive value for END: ")
  if start.isnumeric() and end.isnumeric():
     while True:
      start=int(start)
      end=int(end)
      print(start,end=' ')
      if start<end:
         start+=1
      else:
        break
  else:
    print("Enter a valid positive number.")
display() 
b) while...do
start = input("Enter a positive value for START: ")
end = input("Enter a positive value for END: ")

if start.isnumeric() and end.isnumeric():
    start = int(start)
    end = int(end)
    while start <= end:
        print(start, end=" ")
        start += 1
else:
    print("Enter a valid positive number.")

c)if....else
def switch():
    switcher = {0: "even", 1: "odd"}
    n = input('Enter a value for N: ')
    try:
        n = int(n)
        print(switcher[n % 2])
    except ValueError:
        print("Enter a valid number.")

d)switch()
def compare():
    a = input("Enter a value for A: ")
    b = input("Enter a value for B: ")
    try:
        a = int(a)
        b = int(b)
        if a > b:
            print("A is greater than B")
        elif a < b:
            print("B is greater than A")
        else:
            print("A is equal to B")
    except ValueError:
        print("Enter a valid number.")

compare()
e)for
def iterate():
    string = input("Enter a string: ")
    for i in string:
        print(ord(i), end=" ")
    print()  

iterate()
```















### Output:
![Screenshot 2024-08-27 140223](https://github.com/user-attachments/assets/47001a2c-8e58-4b0f-8ab9-d450c7765b1a)
![Screenshot 2024-08-27 141358](https://github.com/user-attachments/assets/97c3356b-d64d-470f-99b0-9ddeebf215bd)
![Screenshot 2024-08-27 140223](https://github.com/user-attachments/assets/e619f36b-7d6d-41f3-8c54-bed98fb8c100)
![Screenshot 2024-08-27 135445](https://github.com/user-attachments/assets/0b0a2120-134d-455d-87d4-f5d5e4708a44)




### Result:
Thus, the python program to demonstrate the working of given constructs is implemented and the output is verified successfully.


