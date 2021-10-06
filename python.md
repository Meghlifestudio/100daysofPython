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
## String concatenation: taking to strings and merging in one: How to add a variable between two variable.

# Example We have two word Hello world and Angela
print("Hello world" + "Angela")
Above code can't give you Space, Now for space we add one space in between(consider it as another string to add in middle of Hello world and Angela
print("Hello world"+ " "+"Angela")

## Debugging 
## Input Function
It is promt for the user

* Example 1
input("what is you name")
User type Angela

Now if we want to add to see output hello Angela
Print("hello" + ** input("what is you name") ** )
In above the bold part which we nested inside print function it will run first and give a name(string) to system and then 
# New output will come after heelo cancatenated

Hello Angela

# website Thonny to see how code is run one by one

* Example 2 Use of Len function
print( len( input("what is your name ")))

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

'''
print('welcome to brand name generator.')
city_name=input("which city you were grown up?\n")
pet_name= input('what is your pet name?\n')
band_name=("city_name" + "pet_name ")
print("Your brand name could be " + city_name + " " + pet_name )
'''


