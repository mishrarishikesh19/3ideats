# 3ideats

# 1) Write a python program to calculate area of triangle and circle and print the result. Take input from user.

# Calculate area of triangle
'''
A = 1/2 b*h
'''
Base = float(input("Enter the base of the triangle :"))
Height = float(input("enter the height of the  triangle :"))
Are_of_triangle = 1/2 * Base * Height
print("The area of triangle is : " ,Are_of_triangle)

# Calculate area of circle
'''
A = πr2
'''
Radius = float(input("Enter the radius of the circle:"))
Area_of_circle = 3.14 * (Radius **2)
print("The area of the circle is: " , Area_of_circle)


# 2) Explain features of python program.

'''
1.Easy to Learn: Python has a simple syntax and easy to learn, making it a great language for beginners.

2.High-Level Language: Python is a high-level language and allowing developers to focus on the logic of the program memory management, etc.

3.Interpreted Language: Python code is interpreted line by line, making it write and test code. that Python code can be executed.

4.Object-Oriented: Python is an object-oriented language, that can organizes code into objects data.

5.Large Standard Library: Python has large standard library that includes modules for various tasks, such as I/O, networking, and data structures.

6.Dynamic Typing: Python is dynamically typed a variable is  runtime, rather than compile time.

7.Cross-Platform: Python can run on multiple operating systems, including Windows, macOS, and Linux. 

'''

# 3) Discuss difference between local and global variables.

'''
Local Variables   

Defined inside our of system 
Defined within a specific block of code (e.g., a function)
Only accessible within that block
Created when the block is executed and destroyed when the block is exited
'''

#Exemple

def example():
    x = 5  # Local variable
    print(x)

example()  # Outputs: 5
print(x)   # Error: x is not defined (since x is local to the function)

'''
Global Variables

Defined outside of any block of code
Accessible from anywhere in the program
Created when the program starts and destroyed when the program ends 
'''

#Exemple
x = 10  # Global variable

def example():
    global x
    x = 5  # Modify the global variable
    print(x)

example()  # Outputs: 5
print(x)   # Outputs: 5 (global variable was modified)



# 4) Explain if – else statement with an example.
'''
The if-else statement is a fundamental control structure in programming that allows you to execute one block of code if a condition is true and a different block of code if the condition is false. It's a way of making decisions within your program based on conditions.
'''
#Syntex
'''
if condition:
    # Code to execute if the condition is True
else:
    # Code to execute if the condition is False
'''

#Example

age=int(input("enter your age:"))
if age > 18:
    print("can votes:")
else:
    print("cannot votes:")

# 6) What are different ways to create strings in python .
'''
1>Single Quotes: You can create a string by enclosing text in single quotes '''
my_string = 'Hello, World!' 
'''
2>Double Quotes: You can also create a string by enclosing text in double quotes. '''
my_string = "Hello, World!" 
'''
3>Triple Quotes: Triple quotes are used to create a multiline string. You can use either single or double triple quotes. '''
my_string = """This is a
multiline string"""
'''
4>Raw Strings: Raw strings treat backslashes (\) as literal characters, which is useful when dealing with regular expressions or Windows file paths '''
my_string = 'r'
'''
5>String Concatenation: You can concatenate (combine) strings using the + operator. '''
my_string = 'Rishi, ' + 'Mishra'
'''
6>String Multiplication
Strings can be multiplied using the * operator to repeat the string multiple times.
my_string = 'Hi! ' * 3  # Output: 'Hi! Hi! Hi! '
'''
# 7> Write a note on string slicing in python .
'''
A slice is a subset of a sequence (such as a string, list, or tuple) that is extracted from the original sequence using a specific syntax.
Slice is defined by three components:  
Start: The starting index of the slice (inclusive).
Stop: The ending index of the slice (exclusive).
Step: The increment between indices (default is 1).
syntax for a slice is: sequence[start:stop:step]    

example:                                                                            '''  
my_string = "hello world"
my_slice = my_string[0:5]  # start=0, stop=5, step=1
print(my_slice)  # Output: "hello"

# 8> Write a program to check if entered year is leap year or not .

year= int(input("enter year:-"))
if(year%4==0 or year%400==0 and year%100!=0):
    print("year is leap")
else:
    print("year is not leaP")


    # 10> What are different type errors in python?
'''
1)TypeError: Python encounters an operation that is not supported for a particular data type. 
For example: '''                                                                                 
'''a = 5
b = "hello"
print(a + b)  # TypeError: unsupported operand type(s) for +: 'int' and 'str' '''

'''
2)AttributeError: This error occurs try to access an attribute that does not exist for an object. 
For example: '''
'''a = 5
print(a.append(10))  # AttributeError: 'int' object has no attribute 'append' '''

'''
3)IndexError: This error occurs try to access an index that is out of range for a sequence (such as a list, tuple, or string).
For example: '''
'''
a = [1, 2, 3]
print(a[5])  # IndexError: list index out of range '''

'''
4)KeyError: This error occurs try to access a key that does not exist in a dictionary.
For example:'''
'''
a = {"name": "John", "age": 30}
print(a["city"])  # KeyError: 'city'      '''

'''
5)SyntaxError: This error occurs is a syntax error in your Python code, such as a missing colon, incorrect indentation, or invalid syntax. 
For example: '''
if True
    print("Hello")  # SyntaxError: invalid syntax


# 11> Write a bitwise operator in python.
'''
Bitwise AND (&)      
The bitwise AND operator (&) compares each bit of the first operand to the corresponding bit of the second operand. If both bits are 1, the corresponding result bit is set to 1. Otherwise, the corresponding result bit is set to 0.   
'''        
'''
# Bitwise AND
a = 10  # In binary: 1010
b = 4   # In binary: 0100

print("a & b =", a & b)  # AND operation: 1010 & 0100 = 0000 (Output: 0)
'''
'''
Bitwise OR (|)
The bitwise OR operator (|) compares each bit of the first operand to the corresponding bit of the second operand. If either bit is 1, the corresponding result bit is set to 1. Otherwise, the corresponding result bit is set to 0.'''
'''
# Bitwise OR
a = 10  # In binary: 1010
b = 4   # In binary: 0100

print("a | b =", a | b)  # OR operation: 1010 | 0100 = 1110 (Output: 14)

'''
'''
Bitwise NOT (~)
The bitwise NOT operator (~) inverts all the bits of the operand.
'''
'''
# Bitwise NOT
a = 10  # In binary: 1010
b = 4   # In binary: 0100

print("~a =", ~a)  # NOT operation: ~1010 = -(1011) (Inverts and changes the sign) (Output: -11)

'''

# 12. Write a python program to display the following series.
''''
 *
 * *
 * * *
 * * * *
 * * * * *  
'''
'''
# Number of rows we want to print
n = 5

# Outer loop for each row
for i in range(1, n + 1):
    # Inner loop for printing stars in each row
    for j in range(i):
        print("*", end=" ")  # Print star and a space on the same line
    print()  # Move to the next line after each row
'''
'''
1. n = 5: This sets the number of rows to 5.
2. for i in range(1, n + 1): This outer loop controls the rows. It runs from 1 to 5, printing stars in each row.
3. for j in range(i): This inner loop runs i times in each iteration of the outer loop, printing the stars on the same line.
4. print("*", end=" "): This prints a star followed by a space, without moving to the next line.
5. print(): This moves the cursor to the next line after printing each row of stars.
'''
# 13. Write a short note on looping structure in python.
'''
#for
fruits = ['apple', 'banana', 'cherry']
for fruit in fruits:
 print(fruit) 

# while
 i = 0
while i < 5:
    print(i)
    i += 1

# break                       
for i in range(10):
   if i == 5:
    break
print(i)

#contineous
for i in range(15):
  if i ==10:
    continue
  print(i)

'''
#16. Explain the use if in and not in operator in with suitable program
'''
1. in Operator: The in operator returns True if the value is found in the sequence, and False otherwise.

Example:

fruits = ['apple', 'banana', 'cherry']
    if 'apple' in fruits:
        print("Apple is in the list")
        else:
            print("Apple is not in the list")
            # Output: Apple is in the list


2. not in Operator:

The not in operator returns True if the value is not found in the sequence, and False otherwise.

Example:

fruits = ['apple', 'banana', 'cherry']
if 'orange' not in fruits:
    print("Orange is not in the list")
    else:
        print("Orange is in the list") 
        # Output: Orange is not in the list
'''

# 19. Explain the lower(), Split(), find(), len(), isdigit() function with example .
'''
str1 = "Rishi"
result = str1.lower()
print(result)

str2 = "Rishi , kumar, mishra "
result = str2.split(",") 
print(result)

str3 = "Rishi Kumar mishra"
result = str3.find("mishra")
print(result)

str4 = "Rishi"
result = len( str4)
print(result)


str5 = "9876"
str = "Rishi123"
result = str5.isdigit()
digit= str.isdigit()
print(result)  # True 
print(digit)   # False
'''


# 20. Explain any 10 string function with example. 
'''
str1 = "rishi"
result = str1.lower()
print(result)

str2 = "mishra"
result = str2.upper()
print(result)

str3 = "rishi , kumar, mishra "
result = str3.split(",") 
print(result)

str4 = "rishi Kumar mishra"
result = str4.find("mishra")
print(result)

str5 = "rishi"
result = len( str5)
print(result)


str6 = "9876"
result = str6.isdigit()
print(result)  # True 

str7 = "rishi123"
digit= str7.isdigit()
print(digit)   # False

str8 = "hello world"
result = str8.replace("world", "universe")
print(result)  # Output: "hello universe"

str9 = "hello world"
result = str9.startswith("hello")
print(result)  # Output: True

str10 = "hello world"
result = str10.endswith("world")
print(result)  # Output: True

'''
#21. Write a Python program to find those numbers which are divisible by 7 and multiples of 5, between 1500 and 2700 (both included)
'''
# Initialize an empty list to store the numbers

numbers = []

# Iterate over the range from 1500 to 2700 (both included)

for i in range(1500, 2700):
    # Check if the number is divisible by 7 and a multiple of 5
    if i % 7 == 0 and i % 5 == 0:
        # If the condition is true, add the number to the list
        numbers.append(i)
# Print the list of numbers
print("Numbers between 1500 and 2700 that are divisible by 7 and multiples of 5:")
print(numbers)

'''

#23. Write a Python program to guess a number between 1 and 9.
'''
Note: User is prompted to enter a guess. If the user guesses wrong then the prompt appears again until the guess is correct, on successful guess, user will get a "Well guessed!" message, and the program will exit.

import random
guess = None
num = 0

while guess != num:
num random.randint(1,9)
guess = int(input("Guess the number between 1 to 9:-"))

if guess == num:
print("Well guessed!")
 else:
print("Wrong guess! Try again")

'''
