## Introduction to Programming Using Python

---

## Introduction to Python

- Python is a good general-purpose language that can be used in a variety of applications.
- Python is a very humanreadable, programming language.
- Python is a very good choice for beginners.

---
## Basic Data Types

<table>
	<tr>
		<td>Data Type </td>
		<td>Examples </td>
	</tr>
	<tr>
		<td>Integer (int)</td>
		<td>0, 100</td>
	</tr>
	<tr>
		<td>String (str)</td>
		<td>"Hello" , "World"</td>
	</tr>
	<tr>
		<td>Boolean (bool)</td>
		<td>True, False, Result of logical condition</td>
	</tr>
</table>

---
## Python variables

```python

variableName = value 
```

Examples


```python

N = 100 # Type ? 

answer = "yes" # Type ?

found = True # Type ?
```
---

## Python Conditions

```python
if condition1 :
	do something when condition1 is true
elif condition2 :
	do something when condition2 is true
else:
	do something when all conditions are false
```
+++

## Python Condition Example

```python
if signal=="red" :
	print ("Stop")
elif signal=="green" :
	print ("Go")
```

---

## Python while loop

```python
while condition:
	repeat something
```

The loop will end either if condition becomes false or if there is a ***`break`*** statement.

+++

## While loop example

```python
x = 1
while x <= 5:
	print ("|")
	x = x + 1
```

```python
x = 1
while True:
	print ("|")
	if x >= 5:
		break
	x = x + 1
```
---

## Input and Output

```python

print ("Message you want to say to users")

variable=input("Read something from users")
```

+++

## Input and Output Example

```python

name = input("What is your name? ")
print ("Your name is " + name)

age = int(input("What is your age? "))
print ("Your age is " + str(age))


```

---
### Program for Guessing number game.

<iframe height="500px" width="100%" src="https://repl.it/@erajasekar/GuessNumberGame?lite=true" scrolling="no" frameborder="no" allowtransparency="true" allowfullscreen="true" sandbox="allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-modals"></iframe>

+++

### Guessing number game visualization

<iframe width="800" height="580" frameborder="0" src="https://pythontutor.com/iframe-embed.html#code=answer%3D%22%22%0Alow%3D0%0Ahigh%3D101%0Acount%3D0%0A%0Aprint%28%22Think%20a%20Number%20from%201%20to%20100.%20I%20will%20try%20to%20guess%20it.%22%29%0A%0Awhile%20answer!%3D%22y%22%3A%0A%20%20%20%20guess%3D%28low%20%2B%20high%29//2%0A%20%20%20%20count%3Dcount%20%2B%201%0A%20%20%20%20print%28%22%5CnType%3A%20y%29%20for%20Yes.%20l%29%20if%20it%20is%20to%20Large.%20s%29%20if%20it%20is%20to%20Small.%5Cn%22%29%0A%20%20%20%20answer%3Dinput%28%22Is%20it%20%22%20%2B%20str%28guess%29%20%2B%20%22%20%5By/l/s%5D%20%3F%20%3A%20%22%29%0A%20%20%20%20if%20answer%3D%3D%22l%22%3A%0A%20%20%20%20%20%20high%3Dguess%0A%20%20%20%20elif%20answer%3D%3D%22s%22%3A%0A%20%20%20%20%20%20low%3Dguess%0A%20%20%20%20elif%20answer%3D%3D%22y%22%3A%0A%20%20%20%20%20%20break%0A%0Aprint%28%22Great!%20the%20number%20that%20you%20thought%20is%3A%20%22,%20guess%29%0Aprint%28%22Guessed%20in%20%22%20%2B%20str%28count%29%20%2B%20%22%20tries%20%22%29%0A&codeDivHeight=400&codeDivWidth=350&cumulative=false&curInstr=0&heapPrimitives=false&origin=opt-frontend.js&py=3&rawInputLstJSON=%5B%5D&textReferences=true"> </iframe>

---

## Python for loop

```python
for item in list_of_times:
	do something with item
```
Examples

```python
numbers=[1,2,3,4,5]
for n in numbers:
	print (n)
```

---


## Program for sequential search

<iframe height="500px" width="100%" src="https://repl.it/@erajasekar/PrimesSequentialSearch?lite=true" scrolling="no" frameborder="no" allowtransparency="true" allowfullscreen="true" sandbox="allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-modals"></iframe>

+++

### Sequential search visualization

<iframe width="2000" height="550" frameborder="0" src="https://pythontutor.com/iframe-embed.html#code=primes%20%3D%20%5B2,%203,%205,%207,%2011,%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%2013,%2017,%2019,%2023,%2029,%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%2031,%2037,%2041,%2043,%2047,%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%2053,%2059,%2061,%2067,%2071,%20%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%2073,%2079,%2083,%2089,%2097%5D%0AN%20%3D%20int%28input%28'Enter%20the%20number%20to%20check%20for%20prime%3A%20'%29%29%3B%0Afound%20%3D%20False%3B%0Afor%20i%20in%20primes%3A%0A%20%20if%20i%20%3D%3D%20N%3A%0A%20%20%20%20found%20%3D%20True%3B%0A%20%20%20%20break%3B%0A%20%20%20%20%0Aif%20found%3A%0A%20%20print%20%28str%28N%29%20%2B%20%22%20is%20a%20Prime%22%29%3B%0Aelse%3A%0A%20%20print%20%28str%28N%29%20%2B%20%22%20is%20Not%20a%20Prime%22%29%3B%0A&codeDivHeight=400&codeDivWidth=350&cumulative=false&curInstr=29&heapPrimitives=false&origin=opt-frontend.js&py=3&rawInputLstJSON=%5B%2223%22%5D&textReferences=true"> </iframe>

---

## Python Program for Binary Search

<iframe height="500px" width="100%" src="https://repl.it/@erajasekar/PrimesBinarySearch?lite=true" scrolling="no" frameborder="no" allowtransparency="true" allowfullscreen="true" sandbox="allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-modals"></iframe>

+++

### Binary Search visualization

<iframe width="2000" height="550" frameborder="0" src="https://pythontutor.com/iframe-embed.html#code=primes%20%3D%20%5B2,%203,%205,%207,%2011,%0A%20%20%20%20%20%20%20%2013,%2017,%2019,%2023,%2029,%0A%20%20%20%20%20%20%20%2031,%2037,%2041,%2043,%2047,%0A%20%20%20%20%20%20%20%2053,%2059,%2061,%2067,%2071,%20%0A%20%20%20%20%20%20%20%2073,%2079,%2083,%2089,%2097%5D%0A%0AN%20%3D%20int%28input%28'Enter%20the%20number%20to%20check%20for%20prime%3A%20'%29%29%3B%0A%0Astart%20%3D%200%0Aend%20%3D%20len%28primes%29-1%0Afound%20%3D%20False%0A%0A%0Awhile%20start%3C%3Dend%20and%20not%20found%3A%0A%20%20i%20%3D%20%28start%20%2B%20end%29//2%0A%20%20if%20primes%5Bi%5D%20%3D%3D%20N%3A%0A%20%20%20%20found%20%3D%20True%0A%20%20else%3A%0A%20%20%20%20if%20N%20%3C%20primes%5Bi%5D%3A%0A%20%20%20%20%20%20end%20%3D%20i-1%0A%20%20%20%20else%3A%0A%20%20%20%20%20%20start%20%3D%20i%2B1%0A%0Aif%20found%3A%0A%20%20print%20%28str%28N%29%20%2B%20%22%20is%20a%20Prime%22%29%3B%0Aelse%3A%0A%20%20print%20%28str%28N%29%20%2B%20%22%20is%20Not%20a%20Prime%22%29%3B&codeDivHeight=400&codeDivWidth=350&cumulative=false&curInstr=0&heapPrimitives=false&origin=opt-frontend.js&py=3&rawInputLstJSON=%5B%5D&textReferences=true"> </iframe>

---

### Exercise Inverse Guessing Number Game

<iframe height="450px" width="100%" src="https://repl.it/@erajasekar/GuessingNumberGame2?lite=true" scrolling="no" frameborder="no" allowtransparency="true" allowfullscreen="true" sandbox="allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-modals"></iframe>

---

## Searching for Max value

Let's say we have list of numbers:

```python

numbers = [10,50,20,30,100,60]


```

You need to find the Maximum value in the list which is 100 in this example.

+++

### Solving using Best score analogy

* Let's say you are playing a game many times.
* You will get a score at end of each game.
* You will to calculate the best score you have got so far.
* You can use same approach to search for Max.

+++

### Searching for Max solution

<iframe height="500px" width="100%" src="https://repl.it/@erajasekar/SearchMax?lite=true" scrolling="no" frameborder="no" allowtransparency="true" allowfullscreen="true" sandbox="allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-modals"></iframe>

+++

### Searching for Max visualization


<iframe width="2000" height="550"  frameborder="0" src="https://pythontutor.com/iframe-embed.html#code=numbers%20%3D%20%5B10,50,20,30,100,60%5D%0A%0AmaxValue%20%3D%200%0A%0Afor%20n%20in%20numbers%3A%0A%20%20%20%20if%20n%20%3E%20maxValue%3A%0A%20%20%20%20%20%20%20%20maxValue%20%3D%20n%0A%0Aprint%28%22Max%20is%20%3A%20%22%20%2B%20str%28maxValue%29%29%0Aprint%28%22Max%20using%20function%20%3A%20%22%20%2B%20str%28max%28numbers%29%29%29%0A&codeDivHeight=400&codeDivWidth=350&cumulative=false&curInstr=20&heapPrimitives=false&origin=opt-frontend.js&py=3&rawInputLstJSON=%5B%5D&textReferences=false"> </iframe>

---

### Resources

* [Python-Kids-Playful-Introduction-Programming](http://www.amazon.com/Python-Kids-Playful-Introduction-Programming/dp/1593274076)
* [Hello World!: Computer Programming for Kids and Other Beginners](http://amzn.com/1617290920)


