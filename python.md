# Python

[Github MD Cheat Sheet](https://guides.github.com/pdfs/markdown-cheatsheet-online.pdf)

# Day 1

What is strings
text which we want to be shown with "" which shows where to start and end

## Playing with strings, make printing of text in two line by adding \n

# Example 
print("Hello world!\n Hello world")

output

''' Python
Hello world!
Helloworld!
'''
### String concatenation: taking to strings and merging in one: How to add a variable between two variable.
   We can pnly concatenate string not integer

### Example We have two word Hello world and Angela
print("Hello world" + "Angela")
Above code can't give you Space, Now for space we add one space in between(consider it as another string to add in middle of Hello world and Angela
print("Hello world"+ " "+"Angela")

# Debugging 
# Input Function
It is promt for the user

* Example 1
input("what is you name")
User type Angela

Now if we want to add to see output hello Angela
Print("hello" + ** input("what is you name") ** )
In above the bold part which we nested inside print function it will run first and give a name(string) to system and then 
### New output will come after hello cancatenated

Hello Angela

### website Thonny to see how code is run one by one

* Example 2 Use of Len function
```Python
print( len( input("what is your name ")))
```Python

So n above from input will run first give the name and then calculate the length


## Python Variables
Variable is something ehich can be changes or varied
If we want to get previous name Angela we cant retrieve whole data so call that we can store whole imput in a variable name

exmple: name= input("what is your name ")
Later we can refer this by calling name: print (name)


## Excercise DAY 1 Variable
tips add space, add number
user_name (add space in python we use underscore
length1= len(user_name) (number should be added at



the end of variable)

# Day 1 Project Name code generator

``` Python
print('welcome to brand name generator.')
city_name=input("which city you were grown up?\n")
pet_name= input('what is your pet name?\n')
band_name=("city_name" + "pet_name ")
print("Your brand name could be " + city_name + " " + pet_name )
```

# Day 2 : Data types, Subscripting

* Data Types
* String Text no number
* Integer : whole number    
* Boolean : true, false
* Float : decimal

## Subscripting
Pulling out character from the string we use square brackets []

Example: Output: l

```Python
print("Heello"[3])
```

## Strings and numbers

example: ("435" + "500") will give output 435500 and not sum because aything inside quotes is considered as text (String) not number

## Integer
435+500 =935
we can also use underscore for large numbers

## Float and undescore
45_0000 or 45_56.000

# Type Error, Data Types

## check data type: Use type function

``` Python
Print(type(num_char))
```
## Data Casting/ Data type changing

Inorder to add an integer to string convert first Integer to string, 
Use Str, int, float function to change data type
see below example

```python
num_char = len (input("what is your name?\n"))
new_num_char = str(num_char)
print("Your name has " + new_num_char + " characters.")
```

### Example: Adding two digits number 

```Python
two_digit_number = input("Type a two digit number: ")
print(type(two_digit_number))
first_digit=(two_digit_number [0])
second_digit= (two_digit_number [1]) 
result = int(first_digit)
me= int(second_digit)
result= result+ me
print(result)
```

# Mathematical operation

PEMDAS: Parenthesis, Exponential, Multiplication, Division, Addittion, Subsctraction
()
** 
* / 
+ -

## Example: get Height & weight input and show Body mass index to user 
BMI= weight / height *height

```
height = input("enter your height in m: ")
weight = input("enter your weight in kg: ")

BMI= int(weight)/float(height)**2
print(BMI)
print(int(BMI))
```
## ROUND off to nearest 2
Example
print(round(8/3,2))
solution 2.67
print(round(2.333333,2)
solution 2.33

## Floor Division: alway geting integer after division & not floating point
Example
Input
print(8//4)
Output: 2 

## use of mathemtical function and equal to add value to alreday define variable

Example: here we have to add in second step  3 to result of first step
```python
result= 9/3
result/=3
print(int(result))
#solution 1

score=4
score+=5
print(int(score))
#solution 9
```

# Project TIP calculator (Used Round and other function to format two two decimal number, F function)

``` Python
**input("welcome to tip calculator")
bill=float(input("what is your bill amount? $ "))
Tip=int(input("How much you want to  tip? 10, 13, or 16? "))
final_bill=Tip/100 * bill +bill
each_bill= (final_bill/7)
Bill=round(each_bill,2)
**Bill= "{:, 2f},format",(each_bill)**
print(f"Your final bill is {Bill} dollar")
```

         
#If/elif/else and multiple if statement

## in below case only one condition will run
if condition1:
do a
elif condition 2:
do b
else:
do c

## in below case all if condition will run

if condition 1:
do a
if condition 2:
do b
if condition 3
do c:


``` Python

# 🚨 Don't change the code below 👇
print("Welcome to Python Pizza Deliveries!")
size = input("What size pizza do you want? S, M, or L ")
bill=0
if size=="S":
  bill +=15
elif size=="M":
  bill +=20
else:
  bill +=25

add_pepperoni = input("Do you want pepperoni? Y or N ")
if add_pepperoni=="Y":
 if size=="S":
  bill+=2
else:
  bill +=3

extra_cheese = input("Do you want extra cheese? Y or N ")
if extra_cheese=="Y":
  bill+=1


print(f"Your final bill is ${bill}" )
# 🚨 Don't change the code above 👆

#Write your code below this line 👇

```


#LOGIVAL OPERATORS, Combining" if" condiition in one line

## AND operator

both condiition is true then entire line is true and  give output true if any one of the if false it comes false.

Example: a=10
if a>8 and a<12
true

## Or operator
if any one of the condiition is true the result is true, 
if both th econdition is false then result is false

## Not condition

it turns the condition opposite
 example: if its false it converts to true and vice a versa
 a=10
 Not a>10
 
it will be false but with not function it will be true

 
#  Lower function and Count function
Conver text into lower case
Example
"Angel",lower()
angel
Counts number os letter in text

e="Angel", count("e")
1 


##Example lower case, Count, logic operators, string and integer

```Python
# 🚨 Don't change the code below 👇
print("Welcome to the Love Calculator!")
name1 = input("What is your name? \n")

name2 = input("What is their name? \n")
lower_case_names=(name1+name2).lower()
print=lower_case_names
t=lower_case_names.count("t")
r=lower_case_names.count("r")
u=lower_case_names.count ("u")
e=lower_case_names.count ("e")
true= t + r + u + e

l=lower_case_names.count ("l")
o=lower_case_names.count ("o")
v=lower_case_names.count ("v")
e=lower_case_names.count ("e")
love= l + o + v + e
love_score= int(str(true)+ str(love))
print(love_score)

if (love_score<10) or (love_score>90):
  print(f"Your score is{love_score}, you go together like coke and memtos " )
elif (love_score>=40) and (love_score<=50):
   print(f"Your score is {love_score} " )
else:
  print(f"Your score is {love_score}" )

```

#Day 3 Project Treasure find

## ASCII art 
(ASCII) https://ascii.co.uk/art

```Python 
print('''
*******************************************************************************
          |                   |                  |                     |
 _________|________________.=""_;=.______________|_____________________|_______
|                   |  ,-"_,=""     `"=.|                  |
|___________________|__"=._o`"-._        `"=.______________|___________________
          |                `"=._o`"=._      _`"=._                     |
 _________|_____________________:=._o "=._."_.-="'"=.__________________|_______
|                   |    __.--" , ; `"=._o." ,-"""-._ ".   |
|___________________|_._"  ,. .` ` `` ,  `"-._"-._   ". '__|___________________
          |           |o`"=._` , "` `; .". ,  "-._"-._; ;              |
 _________|___________| ;`-.o`"=._; ." ` '`."\` . "-._ /_______________|_______
|                   | |o;    `"-.o`"=._``  '` " ,__.--o;   |
|___________________|_| ;     (#) `-.o `"=.`_.--"_o.-; ;___|___________________
____/______/______/___|o;._    "      `".o|o_.--"    ;o;____/______/______/____
/______/______/______/_"=._o--._        ; | ;        ; ;/______/______/______/_
____/______/______/______/__"=._o--._   ;o|o;     _._;o;____/______/______/____
/______/______/______/______/____"=._o._; | ;_.--"o.--"_/______/______/______/_
____/______/______/______/______/_____"=.o|o_.--""___/______/______/______/____
/______/______/______/______/______/______/______/______/______/______/_____ /
*******************************************************************************
''')
print("Welcome to Treasure Island.")
print("Your mission is to find the treasure.") 
choice1=input('You\'re at crossroad, where you want to go? Type "left" or Type "right" ').lower()

if choice1=="left":
  choice2=input('You are come to the corner of the lake. Type "swim" to swim across, Type "wait" to  wait for the boat').lower()
  if choice2=="wait":
    choice3=input('You\'saved yourself, choose "Red", "blue" or "yellow" color ').lower()
    if choice3=="blue":
     print("Congratulation you will be kissed by Meghna" )

    else: 
     print("You will spend night by Ghost" )
  else:
     print("You got eaten by meghna")
else:
  print("You fell into hole, your game is over")
 
 ```
 


