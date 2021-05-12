# Getting-Started-with-Python

These are my notes for [**_Programming for Everybody (Getting Started With Python) on Coursera_**](https://www.coursera.org/)

## Notes

### **_Week 1_**

#### **1.1 Why Program**  
not been recorded

#### **1.2 Hardware Overview**

1. When you write a program, you create a file on the secondary memory, like a Python file, and then at some point that is loaded into the main memory, translated, and then your program is here. And then when the CPU says what next, your program feeds its first instruction. And then when that's done, the CPU says what's next? It feeds the second instruction, third instruction, fourth instruction. It's called the **fetch-execute cycle**.

2. Definitions  

   (1) **Central Processing Unit (CPU)**: Runs the program - The CPU id always wondering "what to do next". Not the brains exactly - very dumb but very very fast.  
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
   I svae the file as **_HelloWorld.py_**.  

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
   (3) Story structure: constructing a prigram for a purpose  

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
   (4) As a convention, we ad **".py"** as the suffix on the end of these files to indicate they contain Python.  

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
   print('Finis')
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

1. When Python is running in the interactive mode and displaying the chervron prompt(>>>) - what question is Python asking you?  

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

   A variable is a memory location used to store a value (0.6). The value stored in a variable can be updated by replacing the old value (o.6) with a new value (0.936)

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

   Remeber the rules top to down (Parenthesis; Power; Multiplication; Addition; Left to right)

   When writing code - use parenthses

   When writing coed - keep mathematical expressions simple enought that they are easy to understand

   Break long series of mathematical perations up to make them more clear


4. What dose "Type" mean?

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
   


---

### **_Week 5_**


---

### **_Week 6_**


---

### **_Week 7_**


---
## For GitHub
[语法](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)



