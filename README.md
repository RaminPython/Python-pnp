# Python-pnp
eur = 1.3
usd = 1.2
# Your code it here
val = float(input("Enter valute: "))
total_euro      = "total euro: %.2f" % (val/eur)
total_dollar    = "total dollars: %.2f" % (val/usd)
print(total_euro)
print(total_dollar)

tax = 0.15
price = float(input("Enter price: "))
print("price with tax is", price + price * tax)

db_username = "ramin"
db_password = "fericire21"
# Your code it here
username = input("username: ")
password = input("password: ")
print(db_username == username and db_password == password)

def pow():
    global a,b,c
    a = 32
    b = 1
    c = 3
pow()
print(a*b*c)

def factorial(n):
    res = 1
    for i in range(1,n+1):
        res *= i
    
    return res

while True:
    n = int(input("Enter number: "))
    print(factorial(n))

def fibonacci_numbers(nums):
    x, y = 0, 1
    for _ in range(nums):
        x, y = y, x+y
        yield x


for n in fibonacci_numbers(100):
    print(n)

thisDict = {
    "Brand": "Ford",
    "Model": "Mustang",
    "year": 2021
}
print(thisDict)

sampleDict = {
    "emp1": {"Name": "Ramin", "salary": 2021},
    "emp2": {"Name": "George", "salary": 1000},
    "emp3": {"Name": "Andrei", "salary": 3242}
}
sampleDict["emp3"]["salary"] = 1000
print(sampleDict)

book_names = ["Ramin cel mare", "Robert cel mic"]
book_years = [1912, 2021]
# Your code it here
books = {}
for i in range(len(book_names)):
    books[book_names[i]] = book_years[i]

print(books)

products = ["tv", "appel"]
prices = [" 2021, lei", "20 de lei"]
for i in range(len(products)):
    print(products[i],":", prices[i])

blacklist = ["Ramin", "George"]
users = []
while True:
    newuser = input("username: ")
    if newuser in blacklist:
        print("Sorry you cannot enter")
    else:
        users.append(newuser)
    print("Current users")
    print(users)

import calendar

yy = 2021
mm = 3

print(calendar.month(yy, mm))

import calendar

yy = int(input("Enter years: "))
mm = int(input("Enter month: "))
print(calendar.month(yy, mm))

import calendar

yy = 2021
mm = 3

print("This is it my claendar: ")
print(calendar.calendar(yy, mm))

age = int(input("Enter your age: "))

if age <= 24:
    print("Acces")
else:
    print("Sorry you cannot enter")

H    = 10
a    = 1
for i in range(H):
    for j in range(a):
        print("*",end="")
    
    a+=1
    print("")

list = {"Engleza -> en, Spaniola -> sp, Franceza -> fr Romana -> ro, Tiganesti -> tig"}
print(list)

lang = input("language: ")    
if(lang=="en"):
        print("Hello")    
elif(lang=="fr"):
        print("Bonjure")    
elif(lang=="sp"):
        print("Ciao")    
elif(lang=="ro"):
        print("Salut")    
elif(lang=="tig"):
        print("Haorde")    

class Student():
    def __init__(self, name, age):
        self.name = name
        self.age = age

student1 = Student("Andrei", 21);
student2 = Student("George", 31);

print("Andrei", 21); print(student1.age);
print("George", 31); print(student2.age);

class Myacconts():
    def __init__(self, username, password, email):
        self.username = username
        self.password = password
        self.email    = email

print(Myacconts)

username = input("username: ")
print("Username is " + username)

password = input("password: ")
print("Password is " + password)

email = input("email: ")
print("Email is " + email)

Manufacturer = "Ramin"    
Model_name = "iphone 8"    
Gb = "32 Gb"    
Garantie = "30 de zile"    
Image = "https://github.com/aadiaconitei/mysql-python/blob/master/curs4/comenzi.sql"    
Price = 300    
    
    
    
print("Manufacturer: ")    
print(Manufacturer)    
print("Model_name: ")    
print(Model_name)    
print("Gb: ")    
print(Gb)    
print("Garantie: ")    
print(Garantie)    
print("Image: ")    
print(Image)    
print("Price: ")    
print(Price)   

import socket
import time

sSocket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
sSocket.bind(("localhost",1900))
sSocket.listen()
print("Lisening connexion: ")
conn, addr = sSocket.accept()

print("Connexion received from ", addr)
data = conn.recv(1024)

print("Message from client: \n")
time.sleep(2)
print(data)
conn.close()
sSocket.close()

import socket

cSocket = socket.socket(socket.AF_INET,socket.SOCK_STREAM)
cSocket.connect(("localhost",1900))

cSocket.send(b"Ce mai faci")
cSocket.sendall(b"Bine tu")

cSocket.close()

import socket

server = socket.socket(socket.AF_INET,socket.SOCK_DGRAM)
server.bind(("localhost",1900))
msg = server.recvfrom(16)
print(msg)

import socket
client = socket.socket(socket.AF_INET,socket.SOCK_DGRAM)
client.connect(("localhost",1900))
client.send(b"Ce mai faci")

startDate = 2021
endDate = 2434
print("************************* Allowed years *****************************")
for i in range(startDate, endDate):
    print(i)
print("**********************************************************************")

import datetime

x = datetime.datetime.now()
print(x)

txt = "Ramin ce mai faci"[::-1]
print(txt)
'''
import socket

server = socket.socket(socket.AF_INET,socket.SOCK_DGRAM)
server.bind(("localhost",1900))
msg = server.recvfrom(16)
print(msg)

