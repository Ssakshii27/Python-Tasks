Section A: Multiple Choice Questions 
1. What will be the output of the following code?
print(type(5 / 2))
a) int
b) float
c) double
d) error
Ans: b) float

2. Which of the following is a valid variable name in Python?
a) 2variable
b) variable_name
c) variable-name
d) variable name
Ans: b) variable_name

3. How do you take user input in Python?
a) input()
b) scan()
c) cin >>
d) read()
Ans: a) input()

4. What will bool([]) return?
a) True
b) False
c) None
d) Error
Ans: b) False

5. What does len([1, 2, 3, 4]) return?
a) 3
b) 4
c) 5
d) Error
Ans: b) 4

Section B: Short Answer Questions
6. Write a Python program to swap two numbers without using a third variable.
Code: 
a=2
b=3
a=a^b
b=a^b
a=a^b
print(a)
print(b)

7. What is the difference between is and == in Python?
Ans: The is operator is used to compare the memory address of two variables whereas, == is used to compare values of two variable.

8. Write a Python function that returns whether a number is even or odd.
Code: 
def evenodd(n):
    if(n%2==0):
        print("Even Number")
    else:
        print("Odd Number")
evenodd(2)

9. Explain mutable and immutable objects in Python with an example.
Ans: Mutable objects can be changed after creation. Immutable objects cannot be changed once created.
For ex: Lists, dictionaries and sets are Mutable objects whereas, string, tuples and frozensets are the example of immutable objects.

10. Write a Python program to find the largest number in a given list.
Code: 
l=[1,2,3,4,5,54,86,234,8796]
print(max(l))

Section C: Coding Questions
11. Write a Python program to check if a string is a palindrome (same forward and backward).
Code:
def palindrome(s):
    rev=s[::-1]        
    if s==rev:
            print(f'{s} is Pallindrome')
    else:
            print(f'{s} is not Pallindrome')
palindrome('sas')

12. Write a Python program to generate the Fibonacci series up to n terms.
Code:
def fib(n):
    if n==0 or n==1:
        return 1
    return fib(n-1)+fib(n-2)
fib(6)

13. Write a function that takes a list and returns a new list with only the unique elements.
Code:
def unique(l):
    l=set(l)
    l=list(l)
    print(l)
unique([2,3,4,5,6,7,5,55,66,7,7,8,9,1,1,0])

14. Write a Python function to count the number of vowels in a given string.
Code:
def vowels(v):
    count=0
    for i in v:
        if(i in ['a','e','i','o','u','A','E','I','O','U']):
          count+=1
    print(count)
vowels('Hello World. Welcome to Python. MY name is Sakshi')

15. Write a Python program to find the factorial of a number using recursion
Code:
def factorial(n):
    if n==1 or n==0:
        return 1
    return n*factorial(n-1)
factorial(1)