ISD lab sheet week 5
For the practical part of this lab please save the Python programs that you create and take screenshots of the execution (evaluation) of your programs.
Consider this function:

def mystery(x, y) :
result = (x + y) / (y - x)
return result
What is the result of the call mystery(2, 3)? -> 5

What does this program print?
def main() :
a =5
b=7
print(mystery(a, b)) 
def mystery(x, y) :
z = x +y
z = z / 2.0 return z
main() -> 6

What does this program print?
def main() : 
a =4
print(mystery(a + 1))
def mystery(x) :
y = x *x
return y 
main() -> 25
￼￼
Consider this function that prints a page number on the left or right side of a page:
if page % 2 == 0:
print(page) 
else :
print("%60s%d" % (" ", page))
Introduce a function that returns a Boolean to make the condition in the if statement easier to understand.
page=int(input("Give me page num "))
p=page % 2 == 0
if p == 0:
print(p)
else :
print("\t\t\t\t\t\t\t\t\t\t\t\t\t\t\t\t\t\t\t\t\t\t\t\t", page)
Transform the following instructions into a function called count_ spaces. Define a main function that will ask the user to enter some input and call the count_spaces function to return ￼the number of spaces.
Counts the number of spaces spaces = 0 if char == " " :
def main():
userInput=input("Write something: ")
print(cont_space(userInput))
def cont_space(userInput):
spaces = 0
for char in userInput:
if char == " ":
spaces = spaces + 1
return spaces 
main()

Consider this recursive function:
def mystery(n) :
if n <= 0 :
return 0
else:
return n + mystery(n - 1)
What is mystery(4)? -->10

def mystery(n) :
if n <= 0 :
return 0
else:
return mystery(n // 2) + 1
What is mystery(20)? -->5 Consider these functions:
￼￼
def f(x) :
return g(x) + math.sqrt(h(x))
def g(x) :
return 4 * h(x)
def h(x) :
return x * x + k(x) - 1
def k(x) :
return 2 * (x + 1)
Without actually compiling and running a program, determine the results of the following function calls:

a. x1 = f(2) --> 39
b. x2 = g(h(2)) --> 400
c. x3 = k(g(2) + h(2)) --> 92
d. x4 = f(0) + f(1) + f(2) -->62
e. x5 = f(-1) + g(-1) + h(-1) + k(-1) --> 0

Consider the following function:
def f(a) :
if a < 0 :
return -1 n= a
while n > 0 :
if n % 2 == 0 :
n = n // 2 
elif n == 1 :
return 1 
else :
n= 3* n + 1 
return 0
Perform traces of the computations
f(-1) --> -1,
f(0) --> nothing,
f(1) --> 1, 
f(2) --> 1, 
f(10) --> 0,
f(100) --> 0.
