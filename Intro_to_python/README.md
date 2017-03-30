# Introduction to Python 

### Author : Sheryl Bernard

## Project Description 

"Introduction to Python" is a fun and interactive Mozilla Study Group to share skills and ideas on how to get a head start to Python language. This group is best for beginners, yet it is open to all. 

## Getting Set up 

-  Download [Python interpreter](https://www.python.org/downloads/) on your computer.

## What is Python ?

Python is :

-  General purpose programming language
* [High-level programming language](http://www.webopedia.com/TERM/H/high_level_language.html) 
* Easy to learn 
* Multiple programming paradigms, including object-oriented, imperative, functional programming, and procedural styles.
* Interpreted language 
* Fast 

## Basic Overview

Before we get started let’s go through some basics for Python:

* Variable : It stores a piece of value/string, and is given a specific name.
			variable_name1 = 67
			variable_name2 = "Taylor"

* Comments : For single line comment use #(pound), and for multiple line comment enclose whatever you want to comment in three quotes(''').

* Arithmetic Operators: 

|Operators   |	Meaning
|----------  |:------------------
|+		     |   Addition 
|-		     |   Subtraction
|*		     |   Multiplication
|/		     |   Division
|**		     |   Exponential
|%		     |   Modulus		

* Comparators: <br>
![comparisonoperators](https://cloud.githubusercontent.com/assets/20215525/24488402/3e5c9ff2-1534-11e7-979d-2ad2d46ce0bc.png)

* Keywords : These are reserved words and cannot be used to name constants or variables or identifier name. 
![keywords_python](https://cloud.githubusercontent.com/assets/20215525/24488404/4d7631ec-1534-11e7-9867-c69e44f2bcc6.png)

* print : print keyword is used to print anything like value/string on the console.

			print("Test this on my screen!")

* String: Strings are derived data types. A string in Python is a sequence of characters. Strings are immutable. This means that once defined, they cannot be changed. However many python methods, can modify strings. <br><br>
Some common string methods :
  + stringVar.lower() - returns the stringVar in lowercase,
like

		str = "THIS IS AN EXAMPLE"
		print str.lower()
    
       This would give output as:<br>
		this is an example	
			
   + stringVar.upper() - returns the stringVar in uppercase, 
like,

		str = "example"
		print str.upper()

     This would give output as:<br>
		EXAMPLE	

   + stringVar.replace('a', 'b') - replaces all occurrences of a with b in the string,
like

		str = "Mary had a Cat. Cat was of Mary."
		print str.replace("Mary","Cat")

    This would give output as:<br>
		Cat had a Mary.Mary was of Cat.		
  + len(stringVar) - returns length of the string

		str = "Test the length"

	This would give output as:<br>
		15	

	  Alternative of this is,<br>

		stringVar.count()
  + str(variableName) - This string method makes non-strings into strings,

		str(56)
		’56’   #Note that now 56 is a string not an integer 

* String index : Each character is string is assigned an index number started with 0.

![string_index](https://cloud.githubusercontent.com/assets/20215525/24488418/5e787694-1534-11e7-8519-9513644e5a88.png)

Assume, var_name = 'monkey'

Use following format to access the any character,
	var_name[index_number]
like, var_name[4]	for character 'e'
	

To access a group of characters, like 'onk',
	var_name[1:4]	

* isalpha() : This function returns True, if all characters are string,
else it returns False, if all characters are not string.
<code>
str = 'check'
print str.isalpha()   # this would give output as True
str = 'this is not all…string'
print str.isalpha()   # this would give output as False
</code>

* Module : It is a file that contains definitions, i.e. module can define functions, classes, and variables. Simply, it is a file consisting of Python code. Declared as 

		from module_name import function_name
For example, 		
	 from math import sqrt 
    
This command invokes ’sqrt’ function, which is included in 'math' module.
![python-modules](https://cloud.githubusercontent.com/assets/20215525/24488476/bf6b96ac-1534-11e7-8435-010c0b27809f.jpg)


* In Python, whitespace is used to structure code. Whitespace is important, so you have to be careful with how you use it.



## Running the first Hello World program

### Hello world program
```print('Hello World!')```
<br>

### How to compile and run
 
####For Windows:

* Write python code on an editor like Notepad.
* Create a folder on your computer to use for your Python programs, such as C:\pythonpractice, and save your hello.py program in that folder.
* In the Start menu, select "Run...", and type in cmd. This will cause the Windows terminal to open.
* Type cd \pythonpractice to change directory to your pythonpractice folder, and hit Enter.
* Type hello.py to run your program!

** Note: If it didn't work, make sure your PATH contains the python directory. See Getting Python.*

####For Mac:
* Write python code on an editor like TextEditor.
* Create a folder on your computer to use for your Python programs. A good suggestion would be to name it pythonpractice and place it in your Home folder. Save your hello.py program into this folder.
* Open the Applications folder, go into the Utilities folder, and open the Terminal program.
* Type cd pythonpractice to change directory to your pythonpractice folder, and hit Enter.
* Type python ./hello.py to run your program!

####For Linux:
* Write python code on an editor like sublime.
* Create a folder on your computer to use for your Python programs, such as ~/pythonpractice, and save your hello.py program in that folder.
* Open up the terminal program. 
* Type cd ~/pythonpractice to change directory to your pythonpractice folder, and hit Enter.
* Type python ./hello.py to run your program!


**Note : Otherwise, users can write code on any other [IDE](http://searchsoftwarequality.techtarget.com/definition/integrated-development-environment) like [PyCharm](https://www.jetbrains.com/pycharm/download/#section=mac).  **


## Conditional statements

These are used to perform different computations or actions depending on whether a condition evaluates to true or false (Please note that true and false are always written as True and False in Python).

 # If statements 
	* if some-condition:
		#block code one
		#block code two*
 # If - else statements 
	* if some-condition:
		#block code one
		#block code two
	  else:
	 	#block code three *
 # Elif statement
	* if some-condition:
		#block code one
		#block code two
	  elif some-condition:           //elif is short for else if
		#block code three
	  else:
	 	#block code four *		 


## Functions 

Function is a block of code that can be reused to perform single,related action.
It majorly includes the following components:

* Function block begins with the keyword **def**, followed by the function name and parentheses() and semicolon:.

* Any input [parameter or argument](http://stackoverflow.com/questions/156767/whats-the-difference-between-an-argument-and-a-parameter) should be placed within the parentheses. Yet, this is not compulsory.

* Then comes the body which describes the procedure the function carries out. 

###Calling of function 

Once the basic structure of a function is finalized, you can execute it by calling it from another function or directly from the Python prompt.

*Syntax:*
 		# Basic structure of function
		def function_name():
		    ***Comments***
		    #Body of function

		

### Anonymous Lambda function 

These functions are called anonymous because they are not declared in the standard manner by using the def keyword. Lambda functions can have any number of arguments but only one expression. The expression is evaluated and returned. Lambda functions can be used wherever function objects are required.

*Syntax*
		lambda[arg1,arg2,arg3,….argn]:expression


###Lists

List is like [array](https://techterms.com/definition/array). It is a collection of different data-type variables. 
![lists](https://cloud.githubusercontent.com/assets/20215525/24488520/07ab8e04-1535-11e7-913b-07feb00e1571.png)


* To access element of list

	*list_name[index_number]*

* To add elements, this would add at the end of the list
	
	*list_name.append(value)*

* To insert data at a specific desired place in the list

	*list_name.insert(index_number,"element_to_be_added")*

* To delete/remove elements of the lists

	*del list_name[index_number]*
			<br><center> OR</center>

	*del list_name                     //deletes entire list*
			 <br><center> OR</center>

	*list_name.remove("element_to_be_removed")*

* Some other methods that can be applied on the list:

Method   |   Functionality
---------|: --------------------
append() | Add an element to the end of the list
extend() | Add all elements of a list to the another list
insert() | Insert an item at the defined index
remove() | Removes an item from the list
pop() | Removes and returns an element at the given index
clear() | Removes all items from the list
index() | Returns the index of the first matched item
count() | Returns the count of number of items passed as an argument
sort() | Sort items in a list in ascending order
reverse() | Reverse the order of items in the list
copy() | Returns a shallow copy of the list



##Looping

###For Loop

For loop in Python is used to iterate over a sequence (list, tuple, string) or other iterable objects. Iterating over a sequence is called traversal.

*Syntax*
		for variable in sequence:
			#block-code

![forloop](https://cloud.githubusercontent.com/assets/20215525/24488440/880f1c60-1534-11e7-89e1-23cbea4b5e43.jpg)


###While Loop

The while loop in Python is used to iterate over a block of code as long as the test expression (condition) is true. It is an alternative for 'for-loop'.

*Syntax*
		while condition:
		    #execute block code1
		else:
		    #execute block code

If the while condition is True, execute block code1 is executed. Otherwise, else part is executed.

## Reference link
* [Learn python](http://stock.ethop.org/pdf/python/Learning%20Python,%205th%20Edition.pdf)

<br><br>

Happy Learning!<br>
![python_snake](https://cloud.githubusercontent.com/assets/20215525/24488447/96ec46ae-1534-11e7-81cc-b0becbf84ebc.jpg)

	
