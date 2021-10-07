# Python

[Github MD Cheat Sheet](https://guides.github.com/pdfs/markdown-cheatsheet-online.pdf)

# Day 1

What is strings
text which we want to be shown with "" which shows where to start and end

## Playing with strings, make printing of text in two line by adding \n

# Example 
print("Hello world!\n Hello world")

output

'''
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
length1= len(user_name) (number should be added at the end of variable)

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

