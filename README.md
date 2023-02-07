# Tasks-1-2-and-3

# Name:               task 1.py
# Author:             Yahya Jama
# Date Created:       February 05, 2023
# Date Last Modified: February 06, 2023
# Purpose:
# The program will ask the user to put in information they are looking for. For the rectangle and triangle they will put it in cm
# The next next step will ask the user to put in the lengthof the rectangle or triangle.
# As a result, the program will display the area in cm2 and perimeter in cm.

print("Please enter your choice.")
print("1. Calculate the Area of a Circle")
print("2. Calculate the Area of a Rectangle")
print("2. Calculate the Area of a Triangle")
print("4. Quit")

choice = input("Enter choice.")

if choice == '1':
     radius = float(input("Please enter the radius in cm."))
     pi = 3.14
     area = pi * radius * radius
     perimeter = 2 * pi * radius
     print("Area of circle is" +area+ "cm^2")
     print("Perimeter of circle is" +perimeter+ "cm.")
elif choice == '2':
    length = float(input("Enter the length of the rectangle in cm."))
    breadth = float(input("Enter the breadth of the rectangle in cm."))
    area = length * breadth
    perimeter = 2 * (length + breadth)
    print("Area of rectangle is "+area+"cm^2.")
    print("Perimeter of rectangle is"+perimeter+ "cm")
elif choice == '3':
    side = float(input("Enter the side of the triangle in cm."))
    base = float(input("Enter the base of the triangle in cm."))
    height = float(input("Enter the height of the triangle in cm."))
    area = 0.5 * base * height
    perimeter = side + side + side
    print("Area of triangle is"+area+"cm^2.")
    print("Perimeter of triangle is"+perimeter+"cm.")
elif choice == '4':
    print("Try again.")
else:
    print("Invalid input.")


# Name:               task 2.py
# Author:             Yahya Jama
# Date Created:       February 05, 2023
# Date Last Modified: February 06, 2023
# Purpose:
# The purpose of this program will allow us to calculate area and perimeter of a rectangle, square or a circle using functions.
# First we will write a pseudocode.
# Secondly we will write the code depending on the written pseudocode.



def area_square(s):
    return(s * s)
def perimeter_square(s):
    return(4 * s)
def area_rectangle(a,b):
    return(a * b)
def perimeter_rectangle(a,b):
    return(2 * (a+b))
def are_circle(r):
    return(pi * r * r)
def perimeter_circle(r):
    return(2 * pi * r)
def quit():
    return()



print("Please enter your choice.")
print("1. Calculate the Area of a Circle")
print("2. Calculate the Area of a Rectangle")
print("2. Calculate the Area of a Triangle")
print("4. Quit")

choice = input("Enter choice.")

if choice == '1':
     radius = float(input("Please enter the radius in cm."))
     pi = 3.14
     area = pi * radius * radius
     perimeter = 2 * pi * radius
     print("Area of circle is" +area+ "cm^2")
     print("Perimeter of circle is" +perimeter+ "cm.")
elif choice == '2':
    length = float(input("Enter the length of the rectangle in cm."))
    breadth = float(input("Enter the breadth of the rectangle in cm."))
    area = length * breadth
    perimeter = 2 * (length + breadth)
    print("Area of rectangle is "+area+"cm^2.")
    print("Perimeter of rectangle is"+perimeter+ "cm")
elif choice == '3':
    side = float(input("Enter the side of the triangle in cm."))
    base = float(input("Enter the base of the triangle in cm."))
    height = float(input("Enter the height of the triangle in cm."))
    area = 0.5 * base * height
    perimeter = side + side + side
    print("Area of triangle is"+area+"cm^2.")
    print("Perimeter of triangle is"+perimeter+"cm.")
elif choice == '4':
    print("Try again.")
else:
    print("Invalid input.")



# Name:               task 3.py
# Author:             Yahya Jama
# Date Created:       February 05, 2023
# Date Last Modified: February 06, 2023
# Purpose:
# The purpose of this program is to get the name of the user.
# The user name must be more than one letter and less than twenty letters.
# The user name msut contain at least one uppercase letter and one number.
# If the username fails to match the requirments display error message and ask to renter .

username= input("Please enteer a username with a capital letter and a number: ")

if username.islower() and "1234567890" not in username:
    print("Your username will need to have at least one number and at least one capitalized letter")
    username = input("Please enter another username: ")
# To check the length of the username
if len(username) >= 1:
    print("Sorry, username must be longer than one letter.")

if len(username) >= 20:
    print("Sorry, username cannot be more than 20 letters in length.")
