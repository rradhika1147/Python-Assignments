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
def read_file():
    try:
        with open("sample.txt", "r") as file:
            print("Reading file content:\n")
            for line_number, line in enumerate(file, start=1):
                print(f"Line {line_number}: {line.strip()}")

    except FileNotFoundError:
        print("Error: The file 'sample.txt' was not found.")

    except Exception as e:
        print(f"An unexpected error occurred: {e}")
read_file()



2)
def write_and_append_file():
    try:
        text = input("Enter text to write to the file: ")
        with open("output.txt", "w") as file:
            file.write(text + "\n")
        print("Data successfully written to output.txt.\n")
        more_text = input("Enter additional text to append: ")
        with open("output.txt", "a") as file:
            file.write(more_text + "\n")
        print("Data successfully appended.\n")
        print("Final content of output.txt:")
        with open("output.txt", "r") as file:
            for line in file:
                print(line.strip())
    except Exception as e:
        print(f"An error occurred: {e}")
write_and_append_file()

