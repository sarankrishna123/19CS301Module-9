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
reg no:212223070023
name:Saran Krishna P S
def create_matrix(n,m):
         M = []
         for i in range(n):
                   row = []
                   for j in range(m):
                      x = int(input())
                       row.append(x)
           M.append(row)
         return M
r,c = input().split()
A = create_matrix(int(r),int(c))
B = create_matrix(int(r),int(c))
C = []
for i in range(int(r)):
         R = []
 

        for j in range(int(c)):
                item = A[i][j]-B[i][j]
   R.append(item)
C.append(R)
print(A)
print(B)
print(C)
```
### Output:
![image](https://github.com/user-attachments/assets/715e58a2-ac73-4948-b611-c7ed1a20d74e)


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
reg no:212223070023
name:Saran Krishna P S
class program:

      def  __init__(self,a,b,c):
                self.a=a
                self.b=b
                self.c=c
        def display(self):
               even = [i for i in range(self.a,self.c+1,self.b)]
               print(even)
a = int(input())
b = int(input())
c = int(input())

obj = program(a,b,c)
obj.display()
```
### Output:
![image](https://github.com/user-attachments/assets/0bbace20-aa99-41c4-a05c-63b5dcf04a7d)

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
reg no:212223070023
name:Saran Krishna P S
def create(r,c):
            M=[]
        for i in range(int(r)):
             R = []
        for j in range(int(c)):
             x = int(input())
             R.append(x)
           M.append(R)
 return M
r,c = input().split()
matrix = create(int(r),int(c))
print(matrix)
T = [[r[i]for r in matrix]for i in range(len(matrix[0]))]
 print(T)
```
### Output:
![image](https://github.com/user-attachments/assets/4f9b1d3d-84d8-4a05-8ffe-28c11a1283e5)


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
reg no:212223070023
name:Saran Krishna P S
def create_matrix(n,m):
        M=[]
        for i in range(n):
                row=[]
        for j in range(m):
            x=int(input())
            row.append(x)
        M.append(row)
      return M
def print_matrix(M):
    for i in range(len(M)):
         for j in range(len(M[0])):
               print(M[i][j], end=' ')
     print()
def isThoeplitz(M):
#Type your code here
for i in range(len(M)):
      for j in range(len(M[0])):
             if i>0 and j>0 and M[i][j]!=M[i-1][j-1]:
                return False
       return True
n,m = input().split()
A = create_matrix(int(n),int(m))
print("A=",A)
if isThoeplitz(A):
      print(A,"is a Toeplitz Matrix")
 else:
       print(A,"is not a Toeplitz Matrix") print_matrix(A)
```
### Output:
![image](https://github.com/user-attachments/assets/50989d28-3a25-4e2a-bdf4-129d865426ff)

### Result: Thus, the given program is implemented and executed successfully.

### EX: 9.4 find the square root of all elements in a list using list comprehension.     
### Aim: Write a Python program to calculate the square root of all elements in a given list using list comprehension.


### Algorithm:

Start
Read the number of elements 
Initialize an empty list to store the input numbers.
For 𝑖=1i=1 to 𝑛 n:
Read the number and append it to the list.
Use list comprehension with the math.sqrt() function to calculate the square root of each element in the list.
Print the original list.
Print the list of square roots.
End

### Program:
```
reg no:212223070023
name:Saran Krishna P S
n=int(input())
l=[]
for i in range(n):
    x=float(input())
    l.append(x)
sq_l=[item**0.5 for item in l]
print(l)
print(sq_l)

```
### Output:
![image](https://github.com/user-attachments/assets/ab25c3bf-1a04-43cb-be5e-c3cb149fa06a)


### Result: Thus, the given program is implemented and executed successfully.
 

 

