# BasicPython

<div> <h1>Printing </h1> </div>

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
<div> <h1>Variables and Concatenation </h1> </div>

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
<div> <h1>The Input Function </h1> </div>

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
<div> <h1>Integers </h1> </div>

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
    print('His name is ' + name)
    print(name + ' can be contacted at ' + email)
    print('He is ' +str(age) + ' years old and is ' + str(height) + ' inches          tall')
    
  ```
