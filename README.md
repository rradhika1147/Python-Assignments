# Python-Assignments
Assignment 1
1)
a = float(input("Enter the first number: "))
b = float(input("Enter the second number: "))
print("Addition:",a+b)
print("Subtraction:",a-b)
print("Multiplication:",a*b)
print("Division:",a/b)

2)
first_name = input("Enter the first name: ")
last_name = input("Enter the second name: ")
print(f"Hello, {first_name} {last_name}! Welcome to the Python program. ")


Assignment 2
1)
a = int(input("Enter a number: "))
if a % 2 == 0:
    print(f"{a} is an even Number")
else:
    print(f"{a} is an odd Number")



2)
sum = 0
for i in range(1,50):
    sum += i
print("The sum of numbers from 1 to 50 is:",sum)


Assignment 3
1)
def factorial(n):
    if n == 0:
        return 1
    else:
        fact = 1
        for i in range(1,n+1):
            fact *= i
        return fact

a = int(input("Enter a number:"))
b = factorial(a)
print(f"The factorial of {a} is {b}")



2)
import math
a = int(input("Enter a number: "))
print(f"Square root of {a} is {math.sqrt(a)}")
print(f"Natural log of {a} is {math.log(a)}")
print(f"Sine of {a} is {math.sin(a)}")
