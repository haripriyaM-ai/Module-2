## MODULE-2
# EXP 6: Built-in Functions -Binary Conversion Using Built-in Functions in Python

## Aim
To write a Python program to convert the number **16** into its **binary representation** using built-in Python functions.

## Algorithm
1. Assign the value `16` to a variable `a`.
2. Use the built-in `bin()` function to convert the number to binary.
3. Print the result.

## Program

```
a=16
result =  bin(a)
print(result)
```

## Output
![Screenshot 2025-05-21 174351](https://github.com/user-attachments/assets/4481bffa-202f-48e4-b478-a5c6249a3837)

## Result
Thus, the program is verified successfully.

---

# EXP 7: Functions in Python: Modulo Calculator

## Aim
To write a Python program that defines a function which accepts two values and returns their **modulo** using the `%` operator.

## Algorithm
1. Define a function called `result` that takes two arguments `a` and `b`.
2. Inside the function, compute the modulo using `a % b`.
3. Print the result of the modulo operation.
4. Get two integer inputs from the user.
5. Call the `result` function with the user-provided values.

## Program

```
def result(a,b):
    return a % b 
    
n1=int(input())
n2=int(input())
print("result :",result(n1,n2))
```

## Output
![image](https://github.com/user-attachments/assets/94dd7951-f19e-4a16-b259-f86e7a55fb4f)

## Result
Thus, the program is verified successfully.

---

# EXP 8: Lambda Function in Python: Addition of Three Numbers

## Aim
To write a Python program that defines a **lambda function** which takes three arguments `a` and `b` and `c`, and returns their sum.

## Algorithm
1. Get three integer inputs from the user.
2. Use a **lambda function** to define a function `f` that returns `a + b + c`.
3. Call the function with the user inputs and print the result.

## Program
```
i=int(input())
j=int(input())
z=int(input())

f = lambda a, b,c: a+b+c

print(f(i, j,z))
```
## Output
![image](https://github.com/user-attachments/assets/c70f47f8-f3c8-44c0-81d5-ea7aeb126d55)

## Result
Thus, the program is verified successfully.

---

# EXP 9: Looping(Patterns)-Pascal's Triangle Generator in Python

This project demonstrates a simple Python program to generate **Pascal’s Triangle**, where the number of rows is provided by the user.



## Aim

To write a Python program that generates **Pascal's Triangle** using numbers. The number of rows is accepted from the user.


## Algorithm

1. Start the program.
2. Input the number of rows from the user.
3. Loop from 0 to the number of rows.
4. For each row:
   - Print appropriate spaces to shape the triangle.
   - Compute values using the formula:  
     \[
     C(n, k) = \frac{n!}{k!(n-k)!}
     \]
5. Print all rows of Pascal’s Triangle.
6. End the program.


##  Program
```
rows = int(input())
coef = 1

for i in range(1, rows+1):
    for space in range(1, rows-i+1):
        print(" ",end="")
    for j in range(0, i):
        if j==0 or i==0:
            coef = 1
        else:
            coef = coef * (i - j)//j
        print(coef, end = " ")
    print()
```
## Output
![image](https://github.com/user-attachments/assets/b58e63dc-8286-470a-a788-3d72a63ddb8a)

## Result
Thus, the program is verified successfully.

---

# EXP 10: Loops in Python: Palindrome Number Checker

## Aim
To write a Python program that checks whether a given number is a **palindrome** using loops.

## Algorithm
1. Get input from the user and assign it to a variable `num`.
2. Assign the value of `num` to a temporary variable `temp`.
3. Initialize a variable `rev` to 0 (used to store the reversed number).
4. Use a `while` loop to reverse the digits:
   - While `temp > 0`:
     - `rev = (10 * rev) + temp % 10`
     - `temp = temp // 10`
5. After the loop, compare `rev` with `num`:
   - If equal, print that the number is a palindrome.
   - Else, print that it is not a palindrome.

## Program
```
num=int(input())
temp=num
rev=0
while temp>0:
    ld=temp%10
    rev=(rev*10)+ld
    temp=temp//10
if num==rev:
    print(f"The given number {temp} is a Palindrome".format(n))
else:
    print(f"The given number {temp} is not a palindrome".format(n))

```
## Output
![image](https://github.com/user-attachments/assets/8ae648dd-fa8c-4723-9b56-260d861b0874)

## Result
Thus, the program is verified successfully.
