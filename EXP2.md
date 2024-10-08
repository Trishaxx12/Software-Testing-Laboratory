# Ex.No: 2   Matrix Multiplication 

### DATE:                                                                            
### REGISTER NUMBER : 212221040173

### AIM: 
Write a python program for matrix multiplication and inspect for failures.
 
### Algorithm:

Algorithm:
1. Start the program.
2. Create empty list formatrix1, matrix2 and result.
3. Get the rows and columns count from the user.
4. Get the values of two matrix.
5. Perform matrix multiplication and store the answer in result.
6. Stop the program.
### Program:
```
r1, c1 = input("Enter row and column count for matrix 1: ").split()
r2, c2 = input("Enter row and column count for matrix 2: ").split()

# Validate input
if not (r1.isnumeric() and c1.isnumeric() and r2.isnumeric() and c2.isnumeric()):
    print("Enter valid numbers")
else:
    r1, r2, c1, c2 = int(r1), int(r2), int(c1), int(c2)

    # Check multiplication possibility
    if c1 != r2 or max(r1, c1, r2, c2) > 20 or min(r1, c1, r2, c2) == 0:
        print("Matrix multiplication not possible")
    else:
        # Initialize matrices
        matrix1 = []
        matrix2 = []
        result = []

        # Input matrix 1
        print("Enter Matrix 1 elements:")
        for i in range(r1):
            row = []
            for j in range(c1):
                row.append(int(input()))
            matrix1.append(row)

        # Input matrix 2
        print("Enter Matrix 2 elements:")
        for i in range(r2):
            row = []
            for j in range(c2):
                row.append(int(input()))
            matrix2.append(row)

        # Perform matrix multiplication
        for i in range(r1):
            inner = []
            for j in range(c2):
                sum = 0
                for k in range(r2):  # or 'c1'
                    sum += matrix1[i][k] * matrix2[k][j]
                inner.append(sum)
            result.append(inner)

        # Print result
        print("Result:")
        for i in range(r1):
            for j in range(c2):
                print(result[i][j], end=" ")
            print()
```













### Output:
![Screenshot 2024-10-01 140141](https://github.com/user-attachments/assets/1ff98799-a5b4-4a2a-9c5a-450439480ccd)
![Screenshot 2024-10-01 140148](https://github.com/user-attachments/assets/b326e209-7d76-421f-89d2-e10d70930f99)






### Result:
Thus, the python program for matrix multiplication is implemented and the causes for its failure is introspected successfully.

