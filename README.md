# PYTHON_BASIC_PART-2
BASIC COD OF PYTHON PART-2 THERE IS THE conditional statement  loops,if,else,elif then function 
#condition statement
# if statement
'''a=21
if a>=18:
    print("you can vote")'''

# if-else statement
'''a =15
if a>=18:
    print("you can vote")
else:
    print("you can't vote") '''

# if-elif-else statement ex-1
'''a = 65
if a>=80:
    print("you got A grade")
elif a>=60:
    print("you got B grade")
elif a>=50:
    print("you got C grade")
elif a>=40:
    print("you got D grade")
else:
    print("you got F grade")'''

#if-eliff-else statemnt ex-2
'''color = input("enter your color:")
if  color == "red":
    print("stop")
elif color =="yellow":
    print("get ready")
elif color =="green":
    print("go")
else:
    print("invalid color")'''

#if-eliff-else statemnt ex-3
'''age =int(input("enter yor age:"))
if (age < 13):
    print("you are childern")
elif (age >= 13 and age<20):
    print ("you are youngster")
elif (age >= 20 and age<60):
    print("you are adult")
else:
    print("you are senior citizen")
'''
# check login credentials
'''username = input("enter your username:")
Password = input("enter your password:")
if(username == "admin" and Password=="pass"):
    print("LOGIN SUCCESSFUL")
elif(username !="admin"):
    print("wrong username")
else:
    print("wrong password")'''

# num is even or odd
'''n = int(input("enter a number:"))
if(2%n == 0):
    print("num is even")
else:
    print("num is odd")'''

#nesting
'''username =input("enter your username:")
Password = input("enter your password:")

if(username == "admin"and Password=="pass"):
    print("LOGIN SUCCESSFUL")
else:
    if(username !="admin"):
        print("wrong username")
    else:
        print("wrong password")
'''
#match case statement ex-1
'''color = input("enter your color:")
match color:
    case"red":
        print("stop")
    case"yellow":
        print("get ready")
    case"green":
        print("go")
    case _:
        print("invalid color")  '''
#match case statement ex-2
'''day = str(input("enter a day:"))
match day:
    case "monday":
        print("first day of the week")
    case "tuesday":
        print("second day of the week")
    case "wednesday":
        print("third day of the week")
    case "thursday":
        print("fourth day of the week")
    case "friday":
        print("fifth day of the week")
    case "saturday":
        print("sixth day of the week")
    case "sunday":
        print("seventh day of the week")
    case _:
        print("invalid day")    
'''
#LOOPS IN PYTHON
#{ when we want to execute a block of code multiple times we use loops}
#(when we want do many time print any thing on that time we use the loops )
# types of loops in python ther is two types that is while,and for loops
#1. for loop
#2. while loop(it is a key word it says to still codition is true then keep excuting the block of code)
# ex-1 of infinite loop
'''count =1 # iterator means loop ko run i also we can use on the count word
while(count <=5):
    print("hellow word",count)
    count+=1
    print("after loop ,count =", count)
'''
# finit loop =>5x
'''i = 10 # iterator
while(i >= 1):
    print(i)
    i -=1'''
#print multiplication table of any num 'n'
'''n = int(input("enter your num:"))
i=1
while (i <=10):
    print(n * i)
    i+=1'''

# In loop break and continue
# break(when in condtion said stop then stop the excution)
'''i =1
while(i<=10):
    if (i % 6 ==0):
        break
    print(i)
    i+=1    
     #this is updation of the loop
print ("outside loop now....") 
'''
# continue there skip the iteration next iteration run 
'''i =1
while (i <= 10):
    if(i % 3 == 0):
        i+=1
        continue
    print(i)
    i +=1
print("outside loop now ....")     
        '''
# print the odd num from 1 to 10
'''i=1
while (i < 10):
    i+=1
    if(i % 2 == 0):
        continue
    print(i)
  
print("outside loop now ...")'''


#for loops (whatever work we can do with while loop that we can do with the for loop 
# and also whatever work we can do workwith the for loop that we can do while loop)
# most for the time for loop use for the sequeatial travee means any sequence we want to traivel that time we use  
#like -list, tuple,dictionary ,string is the charcter ex hello h1 e2like

'''string ="hello"
for var in string:# in mean check the present ther that latter or not
 print(var)'''
# check the o is exists in word are not
'''string="hello"#o
if 'o' in string:
    print("o is exists in string")'''
#range

'''for i in range(5):
    print(i+1)'''

'''for i in range(5):
    print("hello word")'''

# in word how many time i 
'''word= "artificial intelligence"
ans= 0
for ch in word:
    if (ch =='i'):
        ans +=1
print("ans of i = ", ans)'''  

#loop q- print vowel count of a given string

'''word ="artificial "

count =0

for ch in word:
    if (ch =='a' or ch == 'e'or ch == 'i'or ch == 'o'or ch == 'u'):
     count += 1

print("ans =",count)'''


# range in loop 
#range()-( there is the three parameter that is 1st is the starting value 
# 2nd is the stoping value 
# 3rd is the step value step value means how updation or increment in the loops)  

'''for i in range(5):
   print(i)'''# 0,1,2,3,4
'''for i in range(1,6):
   print(i)'''#1 2,3,4,5

#odd num print
'''for i in range(1,10,2):
   print(i) '''

# even num print
'''for i in range(2,10,2):
   print(i)'''

# loop q print sum of the first 'n' natural num
'''n= int(input("enter num:"))
sum = 0
for i in range(1,n+1):
    sum += i
print("sum=",sum)'''

#function in python
#the function of blocks  for statement that perform spacific task doing  
#ther are two (part 1- definition )(2- call the function)
#function re resuable of component
# def functionname  (): 
#then multiple statment wr write 

def hello(): # this is the function defination
    print("hello")
hello() # this is the function call  
*************************************************************************
# function is like black blocks 
# function definition
def sum(a,b): # parameters
    s = a+b
    return s
ans = sum (7,8)# function call
print(ans)'''
 #3 num taking input and return the avrage 

def cal_avg(a,b,c):
    sum = a+b+c
    return sum/3
print(cal_avg(6,7,9))'''
# defulta value in the function
def sum(a,b=1):
    return a+b
print(sum(6))
******************************************************************************
# function type 
"""#(there are the built in function and user define function) 
# built _in function is the print(),input(),type(),range() -start value stop and step )
#userdefine function there is the difine by user like sum,avreage, caluate logic we  write) """

# lamda function ther are the small enominy function that we define with lambda 
#lambda key word write
sum=lambda a,b: a+b
print (sum(8,9))'''
# using lambda average 
avg=lambda a,b: (a+b)/2
print (avg(8,9))
#main work of lambda that is high order of function

# (WAF)which is write a function to print factorial of'n'
def cal_factorial(n):
    fact = 1
    for i in range(1,n+1):
        fact *= i

    return fact  
n = int(input("enter n:"))  
print(cal_factorial(n))



 






