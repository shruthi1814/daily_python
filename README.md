vname1 = "info@"
name2 = "support@"
name3 = "www."
print(name1+"datawithbara.com")
print(name2+"datawithbara.com")
print(name3+"datawithbara.com")

age = 22
height = 5.14
name = "shruthi"
student = True
no = " "
print("my name is",name)
print("my height is",height)
print("my age is",age)
print("are you student?",student)
print(no)

stamp = "2026-05-12"
print(stamp.split("-"))

print("="*30)
print("ha"*4)

phone = "+49 (167) 123-456"
print(phone.replace("+","").replace(" ","").replace("(","").replace(")","").replace("-",""))

name = "shruthi"
age = 21
student = True
print(f"my name is {name},and I'm {age} years old and my student status is {student}")

print(f"2*4={2*4}")
print(f"4/2= {4/2}")

name = input("enter your name:")
country = "India"
print ("my name is",name,"and I am from",country)

x = 10
y = 3.14
z = 3+4j
print(type(x))
print(type(y))
print(type(z))

print(2-10)
print(abs(2-10))
price = "123.456"    #str
price = float(price)
print(round(price))

# # updating a list
letters = ['a','c','d','e']
letters[1] = 'x'                 # updates the element at the specified index
print(letters)

import math
price = 34.5678
print(math.floor(price))
print(math.ceil(price))
print(round(price))
print(round(price,2))
print(math.trunc(price))

x = 10
y = math.sqrt(x)
print(y)
print(math.trunc(y))

score = 100
if score>=80:
    print("passed")
    print("hurryyyyy!!!")
else:
    print("failed")


# elif statement
score = 80
if score >=90:
    print("good")
elif score >=70:
    print("average")
elif score >=50:
    print("poor")
else:
    print("failed")

# nested if
assignment = 60
project = True
if assignment >=90:
    if project:
        print("A+" )
    else:
        print("good")
else:
    print("fail")


# elif statement
mark = 100
project = False
if mark>=90 and project:
    print("A+")
elif mark >=50 and not project:
    print("good")
else:
    print("Fail")

print("hello")
print("nothing is impossible")

# independent if statement
score = 90
project = False
if score >=80:
    print("hight score")
else:
    print("low score")
if project:
    print("project completed")
else:
    print("project not submitted")

# ternary if
score = 79
print("pass" if score >=80 else "fail")

result = "pass" if score >=80 else "fail"
print(result)

# match case
country = "egypt"
match country:
    case "united states":
        print("us")
    case "india":
        print("IN")
    case "germany":
        print("DE")
    case _:
        print("unknown country")

# challenge-------1
email = "user@gmail.org"
print(email is not " " and email is not "" and "." in email and "@" in email and (email.endswith(".com") or email.endswith(".net") or email.endswith(".org")) and len(email)<=254)

# challenge-------2

password = "Shruthi!1215#"
email = "shruthi@123"

password = password.strip()
email = email.strip()

if password =="":
    print("password must not be empty...fill the password")

elif len(password)<8:
    print("password must contain more than 8 characters..")

elif not(any(ch.isupper() for ch in password) and any(ch.islower() for ch in password)):
    print("password must contain both uppercase and lowercase letters..")

elif password == email:
    print("password must not be same as email..")

# for loop basics
for i in (1,2,3):
    print(i) 

for i in (1,2,3,4,5):
    print("Round:",i)

# for in tuple
items = (1,2,3,4,5,6)
for item in items:
    print(f"Round no: {item}")

# for in list
items = [1,2,3,4,5,"hello"]
for item in items:
    print(f"Round no: {item}")

# for in string
items = " python"
for item in items:
    print(f"Round no: {item}")

# for in range
for item in range(100):
    print(f"Round no: {item}")

# challenge-----------1
# print the 7th table from 1 to 10 using for loop
for i in range(1,11):
    print(f"7 x {i} = {7*i}")

# print a left-aligned pyramid of stars using for loop
for i in range(1,7):
    print("* "*i)

# break statement
names = ["john","jane","doe","","smith"]
for name in names:
    if name=="":
        print("empty value deceted..!")
        break
    print(f"Name:{name}")

# continue statement
names = ["john","jane","doe","","smith"]
for name in names:
    if name=="":
        print("empty value deceted..!")
        continue
    print(f"Name:{name}")

# # example
days = int(input())
sms = int(input())
calls = int(input())
data = float(input())

print("Your plan expired. Kindly recharge"if days > 84 else f"Your plan will be expired on {84-days} days")

print("msg failed" if sms > 100 else f"yet to use {100-sms}")

print("calls could not be connected. kindly top up" if calls > 3000 else f"yet to use {3000-calls} calls")

print("kindly top up" if data > 2.0 else f"yet to use {2.0-data} gb")


# # example
n = "kashmir258"
f = ""
m = ""
d = ""
for i in range(len(n)):
    if n[i].isalpha():
        print(n[i], end = '')
    if n[i].isnumeric():
        f += n[i]
m = sum(int(digit) for digit in f)
first_sum = m
while m>9:
    d = sum(int(d) for d in str(m))
    m = d
print()
print(f)
print(first_sum)
print(m)


# to print a magical prime number if a number is prime and the reverse of the number is also prime then it is called a magical prime number

n = int(input("enter a number: "))
def is_prime(num):  
    if num < 2:
        return False
    for i in range(2, int(num**0.5) + 1):
        if num % i == 0:
            return False
    return True
if is_prime(n):
    print("it is a magical prime number")
else:
    print("not a magical prime number45")

# Print the frequency of every character in the string.
k = input("enter a string:")
for i in range(len(k)):
    count = 0
    for j in range(len(k)):
        if k[i] == k[j]:
            count +=1
    print(k[i],":",count)

