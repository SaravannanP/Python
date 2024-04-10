# Python

# double "" or single '' doesnt matter
print("Python")
print("####################################################################################")
#  Variable  = container for a value. 4 Datatypes
print("#2 (00:05:57​) variables ✘")
# String variable 
name  = "Bro" 
print(name)
# print datatype of variable 
print(type(name)) # <class 'str'>
print("Hello" + name) 

first_name = "Bro"
last_name = "Code" 
full_name = first_name + " " + last_name

print("Hello" + full_name)


# Integer 
age = 21
age = age + 1 # short cut age += 1
print(age) # 22 

print(type(age))  # <class 'int'>

# cant concat string type with int type.Need convert integer to string datatype using typecasting
print("Your age is " + str(age)) # str(age) converts the int variable to string  (String casting)

# float = floating point numbre (a decimal number)
height = 250.5
print(height)
print(type(height))  # <class 'float'>
print("Your height is " + str(height) + " cm")

# boolean 
human = False 
print(human)
print(type(human))
print("Are you a huamn ? " + str(human))
print("####################################################################################")
# multiple assignment - assign multiple variables at the same time with one line of code  
print("#3   (00:17:38​) multiple assignment 🔠")
# name1 = "Bro"
# age1 = 21
# attractive = True

name,age,attractive = "Bro", 21, True

print(name)
print(age)
print(attractive)

# if all same age assign all to 30 with = sign  
Spongebob = patrick = Sandy = Squidward = 30  
print("####################################################################################")
print("#4   (00:20:27​) string methods 〰️")

name = "bro code"
# retruns len of name 
print(len(name))

# returns index of captial B at index 0
print(name.find("o"))

# capitalizes first letter of the string 
print(name.capitalize())


# upper mkes the string all uppercase 
print(name.upper())

# lower makes the string lowercase 
print(name.lower())

# returns false 
print(name.isdigit())

# is alphanumeric 
print(name.isalpha())

# counts how many specific char in the string 
print(name.count("o"))

# replace char in the string 
print(name.replace("o","a"))

# display a string multiple times 
print(name * 3)

print("####################################################################################")
print("#5   (00:25:13​) type cast 💱")
# convert datatype to another
x = 1
y = 2.0
z = "3" 

x = float(x)
y = int(y)
z = int(z)

z = str(z) 

print(x) # 1.0 
print(int(y)) # change to int from float 
print(z* 3) # return 9 

#  again cannot concat str with int or flaot 

print("####################################################################################")
print("#6   (00:30:14​) user input ⌨️")

print("Questions below")
 
#name = input("What is your name ?:")
# convert string to int
#age = int(input("How old are you ?: "))
# convert string to float 
#height = float(input("How tall are you?: "))

#print(name)
#print(age)
#print(height)

print("####################################################################################")
print("#7   (00:36:50​) math functions 🧮")

# ensure that you import math 

import math 

pi = 3.15
x = 1 
y = 2
z = 3 

# rounds pi
print(round(pi))

#round up
print(math.ceil(pi))

#round down 
print(math.floor(pi))

# absolute value of pi 
print(abs(pi))

print(pow(pi,2))

print(math.sqrt(420))

print(max(x,y,z)) 

print(min(x,y,z))

print("####################################################################################")
print("#8   (00:40:58​) string slicing ✂️")

# slicing = create a substring by extracting elements from another string 
#           indexing[] or slice() 
#           [start:stop:step]

name = "Bro code"

# INDEXING 
first_name = name[0]  #returns B 
# stop index is exclusive so + 1 
first_name = name[0:3]  # shorthand [:3]
last_name = name[4:8]  # shorthand [4:]

# if step is 1 
# fancy_name = name[0:8:1] # display everything 

fancy_name = name[0:8:2] # (bocd) prints every third char 

# shorthand name[::2]

print(first_name)
print(last_name)
print(fancy_name)

reversed_name = name[::-1]
print(reversed_name)


# SLICE 
# use comma instead of colon
website = "http://google.com"
website2 = "http://wikipedia.com"

# inti slice object 
# count backwards for negative index starting with -1 
slice = slice(7,-4)


print(website[slice])
print(website2[slice])

print("####################################################################################")
print("#9   (00:51:52​) if statements 🤔")
# if statements = block of code that will execute if condition is true

#age = int(input("How old are you ?: "))
age = 3030

if  age == 100:
    print("old as fuck")
elif age >= 18: 
    print("You are an adult")
elif age < 0: 
    print("You haven't been born yet")
else: 
    print("You are a child!")

print("####################################################################################")
print("10 LOGICAL OPERATORS   58:19​")
# logical operators (and,or,not) = used to check if two or more statements are true
#temp = int(input("What is the temperature outside? : "))
temp = 30
if temp >= 0 and temp <= 30: 
    print("The temperature is good today!")
    print("go outside!")
elif temp < 0 or temp > 30: 
    print("The temperature is bad today")
    print("stay inside")
# not(expression )


print("####################################################################################")    
print("#11 (01:04:03​) while loops 🔄")

# while condition: 
     #do something 
# while 1 == 1 : 
        # print("infinite loop")
        
name = ""                   # None 
while len(name) == 0:        # while not Name: 
    name = input("What is your name? :"   )
print("Hello " + name)
        
print("####################################################################################")    
print("#12 (01:07:31​) for loops ➰")
import time 
# for loop =  a statement tahtw ill execute it's block of code 
#             a limited amount of time 
#              
#               while loop = unlimited 
#               for loop = limited 

for i in range(10): 
     print(i+1)     # 1-10 
for i in range(50,100+1,2): #(inclusive,exclusive,step)
     print(i)       # 50 - 100 by steps of 2 

# iterate through string 
for i in "Bro Code":
    print(i)


for seconds in range(10,0,-1):
    print(seconds)
    #time.sleep(1) # sleep for 1 second after each iteration 
print("Happy new year")

print("####################################################################################")
print("#13 (01:13:04​) nested loops ➿")
# nested loops = The "inner loops" will finish all of it iterations before finishing one iteration of
#                "outer loop"

#rows = int(input("How many rows? "))
rows = 5
#columns = int(input("How many columns? "))
columns = 5 
#symbol = input("Enter the symbol: ")
symbol = "$"

for i in range (rows):
    for j in range (columns):
        # end="" prevents cursor from moving to next line 
       print(symbol, end = "")
    print() 
    

print("####################################################################################")
print("#14 (01:17:08) break continue pass ⛔")
# loop Control statements = change a loops execution from its normal sequence 

# break = used to terminate the loop entirely
# continue = skips to next iteration of the loop 
# pass = does nothing, acts as a placeholder 

while True: 
    name = input("Enter your name: ")
    if name != "" :
        break

phone_number = "123-456-789"

for i in phone_number:
    if i == "-":
        continue
    print(i, end = "")
    
    
for i in range(1,21):
    if i == 13:
        pass 
    else :
        print(i) 


print("####################################################################################")
print("#15 (01:21:06​) lists 🧾")

#  list = used to store multiple items in a single variable 

food = ["pizza","hamburger","hotdog","spaghetti","pudding"]

print(food[0])

# change value at index 0 
food[0] = "sushi"

# add ice cream to end of list 
food.append("ice cream")

# remove hotdog value from list 
food.remove("hotdog")

# remove last element from list 
food.pop()

# add cake to index 0 
food.insert(0,"cake")

# sort in ascending order numerically or by letter 
food.sort()

# remove alll element in the list 
#food.clear()

for x in food:
    print(x)

print("####################################################################################")
print("#16 (01:26:58​) 2D lists 📜")
# 2d lists = list of lists 


drinks = ["coffee","soda","tea"]
dinner = ["pizza","hamburger","hotdog"]
dessert = ["cake","ice cream"]

food = [drinks,dinner,dessert]

print(food)
print(food[0]) # first list 
print(food[0][0]) # coffee 
print(food[1][2]) # hotdog 

print("####################################################################################")
print("#17 (01:30:47​) tuples 📄")
# tuple = Collection which is ordered and unchangeable 
#         used to group together related data 

student = ("Bro",21,"male")

print(student.count("Bro")) # 1 
print(student.index("male")) # 2 

for x in student: 
    print(x) 
    
if "Bro" in student: 
    print("Bro is here") 

print("####################################################################################")
print("#18 (01:33:47​) sets 🍴")
# set  = collection which is unordered, unindexed. No duplicate values 

utensils = {"fork","sppon","Knife"}
dishes = {"bowl","plate","cup","knife"}

# may no be seen in porper order when printed 
# faster than list to check if something in set
# doesnt allow duplicate values 

utensils.add("napkin")
utensils.remove("fork")
#utensils.clear()

# adds all the elemtns in dishes to utensils 
#utensils.update(dishes)

#dishes.update(utensils)

dinner_table = utensils.union(dishes)

for x in utensils:
    print(x) 

for x in dishes:
    print(x) 
    
for x in dinner_table:
    print(x)  

# prints what utensils has but dishes doesnt 
#print(utensils.difference(dishes))

# prints whatever is common 
print(utensils.intersection(dishes))

print("####################################################################################")
print("#19 (01:40:03​) dictionaries 📖")
#   dictionary = A changeable, unordered collection of unique key:value pairs 
#                Fast becaue they use hashing, allow us to access a value quickly 
#                Different from sets beacuse of key value pairs 
#                Dictionary is mutable 
capitals = {'USA':'Washington DC',
            'India' : 'New Dehli',
             'Russia': 'Moscow', 
             'China' : 'Beijing'}
             
capitals.update({'Germany':'Berlin'})
capitals.update({'USA':'Las Vegas'})
print(capitals.items())
capitals.pop('Germany') 
capitals.clear()

#print(capitals['Germany']) # Interrupts program flow if key not found 
print(capitals.get('Germany')) # safer way to access key 
print(capitals.keys())
print(capitals.values())
print(capitals.items())

for key,value in capitals.items():
    print(key,value) 


print("####################################################################################")
print("#20 (01:47:20​) indexing 📑")
# index operator [] = gives acces toa sequences's element (str,list,tuples)

name = "bro code"

if(name[0].islower()):
    name = name.capitalize() # capitalizes first letter  

first_name = name[:3].upper() # BRO
last_name = name[4:].lower() # code
last_character = name[-1] #!

print(first_name)
print(last_name)
print(last_character)

print("####################################################################################")
print("#21 (01:53:23​) functions")
# function = a block  of code which is executed only when it is called

# method singature (arguements) 
def hello(first_name,last_name,age):
    print("hello" + first_name+" "+last_name)
    print("you are " + str(age) + " years old")
    print("Have a nice day")
    
hello("Bro","Code",21)

print("####################################################################################")
print("#22 (02:02:03​) return statement 🔙")
# return statement = Functions send python values/objects back to the caller.
#                    These values/objects are knows as fuctions return value 

def multiply(number1, number2):
    return number1 * number2

x = multiply(6,8)

print(x) 

print("####################################################################################")
print("#23 (02:04:51) keyword arguments 🔑")
#arguements = arguments preceded by an identifier when we pass them to a function 
#             The order of the arguments doesnt matter, unlike positional arguments
#             Pytho knows the names of the arguments that our function receives 

def hello(first,middle,last):
    print("hello" + first+" "+middle + " " +last) 

hello("bro","dude","code")
hello(last="code",middle="Dude",first="Bro")

print("####################################################################################")
print("#24 (02:07:09​) nested function calls 🖇️")\
# nested function calls = function calls inside other function calls 
#                         Innermost function calls are resolved first 
#                         returned values is used as arguement for the next outer function 

num = input("Enter a whole positive number: ")
num = float(num)
num = abs(num)
num = round(num)
print(num) 

print(round(abs(float(input("Enter a whole positive number: ")))))

print("####################################################################################")
print("#25 (02:09:40​) variable scope 🔬")
# scope = the region that a varibale is recognized 
#          A variable is only available from inside the region it is created.
#          A global and locally scoped version of a variable can be created 
# L = local 
# E = Enclosing
# G = Global 
# B = Built-in 

name = "Bro" #global scope (available inside and outside function)

def display_name():
    name = "code"   # local scope(Available only inside this function)
    print(name)
 
display_name()
print(name)

print("####################################################################################")
print("#26 (02:13:23​) *args 📦")
# *args = paramenter that will pack all argument into a tuple 
#         usedful so that a function can accept a varying amount of arguments 


def add(*stuff):
    sum = 0
    # stuff = list(stuff)       created in order to change args value 
    # stuff[0] = 0              cant change any of the args values directly so create tuple
    for i  in stuff: 
        sum += i
    return sum 
 
print(add(1,2,3,4,5,6,7,8))
print("####################################################################################")
print("#27 (02:16:58​) **kwargs 🎁")

def hello(**kwargs):
    #print(" Hello" + title + "" + first + "" + middle + "" + last,end="")
    print(" Hello", end="")
    for key ,value in kwargs.items():
        print(value,end =" ") 

hello(title="Mr.",first="Bro" ,middle="Dude",last="code" )
print("####################################################################################")
print("#28 (02:21:17​) string format 💬")
# str.format() = optional method that gives users 
#                 more control when displaying output 
animal = "cow"
item = "moon"
#print("The " + animal + " jumped over the " + item)
print("The {} jumped over the {}".format(animal,item))
print("The {0} jumped over the {1}".format(animal,item)) #positional argument
print("The {animal} jumped over the {item}".format(animal="cow",item= "moon"))

text = "The {} jumped over the {}"
print(text.format(animal,item))
number = 1000
name = "Bro" 

print("Hello,my name is {}".format(name))
# pads 10 spaces after name 
print("Hello,my name is {:10}".format(name))
# right aligned 
print("Hello,my name is {:>10}".format(name))
# center align 
print("Hello,my name is {:^10}".format(name))

# 3 decimel place f represents floating point number 
print("The number is pi is {:.3f}".format(number))
# add comma at thousand place 
print("The number is pi is {:,}".format(number))
# binary repsentation 
print("The number is pi is {:b}".format(number))
# Octo number 
print("The number is pi is {:o}".format(number))
# in hexadecimal (lowercase x for lower case uppercase for all uppercase ) 
print("The number is pi is {:X}".format(number))
# scientific notation 
print("The number is pi is {:E}".format(number)) 

print("####################################################################################")
print("#29 (02:33:22​) random numbers 🎲")
# pseudo random 
import random 

# random num from 1-6
x = random.randint(1,6) 
y = random.random() 

print(x)
print(y)

myList = ['rock','paper','scissors']
z = random.choice(myList)
print(z)
 
cards = [1,2,3,4,5,6,7,8,9,"J","Q","K","A"]

random.shuffle(cards)

print(cards)

print("####################################################################################")
print("#30 (02:36:43​) exception handling ⚠️")
# exception = events detected duting execution that interrupt the floaw of a program 

try: 
    numerator = int(input("Enter a number to divide : "))
    denominator = int(input("Enter a number to divide by: "))
    result = numerator / denominator 
    
# better handle specific exception  
except ZeroDivisionError as e:
    print(e)
    print("cant divide by zero")
    
except ValueError as e :
    print(e)
    print("Eneter only numbers")
except Exception as e:
    print(e)
    print("Something went wrong")
else : 
# print reuslt if thre are no exceptions
    print(result)
finally:
    # if exception or not will always execute last 
    print("This will always execute")
    

print("####################################################################################")
print("#31 (02:43:40) file detection 📁")
import  os  # Important for 31-36 

# double slash for escape squence for string
path = "D:\\Stuff\\Stuff\\AI\\unapp"

if os.path.exists(path):
    print("That location exists!")
    if os.path.isfile(path):
        print("that is a file")
    elif os.path.isdir(path):
        print("That is a directory!")
else:
    print("That location doesn't exist!")
    
print("####################################################################################")
print("#32 (02:47:28​) read a file 🔍")

# with open closes file automatically
try : 
    with open("C:\\Users\\Sarav\\OneDrive\\Desktop\\Algos.txt") as file:
        print(file.read())
        #closes file automatically after opening then 
except FileNotFoundError:
    print("That file was not found ")
print(file.closed)

print("####################################################################################")
print("#33 (02:51:00​) write a file 📝")
text = " Yoooooooooooooo\nthis is some text\nhave a good one! \n"
# 'r' for read a file , 'a' for append 
with open("test.txt",'w') as file:
     file.write(text) 
     
print("####################################################################################")
print("#34 (02:53:45​) copy a file 🖨️")
# copyfile() = copies contents of a file 
# copy() = copfile()  + permission mode + destination can be a directory 
# copy2() = copy() + copies metadata(file's creation and modification times) 
import shutil

shutil.copyfile('C:\\Users\\Sarav\\OneDrive\\Desktop\\test.txt','C:\\Users\\Sarav\\OneDrive\\Desktop\\copy.txt') # arc , dest 

print("####################################################################################")
print("#35 (02:57:05​) move a file 🗃️")
source = "test.txt" # folder 
destination = "C:\\Users\\Sarav\\OneDrive\\Desktop\\test.txt"

try : 
      if os.path.exists(destination):
        print("There is already a file there")
      else: 
        os.replace(source,destination)
        print(source+ " was not found")
except FileNotFoundError:
    print(source+ " was not found")
print("####################################################################################")
print("#36 (03:01:20​) delete a file 🗑️")
path = "C:\\Users\\Sarav\\OneDrive\\Desktop\\test.txt"


try: 
    os.remove(path) # delete a file 
    #os.remdir(path) # delete a file or empty folder 
    #shutil.rmtree(path) # delete files and folders
except FileNotFoundError:
    print("File not found")
except PermissionError: 
    print("You do not have permissions to dlete that")
except OSError:
    print("That folder contains files")
else: 
    print(path + "deletion was sucessful")
print("####################################################################################")
print("#37 (03:06:15​) modules 💌")
# modeul = a file containing python code. May contain fucntion,classes etc
# used with modular programming ,whihc is to seperate program inot parts 

# import messages 
# import messages as makes
# from  messages import hello,bye 
# from messages import * (not reccomended) 

help("modules")

print("####################################################################################")
print("#38 (03:10:26) rock, paper, scissors game 🗿")
print("####################################################################################")
print("#39 (03:18:32​) quiz game 💯")
print("####################################################################################")
print("#40 (03:35:45​) Object Oriented Programming (OOP) 🐍")
# -----------------------------------
# Attributes describes what an obj is/has and methods is waht its does or actions

# classes have to start with capitalization 
# classes are a blueprint to creating objects 
class Car: 
    make = None
    model = None
    year = None 
    color = None
    # 41 class variables (declared within class but outside of constructor)
    # set up default value and change later 
    wheels = 4 # class variables 
    
    # construct objects (constructor) 
    def __init__(self,make,model,year,color):
        self.make = make    # instance variables 
        self.model = model  # instance variables 
        self.year = year    # instance variables 
        self.color = color  # instance variables 
        
    # self referst o the obj that is using this method 
    def drive(self): 
        print("This car is driving")
        print("This " + self.model + " is driving")
    def stop(self):
        print("This car is stopped")
        print("This " + self.model + " is stopped")
# if in another file then        
#from car import Car 

# dont need to pass in self that is done automaticatlly 
car_1 = Car("Chevy","Corvette",2021,"blue")
car_2 = Car("Ford","Mustang",2022,"red") 

print(car_1.make) 
print(car_1.model) 
print(car_1.year) 
print(car_1.color) 

print(car_2.make) 
print(car_2.model) 
print(car_2.year) 
print(car_2.color) 

car_1.drive()
car_2.stop() 



print("####################################################################################")
print("#41 (03:45:06​) class variables 🚗")
# check 40 for class blueprint 


Car.wheels = 4 # changes all blueprints
car_1.wheels = 2  # changes for that object 
print(Car.wheels)# shows 4 
print(car_1.wheels)# shows 2 
print(car_2.wheels)# whows 4 


print("####################################################################################")
print("#42 (03:48:54​) inheritance 👪")
# child class inherits common attributes and methods from parent class 
class Animal:

    alive = True 
    
    def eat(self):
        print("This animal is eating")
        
    def sleep(self):
        print("This animal is sleeping")
 
# child class  
class Rabbit(Animal):
# rabbit class inherits class variable Alive and eact() and sleep() methods 
    def run(self):
        print("This rabbit is running")
class Fish(Animal):
     def swim(self):
        print("This fish is swimming")
class Hawk(Animal):
    #pass
     def fly(self):
        print("This hawk is flying")
    
rabbit = Rabbit()
fish = Fish()
hawk = Hawk() 


print(rabbit.alive) 
fish.eat()
hawk.sleep()

rabbit.run()
fish.swim()
hawk.fly()

print("####################################################################################")
print("#43 (03:55:30​) multilevel inheritance 👴")
# multi-level inheritance = when a derived(child) class inherits another derived (child) class 

class Organism: 
    alive = True
    
class Animal(Organism):
    def eat(self):
        print("This animal is eating")
        
class Dog(Animal):
    def bark(self):
        print("The dog is barking")
        
dog = Dog()

print(dog.alive)
dog.eat()
dog.bark() 

print("####################################################################################")
print("#44 (03:58:32) multiple inheritance 👨‍👩‍👧‍👦")
# multiple inheritance = when a child class is derived from more than one parent class 

class Prey: 
    def flee(self):
        print("This animal flees")
class Predator:
    def hunt(self):
        print("this animal is hunting")
        
class Rabbit(Prey): 
    pass 
    
class Hawk(Predator):   
    pass 
     
class Fish(Prey,Predator):
    pass 
    
    
rabbit = Rabbit()
hawk = Hawk()
fish = Fish()
 
rabbit.flee()
hawk.hunt()
fish.flee()
fish.hunt()
print("####################################################################################")
print("#45 (04:01:49) method overriding 🙅")
# method overriding allows a sub clas to override something provided by parent class
class Animal:
    def eat(self):
        print("This animal is eating")
        
class Rabbit(Animal):
    def eat(self):
        print("This rabbit is eating a carrot")


rabbit = Rabbit()
rabbit.eat()

print("####################################################################################")
print("#46 (04:04:14​) method chaining ⛓️")
# Method chaining = calling multiple methods sequentaially 
#                   each call performs an action on the same object and returns self 

class Car:
    
    def turn_on(self):
        print("You start the engine")
        return self 
        # required for method chaining
        
    def drive(self):
        print("You drive the car")
        return self # required for method chaining
         
    def brake(self):
        print("You setp on the brakes ")
        return self # required for method chaining
         
    def turn_off(self):
        print("You stop the engine")
        return self # required for method chaining



car = Car()
car.turn_on().drive()
car.brake().turn_off()    

# \ is a line continuation character  
car.turn_on()\
    .drive()\
    .brake()\
    .turn_off() 
    
print("####################################################################################")
print("#47 (04:08:08) super function 🦸")
# super() = Function used to give access to the methods of a parent class.
#           Returns a temporay object of a parent class when used 

class Rectangle:
    #pass
    def __init__(self,length, width):
        self.length = length
        self.width = width 

class Square(Rectangle):
    def __init__(self,length,width):
            #self.length = length 
            #self.width = width 
            super().__init__(length,width)
    
    def area(self):
        return self.length * self.width

class Cube(Rectangle):
    def __init__(self,width,length,height):
                #self.length = length 
                #self.width = width
                self.height = height
                super().__init__(width,length)
    def volume(self):
        return self.length * self.width * self.height 
 
square = Square(3,3)
cube = Cube(3,3,3)
print(square.area())
print(cube.volume())

print("####################################################################################")
print("#48 (04:12:09​) abstract classes 👻")
# prevents a user from creating an object of that class
# + compels a user to override abstract methods in a child class 

# abstract class = a class which contains one or more abstract methods.
# abstract method = a method that has a declration but does not have an implementation.

# abc is acronym for abstract base class 
from abc import ABC, abstractmethod 

# abstract class 
class Vehicle(ABC):
# Need to have minimum one abstract method 
# abstract method declared butno implementation
    @abstractmethod
    def go(self):
        pass 
        
    @abstractmethod 
    def stop(self):
        pass 
        
class Car(Vehicle):
    # children class NEEDS to have abtract method from parent class overidden 
    def go(self):
        print("You drive the car")
    
    def stop(self):
        print("You stopped the car")
        
class Motorcycle(Vehicle):
    # children class NEEDS to have abtract method from parent class overidden 
    def go(self):
        print("You ride the motorcycle")
        
    def stop(self):
        print("You stopped the motorcycle")

# cant instantiate abstract vehicle with abstract methods 
#vehicle = Vehicle()
car = Car() 
motorcycle = Motorcycle()

#vehicle.go()
car.go()
motorcycle.go()

car.stop()
motorcycle.stop()


print("####################################################################################")
print("#49 (04:19:12) objects as arguments 🏍️")
class Car:
    color = None

class Motorcycle:
    
       color = None
  
def change_color(car,color):

    car.color = color
    
car_1 = Car()
car_2 = Car()
car_3 = Car()

bike_1 = Motorcycle()

print(car_1.color)
print(car_2.color)
print(car_3.color)
print(bike_1.color)

change_color(car_1,"red")
change_color(car_2,"white")
change_color(car_3,"blue")
change_color(bike_1,"Black")

print(car_1.color)
print(car_2.color)
print(car_3.color)
print(bike_1.color)


print("####################################################################################")
print("#50 (04:23:20​) duck typing 🦆")
# Duck typing = concept where the class of an object is less important than the methods/attributes 
#               the class might have
#               class type is not check if minimum methods/attributes are present 
#               "If it walks like a duck,and it quacks like a duck,then it must be a duck"

class Duck:
    def walk(self):
        print("This duck is walking")
    def talk(self):
        print("This duck is quacking")
        
class Chicken:
    def walk(self):
        print("This chicken is walking")
    def talk(self):
        print("This chicken is quacking")
        
        
class Person:
    # duck object specifically mentioned 
    def catch(self,duck):
        duck.walk()
        duck.talk()
        print("You caught the critter")
       
duck = Duck()
chicken = Chicken()
person = Person()

person.catch(duck)
# note chicken object passes instead of ducj and it still works
# both object need to have methods of the same name 
person.catch(chicken)

print("####################################################################################")
print("#51 (04:27:38) walrus operator 🦦")
# Walrus operator := 
# walrus operator 
# assigns values to variable as part of a larger expression 

happy = True 
print(happy) 

print(happy := True) 

# foods = list()
# while True:
    # food = input("What food do you like?: ")
        # if food = "quit":
            # break 
    # foods.append(food)
 
foods = list()
while food := input("What food do you like?: ") != "quit":
    foods.append(food)

print("####################################################################################")
print("#52 (04:31:45​) functions to variables 📛")
# assign function to variable in python 

def hello():
    print("Hello")

# prints memory address of fucntion  
print(hello)

hi = hello 
hello()
hi()  

say = print 
say("Whoa! I can't believe this works! :o")

print("####################################################################################")
print("#53 (04:35:21​) higher order functions 👑")
# Higher Order Function = a function that either:
#                         1. accepts a fucntion as an argument 
#                               or 
#                         2. returns a function 
#                           (In python, functions are also treated as objects)



def loud(text):
    return text.upper() 
def quiet(text):
    return text.lower()

# higher order func 
def hello(func):
    text = func("Hello")
    print(text) 
    
hello(loud) # HELLO 
hello(quiet) #hello 


# deividend (10) / Divisor (5) = quotient (2)
# divisor is the higher order function since its returning dividend 
def divisor(x):                 # 4:40:39 
    def dividend(y):
        return y/x 
    return dividend
    
    
divide = divisor(2) 
print(divide(10))
print("####################################################################################")
print("#54 (04:41:06​) lambda λ")

# lambda function = function written in 1 line using lamda keyword 
#                   accepts any number of arguments, but only has one expression.
#                   (Think of it as a shortcut)
#                   (useful if needed fir a short period of time, throw-away)
#   
# lambda parameters:expression 

# def double(x):
    # retrun x * 2 
    
# print(double(5)) 

double = lambda x: x * 2 
print(double(5))

multiply = lambda x,y: x * y
print(multiply(5,6)) 

add = lambda x,y,z : x + y + z 
print(add(1,2,3))

full_name = lambda first_name, last_name: first_name + "" + last_name
print(full_name)

age_check = lambda age: True if age >= 18 else False 
print(age_check(18))

print("####################################################################################")
print("#55 (04:45:44​) sort 🗄️")
# sort() method = used with lists 
# sort() function = used with iterables 


# list 
liststudents = ["Squidward""Sandy""Patrick","Spongebob","Mr.Krabs"]


liststudents.sort()
# liststudents.sort(key)
# liststudents.sort(reverse= True)  sorted by reverse alpha order 
for i in liststudents:
    print(i)
    
tuplestudents = ("Squidward""Sandy""Patrick","Spongebob","Mr.Krabs")    
sorted_students = sorted(tuplestudents)
sorted_students = sorted(tuplestudents,reverse=True)

for i in sorted_students:
    print(i)


# list of tuples 
students = [("Squidward","F",60),
            ("Sandy","A",33),
            ("Patrick","D",36),
            ("Spongebob","B",20),
            ("Mr.Krabs","C",60)]
students.sort()
# grade is a function object via lambda function
grade = lambda grades:grades[1]
students.sort(key=grade)
#students.sort(key=grade,reversed = True)

age = lambda ages:ages[2]
students.sort(key=age)
#students.sort(key=age,reversed = True)

# tuple of tuples 
students = (("Squidward","F",60),
            ("Sandy","A",33),
            ("Patrick","D",36),
            ("Spongebob","B",20),
            ("Mr.Krabs","C",60))
age = lambda ages:ages[2]
sorted_students = sorted(students,key=age)

for i in sorted_students:
    print(i)

print("####################################################################################")
print("#56 (04:53:22​) map 🗺️")
# map() = applies a function to each item in an iterable (list,tuple,etc)
#
# map(function,iterable)


# list of tuples 
store=[("shirt",20.00),
       ("pants",25.00),
       ("jackets",50.00),
       ("socks",10.00)]
 
to_euros = lambda data: (data[0],data[1]*0.82)
to_dollars = lambda data: (data[0],data[1]/0.82)

# convert map object to list 
store_euros = list(map(to_euros, store))
store_dollars = list(map(to_dollars, store))

for i in store_euros:
    print(i)
    
for i in store_dollars:
    print(i)

print("####################################################################################")
print("#57 (04:57:17​) filter 🍺")
# filter() = creates a collection of elements from an iterable for which a function returns True 
#
# filter(function,iterable)

friends = [("Rachel",19),("Monica",18),("Phoebe",17),("Joey",16),("Chandler",21),("Ross",20)]

age = lambda data:data[1] >= 18
 
drinking_buddies = list(filter(age,friends))
 
for i in drinking_buddies:
    print(i)

print("####################################################################################")
print("#58 (05:00:10​) reduce ♻️")
# reduce() = apply a function to an iterable and reduce it to a single cumulative value.
#            perfroms function on first two elements and repeats process untill 1 value remains 
#
# reduce(function,iterable) 

import functools 

letters = ["H","E","L","L","O"]
word = functools.reduce(lambda x,y :x + y,letters)
print(word)

# factorial = [5,4,3,2,1]
# result = functools.reduce(lambda x,y : x * y,factorial)
# print(result)



print("####################################################################################")
print("#59 (05:04:54​) list comprehensions 📰")



print("####################################################################################")
print("#60 (05:10:54) dictionary comprehensions 🕮")


print("####################################################################################")
print("#61 (05:18:59​) zip function 🤐")



print("####################################################################################")
print("#62 (05:23:41​) if _name_ == '__main__' ❓")


print("####################################################################################")
print("#63 (05:29:21​) time module ⌚")



print("####################################################################################")
print("#64 (05:39:58​) threading 🧵")


print("####################################################################################")
print("#65 (05:53:31​) daemon threads 😈")


print("####################################################################################")
print("#66 (05:58:19​) multiprocessing ⚡")

print("####################################################################################")


#93 (09:53:04​) clock program 🕒
#94 (10:01:03​) send an email 📧
#95 (10:07:37​) run with command prompt 👨‍💻
#96 (10:09:53) pip 🏗️
#97 (10:13:30) py to exe 🏃
#98 (10:17:13​) calculator program 🖩
#99 (10:31:38​) text editor program ✏️
#100 (11:05:51) tic tac toe game ⭕
#101 (11:26:25)​ snake game 🐍


def fibo(num): 
    if num <= 1:
        return num
    else :
        return fibo(num-1) + fibo(num-2)
        

print(fibo(2))
 
 
 
# def isLeap(year):
    # if year % 400 and year % 4 and not(year% 100) :True ? False: 
        
