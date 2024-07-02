1:python basics: Python is a high-level, general-purpose programming language. Its design philosophy emphasizes code readability with the use of significant indentation.
  Key features of Python;
  -Easy Readability because of its clean and straight forward syntax
  -Has a rich standard library which includes modules for various functionalities eg, system calls,file input and output.
  -Cross platform compatibility which makes python a versatile choice for developing applications that need to run on different envirnments eg;windows,macOS, Linux and Unix systems.
  -Has a wide and large support communty and ecosystem which leads to rich contributions to third party libraries and frameworks eg  Django and Flask.
        Use cases of Python:
    -Web development using frameworks like django and flask for routing,integration and from handling tasks.
    -Automation and Scripting because of its ease of use and broad library make it ideal for automating repetitive tasks and scripting.
    -Data science and Machine Learning: Python leverages frameworks like pandas,Numpy,MatplotLib to be effective in data analysis and machone learning objectives.
    -Game Development:Python ca also be used to develop games using pygame library.

2. Installing Python:
     -Go to the official Python website([python](https://www.python.org/)) and download th elatest version of python suitable for windows.
     -Run the installer, by oepning the .exe file and follow the installation wizards directions.
     -After installing open the command prompt and type python --version to check if python was installed in the system.
     -Install the virtual environment by running the command pip install virtualenv and then navigate to your projst directory using the command prompt.
     -Create a virtual envirnment with yourr prefered name (eg,,myenv) and run the envirnment by typing the command virtualenv myenv.
     -Activate the envirnment by running myenv\Scripts\activate.mtenev should appear at the beginning of your commmand prompt.
        macOS:
        -Go to the official Python website([python](https://www.python.org/)) and download th elatest version of python suitable for macOS.
        -Open the downloaded .pkg file and follow the installation instructions.
        Open Terminal.
        -Type python3 --version and press Enter. You should see the version number of Python 3.x.
        -First, ensure you have pip installed by running sudo easy_install pip.
        -Navigate to your project directory in Terminal.
        -Create a virtual environment named myenv by running python3 -m venv myenv.
        -Activate the virtual environment by running source myenv/bin/activate. You'll notice (myenv) appears at the start of your terminal prompt, indicating the virtual environment is active.
        Linux:(most linux distributors come with python installed although you can confirm by following the below directions)
        -Open a terminal and update your package list (sudo apt-get update).
        -Install Python by running sudo apt-get install python3.
        -In the terminal, type python3 --version and press Enter. You should see the version number of Python 3.x.
        -Ensure pip is installed by running sudo apt-get install python3-pip.
        -Navigate to your project directory in the terminal.
        -Create a virtul environment named myenv by running python3 -m venv myenv.
        -Activate the virtual environment by running source myenv/bin/activate. You'll see (myenv) at the start of your terminal prompt, indicating the virtual environment is active.

3:Python Syntax and Semantics:
  simple python program 
   print('Hello world!)

   print():a built in python fucntion sued to output data to the screen.
   -string literals; sequence of characters enclosed in the quotes.

4:Data Types and Variables:
   -Numbers(int): Whole numbers, positive or negative, without decimals
     integer_var = 10

   -Float (float): Real numbers, containing a decimal point or represented in scientific notation, e.g., 3.14, 1.61803398875e+00.
        float_var = 10.5

   2:Sequences;
   -string(str):sequence of characters eg, "coding"
       string_var = "Hello, coding!"

   -list(list):an ordered collection of items indexed by integers  mutable (can be changed)
      list_var = ["BMW", "Mercedes", "Audi"]

   -tuple(tuple):similar to list but immutable, meaning once create dthey cannot be changed.
      tuple_var = ("BMW", "Mercedes", "Audi")

   3:Mappings:
   -Dictionary(dict):an unordered collection of key-value pairs eg {key: value}
      dict_var = {"name": "Mike", "age": 27}
   4:Booleans(bool):represents true or false
        boolean_var = True
        boolean-var = False

   5:None(None)
   -a special type of constant in Python that represents athe absence of a value or a nulll value
     none_var = None

    Usage:
    print(f"Integer: {integer_var}")
    print(f"Float: {float_var}")
    print(f"Complex Number: {complex_var}")
    print(f"String: {string_var}")
    print(f"List: {list_var}")
    print(f"Tuple: {tuple_var}")
    print(f"Dictionary: {dict_var}")
    print(f"Boolean: {boolean_var}")
    print(f"None: {none_var}")

5:Control Structures:Conditional statements and loops are fundamental control flow mechanisms in Python, allowing programs to execute certain sections of code based on conditions or repeatedly until a condition is met.
    Conditional statements;
    They enable the execution of of code blocks based on whether a specified condition evaluates to true or false.
    example of an if-else statement;
    age = 35
    if age > 35:
          print("No longer young")
        else("You are still young")

    Loops;They allow a block of code to be executed reeatedly untill a certain condition is no longer met.
    example of a for loop;
     items = ["bike","book","car","apple"]
     for item in items:
        print(item)

 -This loop prints all the items and stops when all the items are printed.

6: Functions in Python:
  -Functions are reusable pieces of code taht perform a specific task.
  -They are useful because they enable developers like me to organize code into loical units that are easier to understand, test and debug.
   Example of a python function that take two arguments and returns their sum;

     def add_numbers(a, b);
     return a + b 

     sum = add_numbers(7, 8)
     print("The sum is:", sum)

7:Lists and Dictionaries:
 -List are ordered collection of items which can be of any type while dictionaries are  unordered collection of key-value pairs whereby each key is unique.
 -Lists are best suited for sequential data where order matters while dictionaries are ideal for mapping data where you want to associate values with unique keys eg, storing phone numbers associated with conatact names.
 -list are accessed via indexing eg, (list[0]),while dictionaries are accesses via keys dict["key].
   Basic Operations;
   //creating a list of items

   items_list = ["potato","beans","pen","car"]
   //accessing an element in the list
   first_item = items_list[2]
   print(firts_item) //pen

   //modify and element
   items_list[1] = 17
   print(items_list) //changes beans to 17

   //append an element 
   items_list.append(6)
   print(items_list)

  //removing an element
   items_list.remove(1)
   print(items_list)

   Creating and manipulating a dictionary;
   //Create a dictionary with key-value pairs
   contacts_dict = {
    "Hannah": "hannah@example.com",
    "Mike": "mike@example.com"
}

  // Access a value
  alice_email = contacts_dict["Hannah"]
  print(hannah_email)

  //Modify a value
  contacts_dict["Hannah"] = "hannah@example.com"
  print(contacts_dict)

 // Add a new key-value pair
  contacts_dict["Charlie"] = "charlie@example.com"
  print(contacts_dict)

  //Remove a key-value pair
  del contacts_dict["Mike"]
  print(contacts_dict)

8: Exception Handling:Exception handling in Python is a mechanism that allows you to deal with unexpected situations that occur during the execution of your program.
  - By using exception handling, you can prevent your program from crashing unexpectedly and provide meaningful error messages to the user or take corrective actions.
  -Python uses try, except, and finally keywords in exception handling
  -try--conatins the code segment that might throw an exception
  -except--handles the exception thrown in the try block, you can have mutiple except blocks to catch different type sof exceptions.
  -finally--contains code that will be executed regardless of whether an exception was raised or not.

  example,,
   try
     result = 10 /0
     print(result)
    except zeroDivisionError:
      print("Cannot divide by zero")
    finally:
      print("Finished calculation")

9:Modules and Packages:In Python, modules and packages are fundamental components for organizing code into reusable and modular units, promoting better code management and collaboration.
  -a module is a single python file (with .py extension) that contains Python definitions and statements.
  -you use the import statement followed by the module name . eg,,
   print(math.sqrt(16))
  -packages is a way of organising related mdules into a single directory hierarchy.
    from mypackage import mymodule

  //Now you can use functions from mymodule
   //mymodule.my_function()

   example of using a math module

   import math

   //calculate the square root of 40
   squareRoot = math.sqrt(40)
   print(squareRoot)

10:File I/O:Reading from and writing to files in Python is straightforward thanks to the built-in file handling capabilities.
 -Python provides the open() function to work with files,which can be used with various modes such as 'r'

 //reading a file

for reading 'w' for writing and 'a' for appending.
    Reading from a File
    //define the filename
    filename = 'file.txt'
    
    //open the file in read mode ('r')
    with open(filename, 'r') as file:
    // read the entire content of the file
    content = file.read()
    //print the content to the screen
    print(content)

  //writing a file
   //define the filename
   filename = 'coding.txt'

   //define a list of strings
   lines_to_write = ['Line1' ,'Line2' ,'Line3']
   //open the file in write mode 
   with open(filename, 'w') as file:
     //iterate over the list of strings
      for line in lines_to_write:
      //write each string followed by a newline character
        file.write('line + '\n')
//you can use 'a' mode instead of 'w' to append the file without overwriting exisiting content.
