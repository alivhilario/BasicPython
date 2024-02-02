# BasicPython

<div> <h2>Printing </h2> </div>

```python
#Do✅
    #input
    print('''the
    big
    black
    box''')
    print("I'm Alex")
    print('She said "Lacomme"'

#output
    the
    big
    black
    box
    I'm Alex
    She said "La comme"

#Don't❌❌
    print('the
    big
    black
    box')

#Do✅
    print("the\nbig\nblack\nbox1")
    print('the big\nblack box2')
    print("the")
    print("big \n\n black")
    print("box3")

    #output
    the
    big
    black
    box1
    the big
    black box2
    the
    big 
    
     black
    box3

#Do✅
    #input
    print("""There once was a fellow
    Who came from the meadow
    And desired to settle
    In caves of yellow""")

    #output
    There once was a fellow
    Who came from the meadow
    And desired to settle
    In caves of yellow
    
  ```
<div> <h2>Variables and Concatenation </h2> </div>

```python
#Do✅
    #input
    value_1 = 'bear'
    value_2 = 'cheetah'
    print(value_1, value_2)
    print(value_1 + value_2)

    #output
    bear cheetah
    bearcheetah

#Use of Braces
#input
    name = 'Alex'
    lastName = 'Jones'
    print('My name is {} and my last name is {}'.format(name, lastName))

 #output
    My name is Alex and my last name is Jones.

#input
    name = 'Alex'
    lastName = 'Jones'
    print(f'My name is {name} {lastName}')

 #output
    My name is Alex and my last name is Jones.
  ```
<div> <h2>The Input Function </h2> </div>

```python
#Do✅
    #input
    letter = input('Type a letter to use for the Christmas tree: ')
    print('  ' + letter)
    print(' ' + letter + letter + letter)
    print(letter + letter + letter + letter + letter)
    print('  |  ')

    #output
      *
     ***
    *****
      |  
    
  ```
<div> <h2>Integers </h2> </div>

```python
#Don't❌❌

    #input
    name = 'Pierre'
    email = 'pierre@gmail.com'
    age = 50
    height = 72

    print('His name is ' + name)
    print(name + ' can be contacted at ' + email)
    print('He is ' + age + ' years old and is ' + height + ' inches tall')

#output
   His name is Pierre
    Pierre can be contacted at pierre@gmail.com
    Traceback (most recent call last):
      File "test.py", line 7, in <module>
        print('He is ' + age + ' years old and is ' + height + ' inches tall')
    TypeError: must be str, not int


#Do✅
    #input
    print('His name is ' + name)
    print(name + ' can be contacted at ' + email)
    print('He is ' +str(age) + ' years old and is ' + str(height) + ' inches          tall')

    #output
    His name is Pierre
    Pierre can be contacted at pierre@gmail.com
    He is 50 years old and is 72 inches tall
    
  ```
<div> <h2>String Multiplication </h2> </div>

```python

#Don't❌❌
    #input
    revenue = input('Business revenue: ')
    cost = input('Business costs: ')
    profit = revenue - cost
    print('The business profit is: ' + str(profit))

#output
     Business revenue: 100
    Business costs: 75
    Traceback (most recent call last):
      File "/Users/bddicken/mu_code/test.py", line 3, in <module>
        profit = revenue - cost
    TypeError: unsupported operand type(s) for -: 'str' and 'str'

#Do✅
    #Input
    revenue = int(input('Business revenue: '))
    cost = int(input('Business costs: '))
    profit = revenue - cost
    print('The business profit is: ' + str(profit))

    #output
    Business revenue: 100
    Business costs: 75
    The business profit is: 25

#Do✅
    #input
    revenue = int(input('Business revenue: '))
    cost = int(input('Business costs: '))
    profit = revenue - cost
    print('The business profit is: ' + str(profit))
    cost_bar = '#' * int((cost / revenue) * 25)
    profit_bar = '#' * int((profit / revenue) * 25)
    print('  cost: ' + cost_bar)
    print('profit: ' + profit_bar)

    #output
     cost: #########
    profit: ###############
    
  ```
<div> <h2>String Indexing</h2> </div>

```python
#Do✅
    #input
    city = ´Jerusalem'
    letter = city[4]
    print(letter

    #output
     s 

#Do✅
    #input
    city = ´Jerusalem'
    rock = city[0] + city[1] + city[8]
    print(rock)

    #output
     Jem 


#Do✅
    #input
    city = ´Jerusalem'
    rock = city[-9] + city[-8] + city[-1]
    print(rock)

    #output
     Jem

#Do✅ Len()
    #input
    text = input('Type something')
    last = text[len(text) -1]
    other = text[len(text) -2]
    print('The last two characters of if your input were: ' + other + last)

    #output
     Belgium
     um
 ```
<div> <h2>Math</h2> </div>

```python
#Do✅
    #Input
    x = 100 + 100
    y = 100 / 2
    print( type(x) )
    print( type(x) )

    #output
    <class 'int'>
    <class 'float'>

#Do✅
    #input INT() 
    revenue = int(input('Business revenue: '))
    cost = int(input('Business costs: '))
    profit = revenue - cost
    print('The business profit is: ' + str(profit))
    costBar = '#' * int((cost / revenue) * 25)
    profitBar = '#' * int((profit / revenue ) * 25)
    print('  cost: ' + costBar)
    print('profit: ' + profitBar)

    #output
    Business revenue: 450
    Business costs: 150
    The business profit is: 300
      cost: ########
    profit: ################

#Don't❌❌ Support string multiplication with FLOATS!!!!
    #input
    x = 'z'
    y = x * 1.5
    print(y)

#output
TypeError: can't multiply sequence by non-int of type 'float'
  
  ```
<div> <h2>Booleans and Boolean Expressions</h2> </div>

```python
#Do✅
    #Input
    homeCost = int(input('How much does your house cost?'))
    availableFunds = int(input('How much money do you have inmediately available?'))
    downPayment = homeCost * 0.2
    if availableFunds >= downPayment:
        print('You can afford the down payment!')

    #output
    How much does your house cost?5000
    How much money do you have inmediately available?2500 
    You can afford the down payment!
  
  ```
<div> <h2>Flag Creator</h2> </div>

```python
#Do✅
    #Input
    # Ask the user for input values and convert to integers
    width = input("Flag width:\n")
    width = int(width)
    height = input("Flag height:\n")
    height = int(height)
    
    # Calculate half of the width and height fur use in multiplication
    half_width = int(width / 2)
    half_height = int(height / 2)
    
    # Create and print the rows of the flag
    upper_row = '#' * half_width + '-' * half_width + '\n'
    lower_row = '-' * width + '\n'
    print(upper_row * half_height, end='')
    print(lower_row * half_height, end='')

    #output
    Flag width:
    5
    Flag height:
    4
    ##--
    ##--
    -----
    -----
  
  ```
<div> <h2>Making Decisions with if statements</h2> </div>

```python
#Do✅
   #Input
# Ask the user for lenght of its name
name = input('What is your first name?')
if len(name) < 35 and name[0].isupper():
    print('That is a valid name')
else:
    print('Sorry, your name is either')
    print('  *Too long')
    print('  *Not capitalized')

    #Input
experience = input("What level of Spanish experience do you have? ")

if experience == "none":
    print("You should take Spanish 101")
elif experience == "101":
    print("You should take Spanish 102")
elif experience == "102":
    print("You should take Spanish 201")
elif experience == "201":
    print("You should take Spanish 202")
elif experience == "202":
    print("You should move on to more advanced classes!")
else:
    print("Sorry, I didn't recognize what you entered.")
    print("Please give me one of these experience levels: none, 101, 102, 201, or 202.")
  ```
<div> <h2>Nesting if-statements</h2> </div>

```python
#Do✅
   #Input
hungry = input('are you hungry? ')
if hungry == 'yes':
  sounds_good = input('What sound good to get? ')
  if sounds_good == 'pizza':
    print('go to Pizza Hut and get some pizza!!')
  elif sounds_good == 'burger':
    print('go to In-Out Burger and get a burger!!')
  elif sounds_good == 'tacos':
    print('go to home and make some tacos')
  else:
    print('unsure')

thirsty = input('are you thirsty? ')
if thirsty == 'yes':
  sounds_good = input('What sound good to drink?')
  if sounds_good == 'soda':
    print('go to Coca-Cola and get some soda!!')
  elif sounds_good == 'water':
    print('go to home and get some water!!')
  else:
     print('unsure')

#input:✅
x = int(input('enter a number: '))
y = int(input('enter a number: '))
if x > y:
  if y*2 == x:
    if y < x-20:
      if y == 100:
        print('I reacehed thsi line')
      else:
        print('Else A')
    else:
      print('Else B')
  else: 
    print('Else C')
else:
  print('Else D')
  ```
<div> <h2>Combining if-Stateents and Loops</h2> </div>

```python
#Do✅
   #Input
hungry = input('are you hungry? ')
if hungry == 'yes':
  sounds_good = input('What sound good to get? ')
  if sounds_good == 'pizza':
    print('go to Pizza Hut and get some pizza!!')
  elif sounds_good == 'burger':
    print('go to In-Out Burger and get a burger!!')
  elif sounds_good == 'tacos':
    print('go to home and make some tacos')
  else:
    print('unsure')

thirsty = input('are you thirsty? ')
if thirsty == 'yes':
  sounds_good = input('What sound good to drink?')
  if sounds_good == 'soda':
    print('go to Coca-Cola and get some soda!!')
  elif sounds_good == 'water':
    print('go to home and get some water!!')
  else:
     print('unsure')

#input:✅
x = int(input('enter a number: '))
y = int(input('enter a number: '))
if x > y:
  if y*2 == x:
    if y < x-20:
      if y == 100:
        print('I reacehed thsi line')
      else:
        print('Else A')
    else:
      print('Else B')
  else: 
    print('Else C')
else:
  print('Else D')
#input✅
n = int(input('type').strip())
if (n % 2 == 0 and n >= 2 and n <= 5) or (n % 2 == 0 and n > 20): 
  print('Not Weird')
elif n >= 6 and n <= 20:
  print('Weird')
else:
  print('Weird')
  ```
<div> <h2>String recargado</h2> </div>

```python
#Do✅
    #Input
    text = 'She knows how to program Py'
    print('Js' in text)
    print('Py ' in text)

if 'Py' in text:
    print('correct decision')
else:
    print('good one too')

    #Output
    False
    False
    correct decision

    #input
    size = len(text)
    print(size)
    print(text.upper())
    print(text.lower())
    print(text.count('o'))
    
    print(text.swapcase())
    print(text.startswith('She'))
    print(text.endswith('Py'))
    print(text.replace('Py', 'Go'))
    
    text_2 = 'this is a title'
    print(text_2)
    print(text_2.capitalize())
    print(text_2.title())
    print(text_2.isdigit())
    print('398'.isdigit())

    #output
    False
    False
    correct decision
    27
    SHE KNOWS HOW TO PROGRAM PY
    she knows how to program py
    4
    sHE KNOWS HOW TO PROGRAM pY
    True
    True
    She knows how to program Go
    this is a title
    This is a title
    This Is A Title
    False
    True
  ```
<div> <h2>String recargado</h2> </div>

```python
#Do✅
    #Input
    text = 'She knows how to program Py'
    print('Js' in text)
    print('Py ' in text)

if 'Py' in text:
    print('correct decision')
else:
    print('good one too')

    #Output
    False
    False
    correct decision
  ```
<div><h3>Piedra papel o tijera</h3></div>

```python
    #Input
    user_option = input('piedra, papel o tijera => ')
    user_option =user_option.lower()
    computer_option = 'piedra'
    if user_option == computer_option:
      print('empate')
    elif user_option == 'piedra':
      if computer_option == 'tijera':
        print('piedra gana a tijera')
        print('user gano')
      else:
        print('papel gana a piedra')
        print('computer gano')
  ```
<div><h3>Indexing & slicing</h3></div>

```python
    #Input
    text = 'She knows how to program Python'
    print(text[0])
    print(text[1])
    # print(text[999])
    size = len(text)
    print('size => ',size)
    print(text[size - 1])
    print(text[-1])
    
    # slicing
    print(text[0:5])
    print(text[10:16])
    print(text[:10])
    print(text[5:-1])
    print(text[5:])
    print(text[:])
    print(text[10:16:1])
    print(text[10:16:2])
    print(text[::2])

    #Output
    S
    h
    size =>  31
    n
    n
    She k
    how to
    She knows 
    nows how to program Pytho
    nows how to program Python
    She knows how to program Python
    how to
    hwt
    Sekoshwt rga yhn

  ```

