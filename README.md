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
