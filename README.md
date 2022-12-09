
   # program to print the average of 10 numbers using loop
totsum = 0
for i in range(10):
    num = int(input("enter the value:"))
    totsum+=num
average = totsum/10
print("the average of the 10 numbers is :"(average))

# program to print the multiplication table of a given number
num = int(input("enter the number:"))
for i in range(1,11):
    print(num,"x",i,"=",num*i)

# program to count the number of digits in a given number
n = int(input("enter the number"))
count = 0
while(n>0):
    count = count + 1
    n = n//10
print("the no of digits in a number is ",(count))

# program to print the reverse of the number pattern
for i in range(5,0,-1):
    for j in range(i,0,-1):
        print(j,end="")
    print()

# Program to display the Fibonacci sequence up to n-th term

nterms = int(input("How many terms? "))

# first two terms
n1, n2 = 0, 1
count = 0

# check if the number of terms is valid
if nterms <= 0:
   print("Please enter a positive integer")
# if there is only one term, return n1
elif nterms == 1:
   print("Fibonacci sequence upto",nterms,":")
   print(n1)
# generate fibonacci sequence
else:
   print("Fibonacci sequence:")
   while count < nterms:
       print(n1)
       nth = n1 + n2
       # update values
       n1 = n2
       n2 = nth
       count =count+1
 
using recursion function the find the factorial of the given number
def factorial(n):
    return 1 if (n ==1 or n ==0) else n*factorial(n-1);
num = 5
print("the factorial of",num,factorial(num))
