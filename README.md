# Getting-Started-with-Python

These are my notes for [**_Programming for Everybody (Getting Started With Python) on Coursera_**](https://www.coursera.org/learn/python)

## Notes

### **_Week 1_**

#### **1.1 Why Program**  
not been recorded

#### **1.2 Hardware Overview**

1. When you write a program, you create a file on the secondary memory, like a Python file, and then at some point that is loaded into the main memory, translated, and then your program is here. And then when the CPU says what next, your program feeds its first instruction. And then when that's done, the CPU says what's next? It feeds the second instruction, third instruction, fourth instruction. It's called the **fetch-execute cycle**.

2. Definitions  

   (1) **Central Processing Unit (CPU)**: Runs the program - The CPU is always wondering "what to do next". Not the brains exactly - very dumb but very very fast.  
   (2) **Input Devices**: Keyboard, Mouse, Touch Screen  
   (3) **Output Devices**: Screen, Speakers, Printer, DVD Burner  
   (4) **Main Memory**: **Fast small temporary storage** - lost on reboot - aka RAM  
   (5) **Secondary Memory**: **Slower large permanent storage** - lasts untill deleted - disk drive/memory stick  

#### **1.3 Python as a Language**

1. Syntax Error: Python is lost.

---

### **_Week 2_**

#### **Demonstration: Using the Python Playground**

1.  
   ```python
   print('Play!')
   print('Hello World.')
   ```

2. Installing Python and writing a program:
  
   **Step 1:** Install **Python3** and **Visual Studio Code**  
   **Step 2:**
   Open **Visual Studio Code**.  
   Create and save a new file on your **desktop**.  
   Also, create a folder on your desktop named **_py4e_**.  
   I save the file as **_HelloWorld.py_**.  

   **Step 3:** Write the code in Visual Studio Code:
   ```python
   print('hello from a file')
   ```
   **Step 4:** Open Terminal (for Mac) and write code:
   ```
   cd ~/Desktop/py4e
   python HelloWorld.py
   ```

---

### **_Week 3_**

#### **1.4 Writing paragraphs of code**

1. Elements of Python  

   (1) Vocabulary/Words: Variables and Reserved words  
   (2) Sentence structure: valid syntax patterns  
   (3) Story structure: constructing a program for a purpose  

2. Reserved words  
You cannot use **reserved words** as variable names/identifiers.
   ```py
   False class return is finally
   None if for lambda continue
   True def from while nonlocal
   and del global not with
   as elif try or yield
   assert else import pass
   break except in raise
   ```

3. Sentences or Lines

   ```
   Assignment statement
   x = 2
   ```
   ```
   Assignment with expression
   x = x + 2
   ```

   ```
   Print function
   print(x)
   ```

   ```
   Variable Operator Constant Function
   ```

4. Python scripts

   (1) interactive Python is good for experiments and programs of 3-4 lines long.  
   (2) Most programs are much longer, so we type them into a file anf tell Python to run the commands in the file.  
   (3) In a sense, we are "giving Python a script".  
   (4) As a convention, we add **".py"** as the suffix on the end of these files to indicate they contain Python.  

5. Interactive versus Script

   (1) Interactive: you type directly to Python one line at a time and it responds.  
   (2) Script: you enter a sequence of statements (lines) into a file using a text editor and tell Python to execute the statements in the file.  

6. Program steps or Program flow

   (1) Like a recipe or installation instrcutions, a program is a **sequence** of steps to be done in order.  
   (2) Some steps are **conditional**: they may be skipped.  
   (3) Sometimes a step or group of steps is to be **repeated**.  
   (4) Sometimes we store a set of steps to be used over and over as needed several places throughout the program.  

7. Sequential Steps

   ```python
   x = 2
   print(x)
   x = x + 2
   print(x)
   ```

8. Conditional Steps

   ```python
   x = 5
   if x < 10:
       print('Smaller)
   if x > 20:
       print('Bigger') 
   print('Finish')
   ```

9. Repeated Steps
   ```python
   n = 5
   while n > 0:
       print(n)
       n = n - 1
   print('Blastoff!')
   ```
   Loops (repeated steps) have **iteration variables** that change each time through a loop.

10. Summary  

    ```python
    name = input('Enter file:')
    handle = open(name)
    
    counts = dict()
    for line in handle:
        words = line.split()
        for word in words:
            counts[word] = counts.get(word,0) + 1
    bigcount = None
    bigword = None
    for word,count in counts.item():
        if bigcount is None or count > bigcount:
            bigword = word
            bigcount = count
    
    print(bigword, bigcount)
    ```

---
### **_Quiz: Chapter 1_** 

1. When Python is running in the interactive mode and displaying the chevron prompt(>>>) - what question is Python asking you?  

   a. What Python statement would you like me to run?  
   b. What is the next machine language instruction to me?  
   c. What is your favourite color?  
   d. What Python script would you like me to run?  
    
   Answer: a.

2. What will the following program print out:  

   ```python
   x = 15
   x = x + 5
   print (x)
   ```
    a. 20  
    b. 5  
    c. 15  
    d. "print x"  
    e. x + 5  

    Answer: a.  

3. Python scripts (files) have names that end with:  

    a. .doc  
    b. .py  
    c. .exe  
    d. .png  

    Answer: b.  

4. Which of these words are reserved words in Python?  
    
    a. make  
    b. break  
    c. todo  
    d. if  
    e. concat  

    Answer: b. d.  

5. What is the proper way to say "good-bye" to Python?  
    
    a. #EXIT  
    b. while  
    c. // stop  
    d. quit()  

    Answer: d.  

6. Which of the parts of a computer actually excutes the program instructions?  

    a. Central Processing Units  
    b. Secondary Memory  
    c. Input/Output Devices  
    d. Main Memory  

    Answer: a.  

7. What is "code" in the context of this course?  

    a. A set of rules that govern the style of programs  
    b. A way to encrypt data during World War II  
    c. A sequence of instructions in a programming language  
    d. A password we use to unlock Python features  

    Answer: c.  

8. A USB memory stick is an example of whihc of the following components of computer architechture?  

   a. Central Processing Unit  
   b. Main Memory  
   c. Output Device  
   d. Secondary Memoty  

   Answer: d.  

9. What is the best way to think about a "Syntax Error" while programming?  

   a. The computer did not understand the statement you entered  
   b. The computer needs to have its software upgraded  
   c. The computer has used GPS to find your location and hates everyone from your town  
   d. The computer is overheating and just wnats you to stop to let it cool down  

   Answer: a.  

10. Which of the following is **not** one of the programming patterns coveres in Chapter 1?  

    a. Sequential Steps  
    b. Random Steps  
    c. Conditional Steps  
    d. Repeated Steps  

    Answer: b.  

---
### **_Week 4_**

#### **2.1 Expressions - Part 1**

1. Constant
   
   **Fixed values** such as numbers, letters, and strings, are called **"constants"** because thier value does not change  

   (1) Numeric **constants** are as you expect  
   (2) String **constants** use single quotes(') or double quotes(")  
   
   ```python
   print(123)
   123
   print(98.6)
   98.6
   print('Hello world')
   Hello world
   ```

2. Variables  
   
   A **variable** is a named place in the memory where a programmer can store data and later retrieve the data using the **variable** "name"

   Programmers get to choose the names of the **variables**

   You can change the contents of a **variable** in a later statement

   ```
   x = 12.2
   y = 14
   x = 100
   ```

3. Python Variable Name Rules

   Must start with a letter or underscore ('_')

   Must consist of letters, numbers, and underscores

   Case Sensitive

   ```
   Good: spam eggs spam23 _speed

   Bad: 23spam #sign var.12

   Different: spam Spam SPAM
   ```

4. Sentences or Lines

   ```
   Assignment statement
   x = 2
   ```
   ```
   Assignment with expression
   x = x + 2
   ```

   ```
   Print function
   print(x)
   ```

   ```
   Variable Operator Constant Function
   ```

5. Assignemnt Statements

   We assign a value to a variable using the assignemnt statement (=)

   An assignment statement consists of an **expression on the right-hand side** and a **variable** to store the result

   ```
   x = 3.9 * x * ( 1 - x )
   ```

   A variable is a memory location used to store a value (0.6). The value stored in a variable can be updated by replacing the old value (0.6) with a new value (0.936)

   The right side is an expression. Once the expression is evaluated, the result is placed in (assigned to) the variable on the left side (i.e. x).

#### **2.2 Expressions - Part 2**

1. Numeric Expressions

   | Operator  | Operation         |
   | --------- |:-----------------:|
   | +         |      Addition     | 
   | -         |    Subtraction    |
   | *         |   Multiplication  |
   | /         |      Division     |
   | **        |        Power      |
   | %         |      Remainder    |


2. Order of Evaluation

   When we string operators together - Python must know which one to do first

   This is called **"operator precedence"**

   Which operator "take precedence" over the others?

   ```
   x = 1 + 2 * 3 - 4 / 5 ** 6
   ```

3. Operator Precedence Rules

   **_Highest precedence rule to lowest precedence rule_**

   - Parentheses are always respected
   - Exponentiation (raise to a power)
   - Multiplication, Division, and Remainder
   - Addition and Subtraction
   - Left to right

   ```python
   x = 1 + 2 ** 3 / 4 * 5
   print (x)
   
   x = 1 + 2^3 / 4 * 5
   x = 1 + 8 / 4 * 5
   x = 1 + 2 * 5
   x = 1 + 10
   x = 11
   ```

   Remeber the rules top to down (Parentheses; Power; Multiplication; Addition; Left to right)

   When writing code - use parenthses

   When writing code - keep mathematical expressions simple enough that they are easy to understand

   Break long series of mathematical operations up to make them more clear


4. What does "Type" mean?

   In a Python variables, literals, and constants have a **"type"**

   Python knows the **difference** between an integer number and a string

   For example **"+"** means "addition" if something is a number and "concentrate" if something is a string

   Concentrate = put together

   ```python
   ddd = 1 + 4
   print(ddd)
   5

   eee = 'hello ' + 'there'
   print(eee)
   hello there

5. Type Matters

   Python knows what **"type"** everything is

   Some operations are prohibited

   **You cannot "add 1" to a string**

   We can ask Python what type something is by using the **type()** function

   ```python
   eee = 'hello ' + 'there'
   eee = eee + 1
   Traceback (most recent call last):
   File "<stdin>", line 1, in <module>
   TypeError: Can't covert 'int' object to str implicitly

   type(eee)
   <class'str'>

   type('hello')
   <class'str'>

   type(1)
   <class'int'>

6. Several types of numbers

   Numbers have two main types:

   - **Integers** are whole numbers: -14, -2, 0, 1, 100, 401233
   - **Floating point numbers** have decimal parts: -2.5, 0.0, 98.6, 14.0

   There are other number types - they are variations on float and integer

   ```python
   xx =1
   type(xx)
   <class 'int'>

   temp = 98.6
   type(temp)
   <class'float'>

   type(1)
   <class 'int'>

   type(1.0)
   <class'float'>
   ```

7. Type conversions
   
   When you put an integer and floating point in an expression, the integer is **implicitly** converted to a float

   You can control this with the built-in functions int() and float()

   ```python
   print(float(99) + 100)
   199.0

   i=42
   type(1)
   <class'int'>
   f = float(i)
   print(f)
   42.0
   type(f)
   <class'float'>
   ```

8. Integer Division

   Interger division produces a floating point result

   **Integer division was different in Python 2.x**

   ```python
   print(10 / 2)
   5.0

   print(9 / 2)
   4.5

   print(99 / 100)
   0.99

   print(10.0 / 2.0)
   5.0

   print(99.0 / 100.0)
   0.99
   ```

9. String conversions

   You can also use **int()** and **float()** to convert between strings and intergers

   You will get **error** if the string does not contain numeric characters

   ```python
   sval = '123'
   type(sval)
   <class 'str'>
   print (sval + 1)
   Traceback (most recent call last):
   File "<stdin>", line 1, in <module>
   TypeError: Can't convert 'int' object to str implicitly
   ival = int(sval)
   type(ival)
   <class 'int'>
   print(ival + 1)
   124
   nsv = 'hello bob'
   niv = int(nsv)
   Traceback (most recent call last):
   File "<stdin>", line 1, in <module>
   ValueError: invalid literal for int() with bas 10: 'x'
   ```

10. User input

    We can instruct Python to pause and read data from the user using the **input()** function

    The **input()** function returns a string

    ```python
    nam = input('Who are you?')
    print('welcome', nam)

    Who are you
    Chunk (Press Enter)
    Welcome Chunk
    ```

#### **2.3 Expressions - Part 3**

1. Comments in Python

   Anything after a **#** is ignored by Python

   Why Comment?
   - Describe what is going to happen in a sequence of code
   - Document who wrote the code or other ancillary information
   - Turn off a line of code - perhaps temporarily

   example:
   ```python
   # Get the name of the file and open it
   name = input('Enter file:')
   handle = open(name, 'r')

   # Count word frequently
   counts = dict()
   for line in handle:
       words = line.split()
       for word in words:
           counts[word] = counts.get(word,0) + 1

   # Find the most common word
   bigcount = None
   bigword = None
   for word,count in counts.items():
       if bigcount is None or count > bigcount:
           bigword = word
           bigcount = count

   # All done
   print(bigword, bigcount)
   ```

2. Converting user input

   If we wnat to read a number from the user, we must convert it from a string to a number using a type conversion function   

   Later we will deal with bad input data

   ```python
   # Convert elevator floors
   inp = input('Europe floor?)
   usf = inp(inp) + 1
   print('us floor', usf)

   Europe floor? ---> 0 (string) (press enter)
   US floor ---> 1 (press enter)
   ```

### **_Quiz: Chapter 2_**

1. In the following code,
   ```python
   print(98.6)
   ```
   What is "98.6"?  

   a. A conditional statement  
   b. A variable  
   c. An iteration/loop statement  
   d. A constant  

   Answer: d.

2. What does the following code print out?
   ```python
   print("123" + "abc")
   ```
   a. This a syntax error becasue you cannot add strings  
   b. 123+abc  
   c. 123abc  
   d. hello world

   Answer: c.

3. Which of the following is a bad Python variable name?  

   a. Spam  
   b. spam23  
   c. spam.23  
   d. spam_23  
   
   Answer: c.

4. Which of the following is not a Python reserved word?  

   a. spam  
   b. break  
   c. continue  
   d. for

   Answer: a.

5. Assume the variable x has been intialized to an integer value (e.g., x = 3). What does the following statement do?  

    ```python
    x = x + 2
    ```
   a. Retrieve the current value for x, add two to it and put the sum back into x  
   b. This would fail as it is a syntax error  
   c. Exit the program  
   d. Create a function called "x" and put the value 2 in the function

   Answer: a.

6. Which of the following elements of a mathematical expression in Python is evaluated first?  
   a. Addition +  
   b. Substraction -  
   c. Parentheses ()  
   d. Multiplication *  

   Answer: c.

7. What is the value of the remainder operator?
   ```python
   42 % 10
   ```
   Hint - the "%" is the remainder operator  
   a. 10  
   b. 420  
   c. 1042  
   d. 2  

   Answer: d.

8. What will be the value of x after the following statement executes:  
   ```python
   x = 1 + 2 * 3 - 8 / 4
   ```
   a. 15  
   b. 4  
   c. 3.0  
   d. 5.0  

   Answer: d.

9. What will be the value of x when the following statement is executed?  
   ```python
   x = int(98.6)
   ```
   a. 98  
   b. 6  
   c. 100  
   d. 99  

   Answer: a.

10. What does the Python **input()** function do?  
    a. Pause the program and read data from the user  
    b. Connect to the networl and retrieve a web page  
    c. Read the memory of the running program  
    d. Take a screen shor from an area of the screen  

    Answer: a.
   
#### **_Assignment 2.2_**
   Write a program that uses **input** to prompt users for their names and then welcome them. Note that **input** will pop up a dialog box. Enter **Sarah** in the pop-up box when you are prompted so your output will match the desired output.

   ```python
   name = input("Enter your name")
   print("Hello " + name)
   ```

#### **_Assignemnt 2.3_**
   Write a program to prompt the user for hours and rate per hour using input to compute gross pay. Use 35 hours and a rate of 2.75 per hour to test the program (the pay should be 96.25). You should use **input** to read a string and **float()** to convert the string to a number. Do not worry about error checking or bad user data.
   ```python
   hrs = input("Enter Hours:")
   rate = input("Enter Rate per Hour:")
   pay = float(hrs)*float(rate)

   print("Pay:", pay)
   ```
---
### **_Week 5_**

#### **3.1 Conditional Statement**
##### **Part 1**

1. Conditional Steps
   ```python
   x = 5
   if x < 10:
      print('Smaller')
   if x > 20:
      print('Bigger')
   print('Finish')
   ```
 
2. Comparison Operators
   - **Boolean experssions** ask a question and produce a Yes or No result which we use to control program flow  
   - **Boolean expressions** using **comparison operators** evaluate to True/False or Yes/No  
   - Comparison operators look at variables but do not change the variables

   |  Python   |      Meaning      |
   | --------- |:-----------------:|
   | <         |      Less than    |
   | <=        |Less than or Equal to|
   | ==        |     Equal to      |
   | >=        |Greter than or Equal to|
   | >         |    Greater than   |
   | !=        |      Not equal    |

   ```python
   x = 5
   if x ==5:
      print('Equal 5')
   if x > 4:
      print('Greater than or Equals 5')
   if x < 6:
      print('Less thaan 6')
   if x <= 5:
      print('Less than or Equals 5')
   if x != 6:
      print('Not equal 6')
   ```

3. One-way decisions
   ```python
   x = 5 
   print('Before 5')
   if x == 5:
      print('is 5)
      print('is still 5
      print('Third 5')
   print('Afterwards 5')
   print('Brfore 5')
   if x == 6:
      print('Is 6')
      print('Is still 6')
      print('Third 6')
   print('Afterwords 6')
   ```

4. 
   increase/maintain after **if** or **for**  
   decrease to indicate **end of block**

   ```python
   x = 5
   if x > 2:
      print('Bigger than 2')
      print('Still bigger')
   print('Done with 2')

   for i in range(5)
      print(i)
      if i > 2:
         print('Bigger than 2')
         print('Done with i', i)
   print('All Done')
   
5. Nested decisions
   ```python
   x = 42
   if x > 1:
      print("More than one')
      if x < 100:
         print('Less than 100')
   print('All done')

6. Two-way decisions
   - Sometimes we want to do one thing if a logical expression is true and something else if the expression is false  

   - It is like a fork in the road - we mush choose **one or the other** path but not both

   - With else:
   ```python
   x = 4
   if x > 2:
      print('Bigger')
   else:
      print('Smaller')
   print('All done')
   ```

#### **3.2 Conditional Statement**
##### **Part 2**

1. Visualize Blocks
   ```python
   x = 4
   if x > 2:
      print:('Bigger')
   else:
      print('Smaller')
   print('All done')
   ```

2. Multi-way
   ```python
   if x < 2:
      print('Small')
   elif x < 10:
      print('Medium')
   else:
      print('LARGE')
   print('All done')
   ```

3. The try/except structure
   - You surround a dangerous section of code with **try** and **except**  
   - If the code in the **try** works - the **except** is skipped  
   - If the code in the **try** fails - it jumps to the **except** section 5 

   (There will not be Traceback)

   ```python
   astr = 'Hello Bob'
   try:
      istr = int(astr)
   except:
      istr = -1
   print('First', istr)
   ```
   When the first conversion fails - it just drops into the exept: clause and the program continues...  

   ```
   we get First -1
   ```

   ```python
   astr = '123'
   try:
      istr = int(astr)
   except:
      istr = -1
   print('Second', istr)
   ```
   When the second conversion succeeds - it just skips the except: clasuse and the program continues...

   ```
   we get Second 123
   ```

4. Try/Except
   ```python
   astr = 'Bob'
   try:
      print('Hello')
      istr = int(astr)
      print('There')
   except:
      istr = -1
   print('Done', istr)
   ```
   ```
   we get: 
   Hello  
   Done, -1
   ```

   ```python
   rawstr = input('Enter a number:')
   try:
      ival = int(rawstr)
   except:
      ival = -1
   
   if ival > 0:
      print('Nice work')
   else:
      print('Not a number')
   ```

### **_Quiz: Chapter 3_**

1. What do we do to a Python statement that is immediately after an **if** statement to indicate that the statement is to be excuted only when the **if** statement is **true**?  

   a. Start the statement with a "#" character  
   b. Indent the line below the if statement  
   c. Begin the statement with a curly brace {  
   d. Underline all of the conditional code  

   Answer: b.  

2. Which of these operators is **not** a comparison/logical operator?  
   a. ==  
   b. !=  
   c. >=  
   d. =  
   e. <=  

   Answer: d.  

3. What is true about the following code segment:  
   ```python
   if x == 5:
      print('Is 5')
      print('Is Still 5')
      print('Third 5')
   ```
   a. Depending on the value of **x**, either all three of the print statement will execute or none of the statement will execute  
   b. The string 'is 5' will always print out regardless of the value for **x**  
   c. The string 'is 5' will never print out regardless of the value for **x**  
   d.  Only two of the three print statements will print out if the value of **x** is less than zaro  

   Answer: a.  

4. When you have multiple lines in an **if** block, how do you indicate the end of the **if** blcok?  
   a. You omit the semicolon; on the last line of the if block  
   b. You de-indent the next line past the if block to the same level of indent as the origincal **if** statement  
   c. You use a curly brace { after the last line of the if block  
   d. You put the colon : character on a line by itself to indicate we are done with the if block  
   
   Answer: b.  

5. You look at the following text:  
   ```python
   if x == 6:
      print('Is 6')
      print('Is Still 6')
      print('Third 6')
   ```
   It looks perfect but Python is giving you an 'Indentation Error' on the second print statemnt. What is the most likely reason?  

   a. Python has reached its limit on the largest Python program that can be run  
   b. You have mixed tabs and spaces in the file  
   c. Python thinks 'Still' is a mis-spelled word in the string  
   d. In order to make humans feel inadequate, Python randomly emits 'Indentation Error' on perfectly good code - after about an hour the error will just go away without any changes to your proagram  

   Answer: b.

6. What is the Python reserved word that we use in two-way if tests to indicate the block of code that is to be executed if the logical test is false?  
   a. iterate  
   b. otherwise  
   c. toggle  
   d. else  

   Answer: d.  

7. What will the following code print out?
   ```python
   x = 0
   if x < 2:
      print('Small')
   elif x < 10:
      print('Medium')
   else:
      print('LARGE')
   print('All done')
   ```  
   a. 
   ```
   Small  
   Medium  
   LARGE  
   All done 
   ```
   b. 
   ```
   LARGE  
   All done  
   ```
   c. 
   ```
   All done  
   ```
   d. 
   ```
   Small  
   All done  
   ```

   Answer: d.  

8. For the following code:   
   ```python
   if x < 2:
      print('Below 2')
   elif x >= 2:
      print('Two or more')
   else:
      print('Something else')
   ```  
   What value of 'x' will cause 'Something else' print out?  

   a. x = 2.0  
   b. x = -22  
   c. This code will never print 'Something else' regardless of the value for 'x'  
   d. x = -2.0  

   Answer: c.  

9. In the following code(numbers added) - which will be the last line to excute successfully?  
   ```python
   (1) astr = 'Hello Bob'
   (2) istr = int(astr)
   (3) print('First', istr)
   (4) astr = '123'
   (5) istr = int(astr)
   (6) print('Second', istr)
   ```  
   a. 1  
   b. 5  
   c. 2  
   d. 6  

   Answer: a.  

10. For the following code:  
    ```python
    astr = 'Hello Bob'
    istr = 0
    try:
       istr = int(astr)
    except:
       istr = -1
    ```  
    What will the value be for **istr after this code executes**?  
 
    a. It will be a random number depending on the operating system the program runs on  
    b. -1  
    c. It will be the 'Not a number ' value(i.e. NaN)  
    d. false  

    Answer: b.  

#### **_Assignment 3.1_**

1. Write a program to prompt the user for hours and rate per hour using input to compute gross pay. Pay the hourly rate for the hours up to 40 and 1.5 times the hourly rate for all hours worked above 40 hours. Use 45 hours and a rate of 10.50 per hour to test the program (the pay should be 498.75). You should use **input** to read a string and **float()** to convert the string to a number. Do not worry about error checking the user input - assume the user types numbers properly.

   ```python
   hrs = input('Enter Hours:')
   rate = input('Enter the Rate:')
   h = float(hrs)
   r = float(rate)
   if h <= 40:
      print(h * r)
   elif h > 40:
      print(40 * r + (h - 40) * 1.5 * r)
   ```
#### **_Assignment 3.2_**
1. Write a program to prompt the user for hours and rate per hour using input to compute gross pay. Pay the hourly rate for the hours up to 40 and 1.5 times the hourly rate for all hours worked above 40 hours. Use 45 hours and a rate of 10.50 per hour to test the program (the pay should be 498.75). You should use **input** to read a string and **float()** to convert the string to a number. Do not worry about error checking the user input - assume the user types numbers properly.

   ```python
   hrs = input('Enter Hours:')
   rate = input('Enter the Rate:')
   h = float(hrs)
   r = float(rate)
   if h <= 40:
      pay = h * r)
   elif h > 40:
      pay = 40 * r + (h - 40) * 1.5 * r)
   print('Pay', pay)
   ```

#### **_Assignment 3.3_**
1. 3.3 Write a program to prompt for a score between 0.0 and 1.0. If the score is out of range, print an error. If the score is between 0.0 and 1.0, print a grade using the following table:
Score Grade
>= 0.9 A
>= 0.8 B
>= 0.7 C
>= 0.6 D
< 0.6 F
If the user enters a value out of range, print a suitable error message and exit. For the test, enter a score of 0.85.
   
   ```python
   score = input('Enter the score:')
   s = float(score)
   g = 'Grade'
   if s >= 0.9:
      g = 'A'
   elif s >= 0.8:
      g = 'B'
   elif s >=0.7:
      g = 'C'
   elif s >=0.6:
      g = 'D'
   elif s < 0.6:
      g = 'F'
   else:
      g = 'Error: Out of Range'
   print('Grade:', g)
   ```

---

### **_Week 6_**

#### **_4.1 Using functions_**

1. Stored (and reused) Steps
   ```python
   def thing():
      print('Hello')
      print('Fun')

   thing() 
   print('Zip')
   thing()  
   ```
   ```
   Output:  
   Hello  
   Fun  
   Zip  
   Hello  
   Fun
   ```

2. Max function
   A **function** is **some stored code** that we use. A function takes some **input** and produces an **output**.
   ```python
   big = max('Hello world')
   print(big)
   w
   tiny = min('Hello world')
   print(tiny)
   ```

   ```python
   'Hello world' (a string)  
   ->
   def max(inp):
      blah
      blah
      for x in inp:
         blah
         blah
   ->  
   'w' (a string)
   ```

#### **_4.2 Buliding functions_**

1. Building our own functions  
   - We create a new function using the **def** keyword followed by optional parameters in parentheses
   - We indent the body of the function  
   - This **defines** the function but **does not** execute the body of the function

   ```python
   x = 5
   print('Hello')

   def print_lyrics():
      print("I'm a lumberjack, and I'm a okay.")
      print("I sleep all night and I work all day.")
   
   print('Yo')
   print_lyrics()
   x = x + 2
   print(x)
   ```

   ```
   Output:
   Hello  
   Yo  
   I'm a lumberjack, and I'm okay.  
   I sleep all night and I worl all day.  
   7
   ```

2. Arguments  
   - An **argument** is a value we pass into the **function** as its **input** when we call the function
   - We use **arguments** so we can direct the **function** to do different kinds of work when we call it at **different** times
   - We put the **arguments** in parentheses after the **name** of the function

   ```python
   big = max('Hello world')
   'Hello world' is the argument
   ```

3. Parameters  
   A **parameter** is a variable which we use **in** the function **definition**. It is a "handle" that allows the code in the function to access the **arguments** for a particular function invocation.

   ```python
   def greet(lang):
      if lang == 'es':
         print('Hola')
      elif lang == 'fr':
         print('Bonjour')
      else:
         print('Hello')
   
   greet('en')
   -> Hello
   greet('es')
   -> Hola
   greet('fr')
   -> Bonjour
   ```

4. Return values
   Often a function will take its arguments, do some computation, and **return** a value to be used as the value of the function call in the **calling expression**. The **return** keyword is used for this.

   ```python
   def greet():
      return "Hello"
   
   (return: 
   1. 'it stops the function'
   2. 'it also determines the residual value')

   print(greet(), "Glenn")
   print(greet(), "Sally")
   ```

   ```
   Output:
   Hello Glenn
   Hello Sally
   ```

   - A "fruit" **function** is one that produces a **result**(or **return value**) 
   - The **return** statement ends the **function** execution and "send back" the **result** of the **function**

   ```python
   def greet(lang):
      if lang == 'es':
         return 'Hola'
      elif lang == 'fr':
         return 'Bonjour'
      else:
         return 'Hello'
   
   print(greet('en'), 'Glenn')
   -> Hello Glenn
   print(greet('es'), 'Sally')
   -> Hola Sally
   print(greet('fr'), 'Michael')
   -> Bonjour Michael
   ```

5. Multiple Parameters/Arguments
   - We can define more than one **parameter** in the **function definition**
   - We simply add more **arguments** when we call the **function**
   - We match the number and order of arguments and parameters

   ```python
   def addtwo(a, b):
      added = a + b
      return added
   
   x = addtwo(3, 5)
   print(x)
   
   -> 8
   ```

### **_Quiz: Chapter 4_**

1. Which Python keyword indicates the start of a function definition?  
   a. sweet  
   b. continue  
   c. def  
   d. return  

   Answer: c.

2. In Python, how do you indicate the end of the block of code that makes up the function?  
   a. You add a line that has at least 10 dashes  
   b. You add the matching curly brace that was used to start the function {  
   c. You de-indent a line of code to the same indent level as the **def** keyword  
   d. You put the colon character (:) in the first colunmn of a line  

   Answer: c.  

3. In Python, what is the **input()** feature best described as?  
   a. A user-defined function  
   b. A built-in funciton  
   c. A reserved word  
   d. A data strcutre that can hold multiple values using string as keys  

   Answer: b.  

4. What does the following code print out?  
   ```python
   def thing():
      print('Hello')

   print('There')
   ```
   a. 
   ```
   thing 
   ``` 
   b.  
   ```
   def  
   thing  
   ```
   c. 
   ```
   There  
   ```
   d.  
   ```
   thing  
   Hello  
   There 
   ```
   Answer: c.  

5. In the following Python code, which of the following is an "argument" to a function?

   ```python
   x = 'banana'
   y = max(x)
   z = y * 2
   ```
   a. x  
   b. max  
   c. 'banana'  
   d. y

   Answer: a.  

6. What will the following Python code print out?  
   ```python
   def func(x):
      print(x)

   func(10)
   func(20)
   ```
   a.
   ```
   def  
   x  
   func  
   func 
   ```
   b.
   ```
   x  
   x  
   ```
   c.
   ```
   10  
   20  
   ```
   d.
   ```
   x  
   20  
   ```

   Answer: c.  

7. Which line of the following Python program will never excute?  
   ```python
   def stuff():
      print('Hello')
      return
      print('World')
   
   stuff()
   ```
   a. print('World')  
   b. stuff()  
   c. print('Hello')  
   d. return  
   e. def stuff():

   Answer: a.

8. What will the following Python program print out?  
   ```python
   def greet(lang):
      if lang == 'es':
         return 'Hola'
      elif lang == 'fr':
         retun 'Bonjour'
      else:
         return 'Hello'
   
   print(greet('fr),'Michael')
   ```
   a. Bonjour Michael  
   b. def Michael  
   c. Hello Michael  
   d.  
   Hola  
   Bonjour  
   Hello  

   Answer: a.

9. What does the following Python code print out? (Note that this is a bit of a trick question and the code has what many would condsider to be a flaw/bug - so read carefully).
   ```python
   def addtwo(a, b):
      added = a + b
      return a
   x = addtwo(2,7)
   print(x)
   ```
   a. 14  
   b. 7  
   c. 2  
   d. addtwo

   Answer: c.

10. What is the most important benefit of writing your own functions?  
    a. Following the rule that whenever a program is more than 10 lines you must use a function  
    b. Avoiding writing the same non-trivial code more than once in your program  
    c. To avoid having more than 10 lines of sequential code without an indent or de-indent  
    d. Following the rule that no function can have more than 10 statements in it

    Answer: b.

#### **_Assignment 4.6_**

1. Write a program to prompt the user for hours and rate per hour using input to compute gross pay. Pay should be the normal rate for hours up to 40 and time-and-a-half for the hourly rate for all hours worked above 40 hours. Put the logic to do the computation of pay in a function called computepay() and use the function to do the computation. The function should return a value. Use 45 hours and a rate of 10.50 per hour to test the program (the pay should be 498.75). You should use **input** to read a string and **float()** to convert the string to a number. Do not worry about error checking the user input unless you want to - you can assume the user types numbers properly. Do not name your variable sum or use the sum() function.

   ```python
   hrs = input('Enter the Hour:')
   rate = input('Enter the Rate:')
   h = float(hrs)
   r = float(rate)

   def computepay(h, r):
      if h <= 40:
         pay = h * r
      if h > 40:
         pay = 40 * r + (h - 40) * 1.5 * r
      return pay
   p = computepay(h,r)
   print('Pay', p)
   ```

---

### **_Week 7_**

#### **_5.1 Loops and Iteration_**

1. Repeated steps  
   Loops (repeated steps) have **iteration variable** that change each time through a loop. Often these **iteration variables** go through a sequence of numbers
   ```python
   n = 5
   while n > 0:
      print(n)
      n = n - 1
   print('Blastoff')
   print(n)
   ```
   ```
   Output:  
   5
   4
   3
   2
   1
   Blastoff
   0
   ```

2. An infinite loop
   ```python
   n = 5
   while n > o:
      print('Lather')
      print('Rense')
      print('Dry off')
   ```

3. Breaking out of a loop
   - The **break** statement ends the current loop and jumps to the statment immediately following the loop  
   - It is like a llop test that can happen anywhere in the body of the loop

   ```python
   while True:
      line = input('> ')
      if line == 'done':
         break
      print(line)
   print('Done!)
   ```
   ```
   > hello there
   hello there
   > pig pig
   pig pig
   > done
   Done!
   ```

4. Finishing and iteration with continue
   The **continue** statement ends the current iteration and jumps to the top of the loop and starts the next iteration
   ```python
   while True:
      line = input('> ')
      if line[0] == '#':
         continue
      if line == 'done':
         break
      print(line)
   print('Done!')
   ```
   ```
   > hello there
   hello there
   > # don't print this
   > print this!
   print this
   > done
   Done!
   ```

#### **_5.2 Definite Loops_**

1. Definite loops (for loops) have explicit **iteration variables** that change each time throygh a loop. These **iteration variables** move through the sequence or set.

2. A simple definite loop
   ```python
   for i in [5, 4, 3. 2, 1]:
      print(i)
   print('Blastoff!')
   ```

3. A definite loop with strings
   ```python
   friends = ['Joseph', 'Glenn', 'Sally']
   for friend in friends:
      print('Happy New Year:', friend)
   print('Done!')
   ```
 
 4. Looking at in...
    - The **iteration variable** "iterates" through the **sequence** (ordered set)  
    - The **block (body)** of code is executed once for each value **in** the **sequence**  
    - The **iteration variable** moves through all of the values  **in** the **sequence**

    ```python
    for i in [5, 4, 3, 2, 1]
         print(i)
      i: iteration variable
      [5, 4, 3, 2, 1]: Five-element sequence
      ```

#### **_5.3 Finding the largest value_**

1. Making "smart" loops
   The trick is "knowing" something about the whole loop when you are stuck writing code that only sees one entry at a time

   ```
   Set some variables to initial values
   ```

   for **thing** in data:

   ```
   Look for something or do something to each entry separately, updating a variable
   ```

   ```
   look at the variables
   ```

2. Looping through a set
   ```python
   print('Before')
   for thing in [3, 41, 12, 3, 74, 15]:
      print(thing)
   print('After')
   ```
   ```
   Output:
   Before  
   9  
   41  
   12  
   3  
   74  
   15  
   After
   ```

3. What is the largest number?
   ```python
   largest_so_far = -1
   print('Before', largest_so_far)
   for the_num in [9, 41, 12, 3, 74, 15]:
      if the_num > largest_so_far:
         largest_so_far = the_num
      print(largest_so_far, the_num)
   print('After', largest_so_far)
   ```
   ```
   Output:
   Before -1  
   9 9  
   41 41  
   41 12  
   41 3  
   74 74  
   74 15  
   After 74
   ```
   We make a variable that contains the largest value we have seen so far. if the current **number we are looking at** is larger, it is the new **largest value we have seen so far**.

#### **_5.4 Loop Idioms_**

1. Counting in a loop

   ```python
   zork = 0
   print('Before', zork)
   for thing in [9, 41, 12, 3, 74, 15]:
      zork = zork + 1
      print(zork, thing)
   print('After', zork)
   ```
   ```
   Output:
   Before 0
   1 9
   2 41
   3 12
   4 3
   5 74
   6 15
   After 6
   ```
   To **count** how many times we execute a loop, we introduce a **counter variable that starts at 0** and we add ***one to it each time through the loop**.

2. Summing in a loop
   ```python
   zork = 0
   print('Before', zork)
   for thing in [9, 41, 12, 3, 74, 15]:
      zork = zork + thing
      print(zork, thing)
   print('After', zork)
   ```
   ```
   Output:
   Before 0
   9 9
   50 41
   62 12
   65 3
   139 74
   154 15
   After 154
   ```
   To **add up** a **value** we encounter in a loop, we introduce a **sum variable that starts at 0** and we add the **value** to the sum each time through the loop.

3. Finding the average in a loop
   ```python
   count = 0
   sum = 0
   print('Before', count, sum)
   for value in [9, 41, 12, 3, 74, 15]:
      count = count + 1
      sum = sum + value
      print(count, sum, value)
   print('After', count, sum, sum / count)
   ```
   ```
   Output:
   Before 0 0
   1 9 9
   2 50 41
   3 62 12
   4 65 3
   5 139 74
   6 154 15
   After 6 154 25
   ```
   An **average** just combines the **counting** and **sum** patterns and **divides when the loop is done**.

4. Filtering in a loop
   ```python
   print('Before')
   for value in [9, 41, 12, 3, 74, 15]:
      if value > 20:
         print 'Large number',value
   print('After')
   ```
   ```
   Output:
   Before
   Large number 41
   Large number 74
   After
   ```
   We use an **if** statement in the **loop** to catch/filter the values we are looking for.

5. Search using a boolean variable
   ```python
   found = False
   print('Before', found)
   for value in [9, 41, 12, 3, 74, 15]:
      if value == 3:
         found = True
      print(found, value)
   print('After', found)
   ```
   ```
   Output:
   Before False
   False 9
   False 41
   False 12
   True 3
   True 74
   True 15
   After True
   ```
   If we just want to search and **know if a value was found**, we use a **variable** that starts at **False** and is set to **True** as soon as we **find** what we are looking for.

6. How to find the smallest value
   ```python
   smallest = None
   print('Before')
   for value in [9, 41, 12, 3, 74, 15]:
      if smallest is None:
         smallest = value
      elif value < smallest:
         smallest = value
      print(smallest, value)
   print('After', smallest)
   ```
   ```
   Output:
   Before
   9 9
   9 41
   9 12
   9 3
   3 74
   3 15
   After 3
   ```
   We still have a variable that is the **smallest** so far. The first time through the loop **smallest** is **None**, so we take the first **value** to be the **smallest**.

7. The "is" and "is not" operators
   ```python
   smallest = None
   print('Before')
   for value in [3, 41, 12, 9, 74, 15]:
      if smallest is None:
         smallest = value
      elif value < smallest:
         smallest = value
      print smallest, value
   print('After', smallest)
   ```
   - Python has an **is** operator that can be used in logical expressions  
   - Implies "**is the same as**"  
   - Similar to, but stronger than **==**  
   - **is not** also is a logical operator

### **_Quiz: Chapter 5_**

1. What is wrong with Python loop:
   ```Python
   n = 5
   while n > 0:
      print(n)
   print('All done')
   ```

   a. This loop will run forever  
   b. The **print('All done')** statement should be indented four spaces  
   c. There should be no colon on the **while** statement  
   d. **while** is not a Python reserved word  

   Answer: a.

2. What does the **break** statement do?
   a. Exits the currently executing loop  
   b. Jumps to the 'top' of the loop and starts the next iteration  
   c. Exits the program  
   d. Resets the iteration variable to its initial value

   Answer: a.

3. What does the **continue** statement do?   
   a. Jumps to the "top" of the loop and starts the next iteration  
   b. Exits the program  
   c. Exits the currently executing loop  
   d. Resets the iteration variable to its initial value  

   Answer: a. 

4. What does the following Python program print out?  
   ```python
   tot = 0  
   for i in [5, 4, 3, 2, 1]:
      tot = tot + 1
   print(tot)
   ```
   a. 5  
   b. 15  
   c. 10  
   d. 0

   Answer: a.

5. What is the **_iteration_** variable in the following Python code?
   ```python
   friends = ['Joseph', 'Glenn', 'Sally']
   for friend in friends:
      print('Happy New Year:', friend)
   print('Done!')
   ```
   a. friend  
   b. Sally  
   c. Glenn  
   d. Joseph

   Answer: a. 

6. What is a good description of the following bit of Python code?
   ```python
   zork = 0
   for thing in [9, 41, 12, 3, 74, 15]:
      zork = zork + thing
   print('After', zork)
   ```
   a. Count all of the elements in a list  
   b. Sum all the elements of a list  
   c. Find the largest item in a list  
   d. Find the smallest item in a list

   Answer: b.

7. What will the following code print out?
   ```python
   smallest_so_far = -1
   for the_num in [9, 41, 12, 3, 74, 15]:
      if the_num < smallest_so_far:
         smallest_so_far = the_num
   print(smallest_so_far)
   ```
   Hint: This is a trick question and most would say this code has a bug - so read carefully  

   a. -1  
   b. 74  
   c. 42  
   d. 3

   Answer: a.

8. What is a good statement to describe the **is** operator as used in the following if statement:
   ```python
   if smallest is None:
      smallest = value
   ```
   a. matches both type and value  
   b. The if statement is a syntax error  
   c. Is true if the **smallest** variable has a value of -1  
   d. Looks up 'None' in the **smallest** variable if it is a string
   
   Answer: a.

9. Which reserved word indicates the start of an "indefinite" loop in Python?  
   a. for  
   b. def  
   c. indef  
   d. while  
   e. break  

   Answer: d.

10. How many times will the body of the following loop be executed?  
    ```python
    n = 0
    while n > 0:
       print('Lather')
       print('Rinse')
    print('Dry off!')
    ```
    a. 0  
    b. 1  
    c. 5  
    d. This is an infinite loop

    Answer: a.

#### **_Worked exercise 5.1_**

   ```python
   num = 0
   tot = 0.0
   while True:
      sval = input('Enter a number:')
      if sval == 'done':
         break
      try:
         fval = float(sval)
      except:
         print('Invalid input')
         continue
      # print(fval)
      num = num + 1
      tot = tot + fval

   # print('All Done!')
   print(tot, num, tot / num)
   ```

#### **_Assignemnt 5.2_**

1. Write a program that repeatedly prompts a user for integer numbers until the user enters 'done'. Once 'done' is entered, print out the largest and smallest of the numbers. If the user enters anything other than a valid number catch it with a try/except and put out an appropriate message and ignore the number. Enter 7, 2, bob, 10, and 4 and match the output below.
   ```python
   largest = None
   smallest = None

   while True:
      try:
         num = input('Enter a number')
         if num == 'done':
            break
         num = int(num)
         if largest is None or num > largest:
            largest = num
         if smallest is None or num < smallest:
            smallest = num
      except:
         print('Invalid input')
         continue
   print('Maximum is', largest)
   print('Minimum is', smallest)
   ```
---
## For GitHub
[语法](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
