name1 = "info@"
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

