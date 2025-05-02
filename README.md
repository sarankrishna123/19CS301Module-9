# 19CS301Module-9
### EX: 9.1                                            MATRIX OPERATIONS
### Aim: To Write a Python Program to subtract two matrices by reading the matrix from the user.
### Algorithm:

STEP 1: Start.

STEP 2: Create a variable r and c for rows and columns of the matrix.

STEP 3: Get the value of r and c from user.

STEP 4: Define a function to create a matrix.

STEP 5 : Define another function to subtract the matrices.

STEP 6: Print the result.

STEP 7 : Stop.
### Program:
```
reg no : 212223070023
name : Saran Krishna P S
def read_matrix(rows, cols):
    matrix = []
    for i in range(rows):
        row = list(map(int, input().split()))
        while len(row) != cols:
            row = list(map(int, input().split()))
        matrix.append(row)
    return matrix

def subtract_matrices(matrix1, matrix2):
    result = []
    for i in range(len(matrix1)):
        row = []
        for j in range(len(matrix1[0])):
            row.append(matrix1[i][j] - matrix2[i][j])
        result.append(row)
    return result

def main():
    rows = int(input())
    cols = int(input())
    matrix1 = read_matrix(rows, cols)
    matrix2 = read_matrix(rows, cols)
    result = subtract_matrices(matrix1, matrix2)
    for row in result:
        print(' '.join(map(str, row)))

if __name__ == "__main__":
    main()

```
### Output:
![image](https://github.com/user-attachments/assets/7963c983-d2c1-4b84-bdb9-c61cda061688)


### Result: Thus, the given program is implemented and executed successfully .

### EX: 9.2 LIST COMPREHENSION
### Aim: To Write a Python class program to generate all even numbers between 200 and 300 and store in a list using list comprehension.
### Algorithm:
STEP 1: Start.

STEP 2: Create a class.

STEP 3: Create variable a,b, and c for upper limit,lower limit and condition.

STEP 4: Intialise the values in the class.

STEP 5 : Define a method and using list comprehension calculate the result.

STEP 6: Print the result.

STEP 7 : Stop.

### Program:
```

reg no : 212223070023
name : Saran Krishna P S
class EvenNumberGenerator:
    def __init__(self, start, end):
        self.start = start
        self.end = end
        self.even_numbers = [x for x in range(start, end + 1) if x % 2 == 0]

    def get_even_numbers(self):
        return self.even_numbers

generator = EvenNumberGenerator(200, 300)
print(generator.get_even_numbers())

```
### Output:
![image](https://github.com/user-attachments/assets/209a1663-0138-41e5-91ed-f225fa087cf5)


### Result: Thus, the given program is implemented and executed successfully .

### EX: 9.3 ADVANCED LIST PROCESSING
### Aim: To Write a Python program to Find the transpose of a matrix using list Comprehension.

### Algorithm:

STEP 1: Start.

STEP 2: Create a variable r and c for rows and columns. 

STEP 3: Get the value of r and c from user.

STEP 4: Define a function to create the matrix.

STEP 5 : Using list comprehension find the transpose of the matrix.

STEP 6: Print the result.

STEP 7 : Stop.

### Program:
```

reg no : 212223070023
name : Saran Krishna P S
rows = int(input())
cols = int(input())
matrix = [list(map(int, input().split())) for _ in range(rows)]
transpose = [[matrix[j][i] for j in range(rows)] for i in range(cols)]
for row in transpose:
    print(' '.join(map(str, row)))


```
### Output:
![image](https://github.com/user-attachments/assets/33ce8b3f-0e7f-4231-9199-0a909d6fb52f)

### Result: Thus, the given program is implemented and executed successfully .
 


### EX: 9.4       TOEPLITZ MATRIX
### Aim: To Write a Python Program to check whether the given matrix is Toeplitz Matrix.


### Algorithm:
STEP 1: Start.

STEP 2: Create a variable r and c for rows and columns.

STEP 3: Get the value of r and c from user.

STEP 4: Define a function to create the matrix.

STEP 5 : Using the formula check for TOEPLITZ MATRIX .

STEP 6: Print the result.

STEP 7 : Stop.


### Program:
```

reg no : 212223070023
name : Saran Krishna P S
def is_toeplitz(matrix):
    rows = len(matrix)
    cols = len(matrix[0])
    for i in range(1, rows):
        for j in range(1, cols):
            if matrix[i][j] != matrix[i - 1][j - 1]:
                return False
    return True

rows = int(input())
cols = int(input())
matrix = [list(map(int, input().split())) for _ in range(rows)]

if is_toeplitz(matrix):
    print("Toeplitz Matrix")
else:
    print("Not a Toeplitz Matrix")


```
### Output:

![image](https://github.com/user-attachments/assets/cd144256-6d18-4e42-ab1a-39ed143f3b82)

### Result: Thus, the given program is implemented and executed successfully.
 

