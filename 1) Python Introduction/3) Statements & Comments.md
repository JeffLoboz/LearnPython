# Python Statement, Indentation, Comments


## Python Statement
- Instructions that a Python interpreter can execute are called statements. 
- a = 1 is an assignment statement.
- **if** statement
- **for** statement
- **while** statement

### Multi-Line statement
- The end of a statement is marked by a newline character.
- We can make a statement extend over multiple lines with the line continuation character. **\**

EX: Explicit Line Continuation

        a = 1 + 2 + 3 + \
            4 + 5 + 6 + \
            7 + 8 + 9

- Line continuation is implied inside paranthesis **( )**, brackets **[ ]**, and braces **{ }**.
- We can implement the above multi-line statement as:
EX:

        a = (1 + 2 + 3 + 
             4 + 5 + 6 + 
             7 + 8 + 9)

- The paranthesis **( )** do the line continuation implicitly
- Same with **[ ]** & **{ }**
EX:

        colors = ['red'
                  'blue',
                  'green']
          
- Can also put multiple statements in a single line using semicolons
EX:

        a = 1;  b = 2; c = 3


## Python Indentation
- Languages like C, C++, and Java use { } to define a block of code.
- Python uses indentation.
- Generally will use 4 whitespaces .
EX:

        for i in range(1, 11):
            print(i)
            if i == 5:
                break
        
- Identation can be ignored in line continuation, but better to indent.
EX: Indented

if True:
    print('Hello')
    a = 5
   
EX: Not indented

        if True: print('Hello'); a = 5

- Both are valid and do the same thing.


## Python Comments
- Comment with #
EX:

        #This is a comment
        #print out Hello
        print('Hello')


## Multi-line comments
EX: #

        #This is a long comment
        #and it extends
        #to multiple lines. 

EX: """ or '''

        """This is also an
        example of multi-lined comments"""

## Docstrings
- Docstring is short for documentation string.
- They're string literals that appear right after the defintion of a function, method, class, or module. 
- Triple quotes are used.
EX:

        def double(num):
            """Function to double the value"""
            return 2*num

- Docstrings are associated with the object as their **__doc__** attribute
- We can access the docstrings of the function with this code: print(double.__doc__)
