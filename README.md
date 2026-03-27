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
for i in range(1,51):
    sum += i
print("The sum of numbers from 1 to 50 is:",sum)


Assignment 3
1)
def factorial(n):
    if n == 0:
        return 1
    else:
        return n * factorial(n-1)
a = int(input("Enter a number:"))
b = factorial(a)
print(f"The factorial of {a} is {b}")



2)
import math
a = int(input("Enter a number: "))
print(f"Square root of {a} is {math.sqrt(a)}")
print(f"Natural log of {a} is {math.log(a)}")
print(f"Sine of {a} is {math.sin(a)}")


Assignment 4
1)
try:
    with open("sample.txt", "r") as file:
        print("Reading file content:\n")
        line_number = 1
        for line in file:
            print("Line", line_number, ":", line.strip())
            line_number += 1
except FileNotFoundError:
    print("Error: The file 'sample.txt' was not found.")
finally:
    print("\nTask 1 execution completed.")

2)
text = input("Enter text to write to the file: ")
file = open("output.txt", "w")
file.write(text + "\n")
file.close()
print("Data successfully written to output.txt.\n")
more_text = input("Enter additional text to append: ")
file = open("output.txt", "a")
file.write(more_text + "\n")
file.close()
print("Data successfully appended.\n")
print("Final content of output.txt:")
file = open("output.txt", "r")
for line in file:
    print(line.strip())
file.close()


Assignment 5
1)
student_marks = {
    "Alice": 85,
    "Bob": 90,
    "Charlie": 78,
    "David": 88
}
name = input("Enter the student's name: ")

if name in student_marks:
    print(f"{name}'s marks: {student_marks[name]}")
else:
    print("Student not found.")



2)
numbers = list(range(1, 11))
first_five = numbers[:5]
reversed_list = first_five[::-1]

print("Original list:", numbers)
print("Extracted first five elements:", first_five)
print("Reversed extracted elements:", reversed_list)
