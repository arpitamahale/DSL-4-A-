# DSL-4-A-
# Practical No: 4(A)
#  Problem Statement: Write a python program to store roll numbers of student in array who attended training program in random order. Write function for searching whether particular student attended training program or not, using Linear search and Sentinel search. Please make note that while realizing the set duplicate entries are to avoided.
# Program:-
def inp(A):
 global n
 global x
 n=int(input("enter total no of student"))
 print("enter roll numbers")
 for i in range(n):
  x=int(input())
  A.append(x)
 print(A)
def lsearch(A,n):
 e=0
 x=int(input("enter roll no to search"))
 for i in range (n):
  if(a[i]==x):
   print("number found at index",i)
   e=1
 if(e==0):
  print("student not found")  
def ssearch(A,n):
 x=int(input("enter roll no to search"))
 last=A[n-1]
 i=0
 A[n-1]=x 
 while(a[i] !=x):
  i=i+1
 A[n-1]=last
 if(i<n-1) or (x==A[n-1]):
  print("number found at index",i)
 else:
  print("number not found")
while True:
 print("--------------------------------")
 print("1:enter and display array")
 print("2:linear search")
 print("3:sentinal search")
 print("4:exit")
 q=int(input("enter your choice"))
 print("--------------------------------")
 if(q==1):
  a=[]
  inp(a)
 if(q==2):
  lsearch(a,n)
 if(q==3):
  ssearch(a,n)
 if(q==4):
  break

# output:
# Output:
# 1:enter and display array
# 2:linear search
# 3:sentinal search
# 4:exit
# enter your choice1
# --------------------------------
# enter total no of student 5
# enter roll numbers
# 1
# 2
# 3
# 4
# 5
# [1, 2, 3, 4, 5]
# --------------------------------
# 1:enter and display array
# 2:linear search
# 3:sentinal search
# 4:exit
# enter your choice 2
# --------------------------------
# enter roll no to search 4
# number found at index 3
# --------------------------------
# 1:enter and display array
# 2:linear search
# 3:sentinal search
# 4:exit
# enter your choice 3 
# --------------------------------
# enter roll no to search 2 
# number found at index 1
# --------------------------------

