# Python
Python Tasks – Day2
1.Install vim and execute a hello world script using powershell a.Python installation link - https://youtu.be/M5ILgNI0iXw (first 20 minutes) b.Vim Installation link - https://youtu.be/SBOFnzVuzOE 2.

Use Jupyter Notebook to execute following code, try to guess what is happing in this code 3.Write down above code using vim on same working directory, and execute it using python interpreter, tell us difference between jupyter and notepad 4.Write Down difference between interpreter and compiler 5.What is Data Structure, why we need one in programs? 6.Run all python (.py) files inside day2 folder on drive, try understanding code beneath each scripts, you will going to create those scripts by yourself in future lecture

#2
import numpy as np
import matplotlib.pyplot as plt
height = np.random.normal(140, 20, 1000)
plt.figure(dpi=200)
plt.title("Height Distribuion")
plt.xlabel("Height (cm) ")
plt.ylabel("Frequency")
plt.hist(height, bins=30, ec="gold")
plt.show()

#3
Difference beteween jupyter and notepad:
    
notepad-Notepad is a generic text editor included with all versions of Microsoft Windows that lets you 
        create, open, and read plaintext files with a .txt file extension. If the file contains 
        special formatting or is not a plaintext file, it cannot be read in Notepad.
        
jupyter-Jupyter is a free, open-source project that supports interactive computing across all programming languages. 
        It provides tools such as JupyterLab and Jupyter Notebook for creating and sharing computational 
        documents, with support for over 40 programming languages including Python, R etc.
        
​
#4
Difference between interpreter and compiler:
​
Interpreter:-                                      
1.Translates program one statement at a time.    
​
2.Interpreters usually take less amount of time to analyze the source code.
  However, the overall execution time is comparatively slower than compilers.
    
3.No Object Code is generated, hence are memory efficient.
​
4.Programming languages like JavaScript, Python, Ruby use interpreters.
​
Compiler:-
1.Scans the entire program and translates it as a whole into machine code.
​
2.Compilers usually take a large amount of time to analyze the source code. 
  However, the overall execution time is comparatively faster than interpreters.
​
3.Generates Object Code which further requires linking, hence requires more memory.
​
4.Programming languages like C, C++, Java use compilers.
    
,stack,linked list,hash maps,trees etc.
#5
#.What is Data Structure, why we need one in programs? 
In computer science, a data structure is a way of organizing and storing data in a computer program 
so that it can be accessed and used efficiently. Data structures provide a means of managing large amounts of data,
enabling efficient searching, sorting, insertion, and deletion of data.
​
EX-array ,queue,stack,linked list,hash maps,trees etc.
Python Tasks – Day3
What are Data Structures? List some of data structures and their use in real world application? 2.Read till Chapter-1 to Chapter - 5 from book I shared called Learning Python 3.Create a list data type and store names of your friends in it (at least 5), check out what are methods available in list data type, try to figure out their working using help function in python. 4.What is difference between ordered data type and unordered data type? 5.Write down types of each value given? (In python) a.100 b.105.5 c.192.56j d.10+6j e.‘10’ f.‘Hello world’5 g.[ 10, 20, 50, 100] h.{‘name’: ‘sachin’, ‘age’: 24, ‘language’: ‘python’}
#4
#difference between ordered data type and unordered data type:-
​
In Python, the lists, strings and tuples are ordered collection of objects and sets and dictionaries 
are unordered collection of objects.
dictionary
#5
(In python) 
​
a.100 -integer
b.105.5 -float
c.192.56j -complex
d.10+6j -complex
e.‘10’ -string
f.‘Hello world’5 -string
g.[ 10, 20, 50, 100] -list 
h.{‘name’: ‘sachin’, ‘age’: 24, ‘language’: ‘python’} -dictionary
Python Tasks – Day4
1.Explore split, strip, replace, center, title methods of string data type in python 2.Explore append, pop, remove, sort methods of list data type 3.Create 5 real time lists to store some useful information in python eg. Language = [ ‘java’, ‘c’, ‘c++’, ‘ruby’ ] 4.What is difference between mutable and immutable data types in python 5.What are identifiers, list rules of identifiers in python

#1
string="hello world iron man ###123lol"
print(string.split())
['hello', 'world', 'iron', 'man', '###123lol']
str="    hello world          " #strip removes all leading and trailing spaces
print(str.strip())
Type Markdown and LaTeX: 𝛼2
str1="I love D.C comics"
x=str1.replace("D.C","Avengers")
print(x)
I love Avengers comics
str2="Physics"
str2.center(20)#center alignment
'      Physics       '
str3="blazing sun"
str3.title() 
#The title() method returns a string where the first character in every word is upper case. Like a header, or a title.
'Blazing Sun'
#2
​
#L=[] empty list OR L=list()
L1=['parthiv','ravi']
​
#append or adding element to list
L1.append("rani")
for a in L1:
    print(a)
​
parthiv
ravi
rani
L1.pop()
for a in L1:
    print(a)
    
parthiv
ravi
L2=list("Avengers")
for a in L2:
    print(a)
print("------------------------------------------------------------------------------")
L2.pop()#s deleted
L2.pop(2)#e deleted
​
for a in L2:
    print(a)
A
v
e
n
g
e
r
s
------------------------------------------------------------------------------
A
v
n
g
e
r
L3=['a','aza','avaba','b','b','a','c','c','a','aza']
L3.remove('a')#removes first occurence of item in list
for a in L3:
    print(a)
print("---------------------------------------")
​
L2.insert(2,'e')
for a in L2:
    print(a)
print("---------------------------------------")
​
L2.remove('e')
for a in L2:
    print(a)
​
aza
avaba
b
b
a
c
c
a
aza
---------------------------------------
A
v
e
e
n
g
e
r
---------------------------------------
A
v
e
n
g
e
r
L=list(input("enter list elements of single digit integer type"))
for a in L:
    print(a)
    
print("----------------------------------------")
L.sort()
for a in L:
    print(a)
​
​
enter list elements of single digit integer type5467283454484930
5
4
6
7
2
8
3
4
5
4
4
8
4
9
3
0
----------------------------------------
0
2
3
3
4
4
4
4
4
5
5
6
7
8
8
9
#3
Language=["Jva",'C',"c++","ruby"] # "" or ''
for a in Language:
    print(a)
​
Jva
C
c++
ruby
#4
Mutable data types are changable data .EX-list,dictionary,set
Immutable datatypes are not changable data.EX-int,float,complex,string,tuple.
​
#5
Indentifiers are variables,which points to identify an object or value.
​
Ex-Student="Jacob".
here, Value/Jacob is an object of class String.
here, Variable/Student is an identifier pointing to an object of class String.
Python Tasks – Day5
1.What is difference between shallow copy and deep copy? 2.You want to create a library management application, you need to store data about books, students in your program, how will you store data inside python using list? Create some lists with fake data to store information about library management. 3.This chapter introduced assignment statements, like spam = 10. What is the difference between an expression and a statement? 4.Define following a.Atomic data types / Primary data types b.Secondary data type / User Defined Data Type 5.What is UDF?

#1
string="hello python"
string.islower()
True
print(string.upper())
print(string)
HELLO PYTHON
hello python
#1
colours=['red','blue','green']
b=colours #shallow copy   colors,b->|red|blue|green|
b=list(colours)#true copy or deep copy  colors->|red|blue|green| ,b->|red|blue|green|
​
#2
n=int(input("enter total no of students"))
c=0
for i in range(0,n): 
    x1=input("enter student name")
    x2=input("enter book name")
    list=[x1,x2]
    if(c==0):
        list1=list
        c=c+1
    else:
        list.append(list1)
    
    
for a in list:
    print(a)
    
enter total no of students3
enter student namep
enter book nameb
enter student namer
enter book namebo
enter student namem
enter book nameboo
m
boo
['p', 'b']
#3
Statement do not necessarily return values.
Statement are exceuted by compiler
int oddnum=5 #statement
​
expression returns a value.
Expressions are a part of statement and is evaluated by compiler 
a=a+1,c=a+b,100*(25+1)#expression
#4
primary data type-primary data type are pre-defined aldready exist in python programing
ex-boolean,integer,float,complex,tuple,string,list ,dictionary
​
user defined data type-data type is defined by programmer or user.
ex-linked-list,stack,queue,tree,graph,hashmap
#5
UDF-User defined function
ex-
def temp_c_to_f(f):
    f=((9*c)/5)+32
    return f
temp_c_to_f is a UDF
​
Python Tasks – Day6
1.Write down 10 projects ideas you want to implement using python 2.Create at list 5 objects using list, dictionary, it will be good if you store realistic data
3.What is duck typing in python, what are Dunder or special methods? 4.What are operators? How many types of operators are there in python?

Python Tasks – Day8
1.What are the two values of the Boolean data type? How do you write them? 2.What are the three Boolean operators? 3.Write out the truth tables of each Boolean operator (that is, every possible combination of Boolean values for the operator and what they evaluate to). 4. What do the following expressions evaluate to? (5 > 4) and (3 == 5) not (5 > 4) (5 > 4) or (3 == 5) not ((5 > 4) or (3 == 5)) (True and True) and (True == False) (not False) or (not True) 5. What are the six comparison operators? 6.What is the difference between the equal to operator and the assignment operator? 7.Explain what a condition is and where you would use one.

#1
Two values of boolean data type is true and false.We represent it as 1 and 0 respectively.
​
#2
three boolean operators
AND-and
OR-or
NOT-not
​
#3
AND     OR     NOT
T T-T |T T-T | T -F
T F-F |T F-T | F -T
F T-F |F T-T |
F F-F |F F-F |
​
#4
AND-SERIES, OR-PARALLEL
(5 > 4) and (3 == 5)#->T & F ->F-0
not (5 > 4) #-> false -0
(5 > 4) or (3 == 5)#->T || F ->T -1
not ((5 > 4) or (3 == 5))# -> not( T || f) -> not(t) ->f -0
(True and True) and (True == False)# ->f -0
(not False) or (not True)#-> t -1
​
#5
6 comparision operators
>,<,=,>=,<=,==
​
#6
Difference between equal-to operator and assignment operator:
    
assignment operator  (a=5)- assigns value to a variable
equal-to operator  (a==b)- compares value of variables
Python Tasks – Day9
1.Write a Python program to check whether a number is negative, positive or zero. 2.Write a Python program to check whether a number is divisible by 5 and 11 or not. 3.Write a Python program to check whether a year is leap year or not. 4.Write a Python program to check whether a character is alphabet or not. 5.Write a Python program to input any alphabet and check whether it is vowel or consonant. 6.Write a Python program to input any character and check whether it is alphabet, digit or special character. 7.Write a Python program to check whether a character is uppercase or lowercase alphabet. 8.Write a Python program to input week number and print weekday. 9.Write a Python program to input angles of a triangle and check whether triangle is valid or not. 10.Write a Python program to input all sides of a triangle and check whether triangle is valid or not. 11.Write a Python program to check whether the triangle is equilateral, isosceles or scalene triangle. 12.Write a Python program to input marks of five subjects Physics, Chemistry, Biology, Mathematics and Computer. Calculate percentage and grade according to following: Percentage >= 90% : Grade A Percentage >= 80% : Grade B Percentage >= 70% : Grade C Percentage >= 60% : Grade D Percentage >= 40% : Grade E Percentage < 40% : Grade F 13.Write a Python program to input basic salary of an employee and calculate its Gross salary according to following: Basic Salary <= 10000 : HRA = 20%, DA = 80% Basic Salary <= 20000 : HRA = 25%, DA = 90% Basic Salary > 20000 : HRA = 30%, DA = 95% 14.Write a Python Program to input electricity unit charges and calculate total electricity bill according to the given condition: For first 50 units Rs. 0.50/unit For next 100 units Rs. 0.75/unit For next 100 units Rs. 1.20/unit For unit above 250 Rs. 1.50/unit An additional surcharge of 20% is added to the bill

#1
a=int(input("enter number"))
​
if(a>0):
    print("positive")
elif(a==0):
    print("negative")
else:
    print("negative")
    
    
enter number-6
negative
#2
a=int(input("enter number"))
​
if((a%10==0 or a%5==0) and (a%11==0)):
    print("divisible by both 5 and 11")
elif(a%10==0 or a%5==0):
    print("divisible by 5")
elif(a%11==0):
    print("divisible by 11")
else:
    print("Not divisible by 5 and 11")
​
enter number16
Not divisible by 5 and 11
#3
a=int(input("enter number"))
​
if(a%4==0 or a%100==0 or a%400==0):
    print("leap year")
​
else:
    print("Not leap year")
​
enter number1004
leap year
#4
a=input("enter word")
​
b=a.isalpha()
print(b)
if(b==1):
    print("alphabet")
else:
    print("not alphabet")
    
enter a numbersddfgh
True
alphabet
#5
def vowel_or_consonant(x):
    if(x=="a" or x=="e" or x=="i" or x=="o" or x=="u"):
        print("vowel")
    else:
        print("consonant")
        
​
        
a=input("enter a character")
​
vowel_or_consonant(a)  
​
enter a characterx
consonant
#6
a=input("enter alphabet,digit or special character")
​
if(a.isalpha()==1):
    print("alphabet")
elif(a.isdigit()==1):
    print("digit")
else:
    print("special chracter")
enter alphabet,digit or special character#
special chracter
#6
a=input("enter alphabet,digit or special character")
​
if((a>='a' and a<='z') or (a>='A' and a<='Z')):
    print("Alpphabet")
elif(a>='0' and a<='9'):
    print("digit")
else:
    print("special character")
enter alphabet,digit or special character2
digit
#7
a=input("enter alphabet to chcek lowercase or uppercase\n")
​
if(a.islower()==1):
    print("lowercase alphabet")
elif(a.isupper()==1):
    print("uppercase alphabet")
enter alphabet to chcek lowercase or uppercase
w
lowercase alphabet
#8
# Python program to input week number and print week day
weekday = int(input("Enter weekday number (1-7) : "))
​
if weekday == 1 :
    print("\nMonday");
​
elif weekday == 2 :
    print("\nTuesday")
​
elif(weekday == 3) :
    print("\nWednesday")
​
elif(weekday == 4) :
    print("\nThursday")
​
elif(weekday == 5) :
    print("\nFriday")
​
elif(weekday == 6) :
    print("\nSaturday")
​
elif (weekday == 7) :
    print("\nSunday")
​
else :
    print("\nPlease enter any weekday number (1-7)")
Enter weekday number (1-7) : 5

Friday
#9
print("enter the angles of a triangle of three sides in degrees")
a=int(input())
b=int(input())
c=int(input())
if(a+b+c==180):
    print("polygon is triangle")
else:
    print("not triangle")
​
enter the angles of a triangle of three sides in degrees
60
40
80
polygon is triangle
#10
print("enter 3 sides of a triangle")
a=int(input())
b=int(input())
c=int(input())
if(a+b>c and b+c>a and a+c>b):
    print("polygon is triangle")
else:
    print("not triangle")
enter 3 sides of a triangle
3
4
5
polygon is triangle
#11
print("Input lengths of the triangle sides: ")
x = int(input("x: "))
y = int(input("y: "))
z = int(input("z: "))
​
if x == y == z:
    print("Equilateral triangle")
elif x==y or y==z or z==x:
    print("isosceles triangle")
else:
    print("Scalene triangle")
Input lengths of the triangle sides: 
x: 2
y: 2
z: 3
isosceles triangle
#12
print("enter marks of five subject out of 100")
a=int(input("physics:\n"))
b=int(input("chemistry:\n"))
c=int(input("biology:\n"))
d=int(input("maths:\n"))
e=int(input("computer:\n"))
​
Percentage=((a+b+c+d+e)/500)*100
print("Percentage:",Percentage,"%\n")
if(Percentage >= 90): 
    print("Grade A")
elif(Percentage >= 80):
    print("Grade B") 
elif(Percentage >= 70):
    print("Grade C") 
elif(Percentage >= 60) :
    print("Grade D") 
elif(Percentage >= 40 ):
    print("Grade E") 
elif(Percentage < 40 ):
    print("Grade F")
​
​
enter marks of five subject out of 100
physics:
40
chemistry:
50
biology:
60
maths:
70
computer:
80
Percentage: 60.0 %

Grade D
#13
b=int(input("enter basic salary"))
​
if(b<= 10000 ):
    HRA = 20
    DA = 80 
elif(b<= 20000) :
    HRA = 25
    DA = 90 
elif(b> 20000) :
    HRA = 30
    DA = 95
​
total=b+HRA*b+DA*b
print("HRA-",HRA,"%","DA-",DA,"%\n")
print("total salary-",total)
enter basic salary1000000
HRA- 30 % DA- 95 %

total salary- 126000000
#14
# Python Program to Calculate Electricity Bill
 
units = int(input(" Please enter Number of Units you Consumed : "))
​
if(units < 50):
    amount = units * 2.60
    surcharge = 25
elif(units <= 100):
    amount = 130 + ((units - 50) * 3.25)
    surcharge = 35
elif(units <= 200):
    amount = 130 + 162.50 + ((units - 100) * 5.26)
    surcharge = 45
else:
    amount = 130 + 162.50 + 526 + ((units - 200) * 8.45)
    surcharge = 75
​
total = amount + surcharge
print("\nElectricity Bill = %.2f"  %total)
 Please enter Number of Units you Consumed : 79

Electricity Bill = 259.25
Python Tasks – Day10
1.Python Program to Check Palindrome Number 2.Python Program to Print all multiples of 3 and 5 in an Interval 3.Python Program to Find the Factorial of a Number 4.Python Program to Print the Fibonacci sequence 5.Python Program to Check Armstrong Number

#1
a=int(input("enter a number"))
n=a
s=0
while(n>0):
    r=n%10
    s=s*10+r
    n=n//10 #/->float //->int
        
if(a==s):
    print("Palindrome")
else:
    print("not palindrome")
enter a number14641
Palindrome
#2
print("enter interval ;lower limit and upper limit; multiples of 3 and 5")
n1=int(input("enter lower limit"))
n2=int(input("enter upper limit"))
​
for i in range (n1,n2+1):
    if(i%3==0)or(i%5==0):
        print(i,",",end='')
        
enter interval ;lower limit and upper limit; multiples of 3 and 5
enter lower limit12
enter upper limit50
12 ,15 ,18 ,20 ,21 ,24 ,25 ,27 ,30 ,33 ,35 ,36 ,39 ,40 ,42 ,45 ,48 ,50 ,
#3
n=int(input("enter factorial of a number"))
f=1
for i in range(1,n+1):
    f=f*i
    
print(f)
enter factorial of a number5
120
#4
n=int(input("enter limit for fibonnaci series")) 
a=0
b=1
print(a,",",end='')
print(b,",",end='')
for i in range(1,n+1):
    c=a+b
    print(c,",",end='')
    a=b
    b=c
​
enter limit for fibonnaci series20
0 ,1 ,1 ,2 ,3 ,5 ,8 ,13 ,21 ,34 ,55 ,89 ,144 ,233 ,377 ,610 ,987 ,1597 ,2584 ,4181 ,6765 ,10946 ,
#5
a=int(input("enter a number"))
n=a
s=0
while(n>0):
    r=n%10
    s=s+r*r*r
    n=n//10 #/->float //->int
        
if(a==s):
    print("Armstrong")
else:
    print("not armstrong")
enter a number153
Armstrong
Python Tasks – Day11
1.Write Python Code to print these patterns

2.Write Python Code to print these patterns

3.Write Python Code to print these patterns

4.Write Python Code to print these patterns

5.Write Python Code to print these patterns

# Python Tasks – Day12
1.Write a code to implement Guess Game Guess Game
constraints / Rules
you have 5 chance to guess correct number which is choosen by computer / friend
Range which is allowed to select a number 1-50
After each guess you should give some tips / hints to user to improve their chance of winning
for example if user guess a number which is higher than actual number you should say `hint: think a low number!
if user guess a number which is lower than actual number you should say `hint: think a big number!`
      if user wins we will show a congrats messege and stop our game
      if any time user guess is out of limit than print a warning message saying Think in Limits 1-50 only!
      but we do not count this as a chance
2.Solve this problem https://www.hackerrank.com/challenges/list-comprehensions/problem 
3.Solve this problem https://www.hackerrank.com/challenges/python-lists/problem 
4.Solve this problem https://www.hackerrank.com/challenges/finding-the-percentage/problem 
5.Write a program to sort a list without using inbuilt functions (list.sort not allowed)
a.Using Bubble Sort Algorithm
b.Using Insertion Sort Algorithm 
c.Using Selection Sort Algorithm
#1
import random
print("enter interval for guessing nummber")
print("ONLY 5 CHANCES.")
l=int(input("enter lower limit of interval"))
u=int(input("enter upper limit of interval"))
​
#random number by computer within l and u
x=random.randint(l,u)#built-in function
print(x)
​
for i in range (1,6):
    print("Guess number;chance",i,":\n")
    a=int(input())
    if(a==x):
        print("Congratulation!u won.")
        break
    elif(a>x):
        print("hint:think lower")
    elif(a<x):
        print("hint:think higher")
        
if(a!=x):
    print("Better luck next time.U lose!!")
​
​
​
enter interval for guessing nummber
ONLY 5 CHANCES.
enter lower limit of interval15
enter upper limit of interval100
57
Guess number;chance 1 :

57
Congratulation!u won.
#3
def insert(x):
    list.append(x)
print("1.insert i e: Insert integer  at position")
print("2.print: Print the list.")
print("3.remove e: Delete the first occurrence of integer ")
print("4.append e: Insert integer  at the end of the list.")
print("5.sort: Sort the list.")
print("6.pop: Pop the last element from the list.")
print("7.reverse: Reverse the list.")
​
Python Tasks – Day13
1.Write a Python Code to count the Number of Each Vowel in a given string 2.Write a Python Code to count number of words, characters and number of spaces in a given stirng 3.Write a Python Program to remove punctuation from a given string (using loop) 4.Write a Python Program to take a mxn matrix input from user and stored in nested list 5.Write a Python Program to add, multiply and transpose two matrices given by user

#1
string=input("enter string")
l1=list(string)
c=1
for a in l1:
    if(a=='a' or a=='e'or a=='i' or a=='o' or a=='u' or a=='A' or a=='E' or a=='I' or a=='O' or a=='U'):
        c=c+1
​
print("No of vowel in string",string,"is:",c)        
        
        
enter stringasdfghji
No of vowel in string asdfghji is: 3
#2
wordCount=0
charCount=0
str=input("Enter the string\n")
split_str=str.split()
wordCount=len(split_str)
for word in split_str:
    charCount+=len(word)
print("Total words in the given string ",wordCount)
print("Total characters in the given string ",charCount)
print("Number of space in the given string ",(wordCount-1))
Enter the string
welcome everyone to wonderland
Total words in the given string  4
Total characters in the given string  27
Number of space in the given string  3
#3
​
# Python code to demonstrate working of
# Removing punctuations in string
# Using loop + punctuation string
​
# initializing string
test_str = "Gfg, is best : for ! petho ;"
​
# printing original string
print("The original string is : " + test_str)
​
# initializing punctuations string
punc = '''!()-[]{};:'"\,<>./?@#$%^&*_~'''
res=" "
# Removing punctuations in string
# Using loop + punctuation string
for ele in test_str:
    if ele not in punc:
        res+=ele
​
# printing result
print("The string after punctuation filter : " + res)
​
The original string is : Gfg, is best : for ! petho ;
The string after punctuation filter :  Gfg is best  for  petho 
#4
# A basic code for matrix input from user
​
R = int(input("Enter the number of rows:"))
C = int(input("Enter the number of columns:"))
​
# Initialize matrix
matrix = []
print("Enter the entries rowwise:")
​
# For user input
for i in range(R):    # A for loop for row entries
    a =[]
    for j in range(C):  # A for loop for column entries
        a.append(int(input()))
    matrix.append(a)
​
# For printing the matrix
for i in range(R):
    for j in range(C):
        print(matrix[i][j], end = " ")
    print()
​
#5
# Program to add two matrices using nested loop
​
X = [[1,2,3],
    [4 ,5,6],
    [7 ,8,9]]
​
Y = [[9,8,7],
     [6,5,4],
     [3,2,1]]
​
​
result = [[0,0,0],
         [0,0,0],
         [0,0,0]]
​
# iterate through rows
for i in range(len(X)):
# iterate through columns
    for j in range(len(X[0])):
        result[i][j] = X[i][j] + Y[i][j]
​
for r in result:
    print(r)
​
[10, 10, 10]
[10, 10, 10]
[10, 10, 10]
# Python Tasks – Day14
​
1.Program to find the sum of digits of a number until the number is reduced to 1 digit
2. Program to find LCM and HCF of two numbers
3.Write a program to accept any number n and print the cube of all numbers from 1 to n which are divisible by 3. Rewrite the program using a continue statement.
4.Write a program to read roll number and marks of 10 students in 3 subjects. The valid range for roll number is 1000-9999,
if the roll number entered is not in this range, the user should be asked to enter again. Calculate total marks of only those students who get more than or equal to 40 marks in each subject. Count the number of students whose total is more than 200. Print the roll number of the students who gets the highest total.
5.Write a program to input a number and count the digits in it. Use while loop and the program should work correctly for 0 also.
6.Write a program to enter a number and find the reverse of that number. Also display the double of the reverse number. (don’t use string magic)
#1
a=int(input("enter number to get sum of digits"))
n=a
s=0
while(n>0):
    r=n%10
    s=s+r
    n=n//10
print("The sum of digit is:",s)
enter number to get sum of digits3336
The sum of digit is: 15
!=
#2
print("enter two number to find hcf and lcm")
n1=int(input())
n2=int(input())
a=n1
b=n2
t=b
while(t!=0):
    t=b
    b=a%b
    a=t
​
hcf=a  #hcf*lcm=a*b
lcm=(a*b)/hcf
​
print("highest common factor of",n1,"and",n2,"is:",hcf)
print("least common multiple of",n1,"and",n2,"is:",lcm)
enter two number to find hcf and lcm
6
12
---------------------------------------------------------------------------
ZeroDivisionError                         Traceback (most recent call last)
Cell In[21], line 10
      8 while(t!=0):
      9     t=b
---> 10     b=a%b
     11     a=t
     13 hcf=a  #hcf*lcm=a*b

ZeroDivisionError: integer division or modulo by zero

#3
#Write a program to accept any number n and print the cube of all numbers from 1 to n which are divisible by 3. 
#Rewrite the program using a continue statement.
​
n=int(input("enter number"))
​
for i in range(1,n+1):
    a=i*i*i
    if(a%3==0):
        print(a,",",end='')
        
        
​
enter number23
27 ,216 ,729 ,1728 ,3375 ,5832 ,9261 ,
#4
​
# Defining a class student, which contain name, Roll number and marks of the student.
class Student(object):
    def __init__(self, name, roll, marks):
        self.name = name
        self.roll = roll
        self.marks = marks
    
    def getmarks(self):
        return self.marks
    
    def getroll(self):
        return self.roll
    
    def __str__(self):
        return self.name + ' : ' + str(self.getroll()) +'  ::'+  str(self.getmarks())
  
# Defining a function for building a Record 
# which generates list of all the students    
def Markss(rec, name, roll, marks):
    rec.append(Student(name, roll, marks))
    return rec
# Main Code
Record = []
x = 'y'
while x == 'y':
    name = input('Enter the name of the student: ')
    height = input('Enter the roll number: ')
    roll = input('Marks: ')
    Record = Markss(Record, name, roll, height)
    x = input('another student? y/n: ')
# Printing the list of student
n = 1
for el in Record:
    print(n,'. ', el)
    n = n + 1
Enter the name of the student: petho
Enter the roll number: 100
Marks: 23
another student? y/n: n
1 .  
---------------------------------------------------------------------------
TypeError                                 Traceback (most recent call last)
Cell In[23], line 36
     34 n = 1
     35 for el in Record:
---> 36     print(n,'. ', el)
     37     n = n + 1

Cell In[23], line 17, in Student.__str__(self)
     16 def __str__(self):
---> 17     return self.name + ' : ' + str(self.getroll()) +'  ::'+  str(self.getmarks())

TypeError: 'str' object is not callable

#5
n=int(input("enter number"))
c=0
while(n>0):
    n=n//10
    c=c+1
print("total no.of digits:",c)
enter number12345
total no.of digits: 5
#6
n=int(input("enter number"))
s=0
while(n>0):
    r=n%10
    s=s*10+r
    n=n//10
    
print("The reverse of the number is:",s)
​
print("Double of reverse number is:",s*s)
enter number21
The reverse of the number is: 12
Double of reverse number is: 144
