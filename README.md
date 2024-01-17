# BasicPython

<div> <h2>Printing </h2> </div>

```python
#Do✅
    #input
    print('''the
    big
    black
    box''')

#output
    the
    big
    black
    box

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

