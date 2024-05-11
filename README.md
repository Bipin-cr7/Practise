#  Full Python COURSE

# variable = a reusable container for storing a value
#                   a variable behaves as if it were the value it contains

# INTEGER
age = 21
players = 2
quantity = 5

print(f"You are {age} years old")
print(f"There are {players} players online")
print(f"You would like to buy {quantity} items")

# FLOAT
gpa = 3.2
distance = 2.5
price = 10.99

print(f"Your gpa is {gpa}")
print(f"You ran {distance}Km")
print(f"The price is ${price}")

# STRING
name = "Bro"
food = "pizza"
email = "Bro123@gmail.com"

print(f"Hello {name}")
print(f"You like {food}")
print(f"Your email is: {email}")

# BOOLEAN
online = True
for_sale = False
running = False

print(f"Are you online?: {online}")
print(f"Is the item for sale?: {for_sale}")
print(f"Game running: {running}")





# type casting = The process of converting a value of one data type to another
#                          (string, integer, float, boolean)
#                          Explicit vs Implicit

name = "Bro"
age = 21
gpa = 1.9
student = True

# print(type(name))
# print(type(age))
# print(type(gpa))
# print(type(student)) 

age = float(age)
print(age)

gpa = int(gpa)
print(gpa)

student = str(student)
print(student)

name = bool(name)
print(name)



# ------------------------------------------------
# EXERCISE 1 MAD LIBS
# ------------------------------------------------
adjective1 = input("Enter an adjective: ")
noun = input("Enter a noun: ")
adjective2 = input("Enter an adjective: ")
verb = input("Enter a verb: ")
adjective3 = input("Enter an adjective: ")

print(f"Today I went to a {adjective1} zoo.")
print(f"In an exhibit, I saw {noun}.")
print(f"{noun} was {adjective2} and {verb}ing.")
print(f"I was {adjective3}!")




# ------------------------------------------------
# EXERCISE 2 AREA CALC
# ------------------------------------------------
length = float(input("Enter the length: "))
width = float(input("Enter the width: "))

#area = length * width
#print(f"The area is: {area}cm^2")

# ------------------------------------------------
# EXERCISE 3 SHOPPING CART
# ------------------------------------------------
item = input("What item would you like to buy?: ")
price = float(input("What is the price?: "))
quantity = int(input("How many would you like?: "))

total = price * quantity

print(f"You have bought {quantity} x {item}/s")
print(f"Your total is: ${round(total, 2)}")




# if = Do some code IF condition is True
# else = Do something else if above condition/s are False

# —---------------------
#   EXAMPLE 1
# —---------------------
age = int(input("Enter your age: "))

if age >= 100:
   print("You are too old to sign up")
elif age >= 18:
   print("You are now signed up")
elif age < 0:
   print("You haven't been born yet")
else:
   print("You must be 18+ sign up")

# —---------------------
#   EXAMPLE 2
# —---------------------
response = input("Do you want food (Y/N)?: ")

if response == "Y":
   print("Have some food")
else:
   print("No food for you!")

# —---------------------
#   EXAMPLE 3
# —---------------------
name = input("Enter your name: ")

if name == "":
   print("You did not enter your name!")
else:
   print(f"Hello {name}")

# —---------------------
#   EXAMPLE 4
# —---------------------
online = False

if online :
   print("You are online")
else:
   print("You are offline")




# calculator eercise 

operator = input("Enter an operator (+ - * /): ")
num1 = float(input("Enter the 1st number: "))
num2 = float(input("Enter the 2nd number: "))

if operator == "+":
    result = num1 + num2
    print(round(result, 3))
elif operator == "-":
    result = num1 - num2
    print(round(result, 3))
elif operator == "*":
    result = num1 * num2
    print(round(result, 3))
elif operator == "/":
    result = num1 / num2
    print(round(result, 3))
else:
    print(f"{operator} is not a valid operator")



# Python weight converter

weight = float(input("Enter your weight: "))
unit = input("Kilograms or Pounds? (K or L): ")

if unit == "K":
    weight = weight * 2.205
    unit = "Lbs."
    print(f"Your weight is: {round(weight, 1)} {unit}")
elif unit == "L":
    weight = weight / 2.205
    unit = "Kgs."
    print(f"Your weight is: {round(weight, 1)} {unit}")
else:
    print(f"{unit} was not valid")


# Temperature converter 


unit = input("Is this temperature in Celsius or Fahrenheit (C/F): ")
temp = float(input("Enter the temperature: "))

if unit == "C":
    temp = round((9 * temp) / 5 + 32, 1)
    print(f"The temperature in Fahrenheit is: {temp}°F")
elif unit == "F":
    temp = round((temp - 32) * 5 / 9, 1)
    print(f"The temperature in Celsius is: {temp}°C")
else:
    print(f"{unit} is an invalid unit of measurement")



# logical operators = used on conditional statements

#              and = checks two or more conditions are True
#               or = checks if at least one condition is True
#              not = True if condition is False, and vice versa

temp = 20
sunny = True

if temp <= 0 or temp >= 30:
    print("The temperature is bad")
else:
    print("The temperature is good")

if not sunny:
    print("It is cloudy")
else:
    print("It is sunny")






    # -------------------------------
# STRING METHODS
# -------------------------------
# name = input("Enter your name: ")
# phone_number = input("Enter your phone #: ")

# length = len(name)
# index = name.find(" ")
# name = name.capitalize()
# name = name.upper()
# name = name.lower()
# result = name.isdigit()
# result = name.isalpha()
# result = phone_number.count(" ")
# phone_number = phone_number.replace("-", "")

# -------------------------------
#        EXERCISE
# -------------------------------
username = input("Enter a username: ")

if len(username) > 12:
   print("Your name can't be more than 12 characters")
elif not username.find(" ") == -1:
   print("Your username can't contain spaces")
elif not username.isalpha():
   print("Your username can't contain digits")
else:
   print(f"Welcome {username}!")




   # indexing = accessing elements of a sequence using [] (indexing operator)
#                     [start : end : step]

credit_number = "1234-5678-9012-3456"

print(credit_number[0])
print(credit_number[0:4])
print(credit_number[:4])
print(credit_number[4:8])
print(credit_number[4:])
print(credit_number[-1])
print(credit_number[-4:])
print(credit_number[::2])
print(credit_number[::3])

# EXERCISE 1  display onlylast numbers 
credit_number = "1234-5678-9012-3456"
# last_digits = credit_number[-4:]
# print(f"XXXX-XXXX-XXXX-{last_digits}")

# EXERCISE 2  reverse the order of the numbers
credit_number = "1234-5678-9012-3456"
credit_number = credit_number[::-1]
print(credit_number)

# Email Slicing 


email = input("Enter your email: ")

username = email[:email.index("@")]
domain = email[email.index("@") + 1:]

print(f"Your username is {username} and domain is {domain}")






# ----------  EXAMPLE 1  ---------- 
def display_invoice(username, amount, due_date):
   print(f"Hello {username}")
   print(f"Your bill of ${amount:.2f} is due: {due_date}")

# display_invoice("BroCode", 42.50, "01/01")
# display_invoice("JoeSchmo", 100.01, "01/02")

# ----------  EXAMPLE 2  ---------- 
def create_name(first, last):
    first = first.capitalize()
    last = last.capitalize()
    return first + " " + last

full_name = create_name("spongebob", "squarepants")
print(full_name)




# format specifiers = {:flags} format a value based on what flags are inserted

# .(number)f = round to that many decimal places
# :(number) = allocate that many spaces
# :0(number) = allocate and zero pad that many spaces
# :< = left justify
# :> = right justify
# :^ = center align
# :+ = use a plus sign to indicate positive value
# := = place sign to leftmost position
# :  = insert a space before positive numbers
# :, = comma separator
# :% = percentage format

price1 = 3.14159
price2 = -987.65
price3 = 12.34
print(f"price1 is: ${price1:}")
print(f"price2 is: ${price2:}")
print(f"price3 is: ${price3:}")



 #while loop = perform some code WHILE some condition remains true

# ---------------- EXAMPLE 1 ----------------

name = input("Enter your name: ")

while name == "":
   print("You did not enter your name!")
   name = input("Enter your name: ")

print(f"Hello {name}")

# ---------------- EXAMPLE 2 ----------------

age = int(input("Enter your age: "))

while age < 0:
   print("Age can't be negative")
   age = int(input("Enter your age: "))

print(f"You are {age} years old")


# ---------------- EXAMPLE 3 ----------------

food = input("Enter a food you like (q to quit): ")

while not food == "q":
   print(f"You like {food}")
   food = input("Enter another food you like (q to quit): ")

print("bye")

# ---------------- EXAMPLE 4 ----------------

num = int(input("Enter a # between 1 - 10: "))

while num < 1 or num > 10:
    print(f"{num} is not valid")
    num = int(input("Enter a # between 1 - 10: "))

print(f"You picked the number {num}")
