CS335A: Compiler Design (Assignment 3: PARSER)
===================================================================

* Source Language: *Python3*
* Target Language: *x86 Assembly*
* Implementation Language: *Python*
* Authors: Deepak Kumar, Kamesh Kanwariya, Palash Chauhan and Rahul Kumar Wadbude

* Tool Used : PLY (Python Lex and Yacc)

### Running Instruction
_______________________

1. Run the following command to run test1.py
```
make test=test/test1.py all
```

### Directory Structure
______________________________________________________
* bin:
	* lexer.py [Python source file to specify language lexemes]
	* parser.py [Python source file to specify grammar]
	* yacc.py [Python source file from PLY for parsing ]
	* generate.py [Python file to generate rightmost derivation in html ]
* src:
	* lexer.py [Python source file to specify language lexemes]
	* parser.py [Python source file to specify grammar]
	* yacc.py [Python source file from PLY for parsing ]
	* generate.py [Python file to generate rightmost derivation in html ]
* test:
	* 'test1'.py [Test files]
	* 'test2'.py [Test files]
	* 'test3'.py [Test files]
	* 'test4'.py [Test files]
	* 'test5'.py [Test files]
* makefile
* README.pdf

A Tutorial on the language features offered by the compiler 
----------------------------------------------------------------
----------------------------------------------------------------

The compiler supports the basic structures of the Programming languages such as assignment , operators , loops ans function calls.

*Note : Indentation is through tabs or spaces

Assignment 
____________________________
```
a=10
a=10.2
a=b
a=[1,2,3,4,a,b]
```
Print Statement 
____________________________
```
print a
print 4
print 4.6
print 'hello world'
print "hello world"
print '''hello world'''

```

Operators with Parenthesis
_______________________________________

```
c = a + b - c * c / d % k
c=(a+b)**(c+d)
a+=b
a-=c
a*=c
a/=c
a%=c
```
Relational & Logical Operators
_________________________________________
```
a = 4 > 3
a= 4 > 3 and 5==5
a= a > b or c <= 9 and not True 
if True and True:
  do something
```
If Statement
___________________________
```
a=9
if a==9:
  print 'yes'
a=10
if a == 10:
  print 1
else :
  print 2
```

While Statement
_____________________________

```
while a > 0:
  print 'hi'
```

Nested Looping
________________________

```

while a > 0:
  while b >= 0:
    while c>=0:
      for i in [1,2,3]:
        print 'hi'
```

Function Without Parameters
______________________________________

```
def myfun():
  a=10
myfun()
```

Function With Parameters
_________________________________

```

def myfun(c, d, e, f):
  print c,d,e,f
a = myfun(1000, 100, 10, 1)
print a

```

Function call from another function
__________________________________________
```
def f():
	return 1
def f1():
  f()	
```
Recursion
_______________________________
```
f():
  print 'hi'
  if i>1:
    f()
```
Break & Continue Statement
__________________________

```
for i in [1,2,3]
  a=1
  if i==3:
    break
  else:
    continue
```
