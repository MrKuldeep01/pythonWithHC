# 👋 Hello Dev. this is review Note for Python 📌

## In this, Am following the great Youtube channel **Chai-Aur-Code** ☕👨‍💻 from well known person **Hitesh_Choudhary**

#### Hnji to kyaa haal he aap sbke, chliA suru krte he...

- **Night One:**

  - installation 📥
  - Hello world 🧬
  - function declaration and call 🚀
  - importing function from another file 🐾
  - A look at inner working of python ⚒

    - Python Script/Code
    - Byte code

      ```javaScript
       [
         {
           mostly : "hidden",
           showWhene : "import/sys_related_tasks",
           running_speed : "higher_then_script",
           can_run_on_another_vm : false,
           send_to : "(PVM)Python_Virtual_Machine",
           machine_code : [false,"!machine_code"]
         },
         {
           __pycache__ : "system_specific_folder",
           double_underscore : true,
           for_what : "to_manage_system_versions_and_binaries",
           work_with : "imported_files",
           not_work_with : "top_level_files",
         },
         {
           PVM : "Python_Virtual_Machine",
           continous_code_loop : true,
           iterate_code : "that's_why_py_called_interprated_language",
           pvm_means : "runtime_engine",
         },
         {
           Python_types :
            { cPython : "Mostly_user",
              jython : "when_working_with_java",
              pypy : "performance_related_work",
              iron_python : "another_type",
              stackless : "another_type",
            }
         },

       ]
      ```

  - Python shell 🐚
  - importing packege like : os, sys, importlib 🛴
  - Short look at variables 🗃
  - for loop ➰
  - some Errors : name error, indentation error, attribute error 🤦‍♂️
  - Mutable / Imutable ✅
    - refrences
    - mostly data types are called object

- **Day Two:**

  - Data/Object types intro.
    - Numbers
    - String
    - List
    - Dictionary
    - Tuple
    - Set
    - Boolean
    - None
    - Files
    - Function, Module, Classes
    - Advanced
      - Decorators
      - Generators
      - Interators
      - Meta Programming
  - Numbers in depth
    - Decimal : base_10
    - Float
      - 'from decimal import Decimal' : A dedicated packege to work with floating point numbers.
    - Binary : base_2
      - 0b1001 : this is the standerd way to assign different types of numbers in programs.
      - int(num,2) : function to convert first argument to the base as second num given in the argument
    - Octal : base_8
      - 0o23476
      - int(num,8)
    - Hex : base_16
      - 0x9fa2
      - int(num,16)
    - Operator precedence
      - best practice is to use () whenever you need to work with multiple operators.
    - casting
      ```python
        pring(4 + 3.1)
        # 7.1 but not a good practice X
        int(123.3)
        # convert the num into integer 123
        float(123)
        # convert the num into float 123.0
        # you have to care about these while dealing with multiple types of numbers
        # best prcatice is to use same data type values while operating.
      ```
    - and or operators
    - true = 1
    - false = 0
    - math packege
      - floor() : always move to the lower values in number line
      - trunc() : always move toword the zero in number line
    - bitwise operators
      - left shift
      - right shift
      - |
      - &
    - random packege
      - random.random()
      - random.randint(start , end + 1)
      - random.choice([])
      - random.shufle([])
    - fraction packege
      - fraction(2,4) : to represent 2/4
  - Sets
    - {1,2,3,4} : values are writen without keys.
    - intersaction : &
    - union : |
    - differences : -
    - empty set will represented as : set() not {}
  - Type Chacking
    - type()
  - Strings in depth
    - single quates, double quates, triple quates
      - 'name'
      - "name"
      - """name
        is kuldeep"""
    - r" " : row string, mostly used in windows path where we deal with multiple slashes.
      - r"c:\\hp\user\home"
    - slic
      - [ start : end + 1 : hopping + 1 ]
      - minus index is allowed
      - str[ 1 : 5 : 2 ] : starting from 1 index to 4 with hopping 1
    - lower()
    - upper()
    - replace("a","b") : replace every "a" in string with "b"
    - split()
      - split the string with given sipirator.
    - find()
      - find the index of given arg in string and return -1 in not found
    - count()
    - return the count of given arg in string
    - format()
      ```python
       str = " I am {} "
       print(str.format("kuldeep"))
       # result : ' I am kuldeep '
      ```
    - join() : to convert the List into String
      ```python
       demo_list = [ "apple", "banana", "orange" ]
       print(", ".join(demo_list))
       # result : apple, banana, orange
      ```
    - len()
      - return the lenth of strign
    - loop on string

      ```python
      str = "abcd"
      for letter  in str:
        print(letter, end(" "))

      # result : a b c d
      ```

    - backslash char
      - \\
      - \"
      - \n
      - \t
    - checks
      - is
        ```python
        a = "str"
        b = "str"
        print(a == b)
        # true
        print(a is b)
        # false
        a = b
        print(a is b)
        # true
        # whole game is walking around memory references
        ```
      - in
        ```python
        a = "str"
        b = "t"
        print(b in a)
        # true
        ```

  - List in depth

    - getting specific index value
    - slicing
    - slicing & assign new values
    - loop in list
      ```python
      demo_list = ["a", 1, 'b', 2]
      for value in demo_list:
        print(value, end(" "))
      # 'a' 1 'b' 2
      ```
    - conditional in list
      - if
        ```python
          if "b" in demo_list:
            print("we have b")
          # we have b
        ```
    - appand() : to adding element in list
    - pop() : remove last element
    - remove() : remove given element
    - insert(index,value) : add a value at given index
    - copy() : to create a copy of List
      - newList = oldList.copy() : oldList's copy into newList
    - List comprehantion

      ```python
        squar_num = [x**2 for x in range(10)]
        print(squar_num)
        # 1,4,9,16,......81  :: 10 is not included

      ```

- **Day Three:**

  - Dictionary in depth

    - declaration
      ```python
        demo_dic = {"name" : "lucky", "age":23}
      ```
    - accessing with key
      - ['name'] : can give an error if not found
      - .get("name") :
    - inserting element
      - my_dictionary["sex"] = "male"
    - removing element
      - my_dictionary.pop("age")
      - my_dictionary.popitem() : remove last last item
    - delete operator
      - del my_dictionary["sex"]
    - can be changed mutable
    - loop in dictionary

      ```python
      for key in demo_dic:
        print(key)
        # name
        # age

      for key,value in demo_dic.items():
        print(key, value)
        # name lucky
        # age 23
      ```

    - conditional in dictionary
      - if
        ```python
          if "age" in demo_dic:
            print(true)
          # true
        ```
    - length
      - len(dictionary)
    - copy()
    - nesting is allowed in dictionary
    - { x : x\*\*2 for x in range(11) } : {0:0,1:1,2:4,3:9,....10:100}
    - clearing full dictionary
      - clear()
    - creating in dictionary from given list of items and assigning them a default value

  - Tuples in depth

    - immutable : not change-able
    - declaration : (comma sipirated values)
    - accessing elements : [ index ]
    - nagitive index allowed : [ -index]
    - slicing / dicing : [ start : end + 1 : hopping ]
    - len()
    - nesting allowed
    - count()
    - type()
    - distructuring : (a,b) = ("value1", "value2")
    - inline conditionals 
    - exit method to stop the exicution of the program

- **Day 4:**
  - Solve 10 conditional questions

    - Learning :
      - input by command line : value = input(" enter any value: ")
      - if, elif
    - age group catagorization : child( > 13 ), teenager( 13 - 19 ), adult(20 - 59), old( > 60 )

    ```python
      age = int(input("enter your age : "))
      if age <= 0 :
          print("invalid age ")

      elif age < 13 :
          print("you are child becase U R : ", age)

      elif age <=19:
          print("you are a teenager because U R : ", age)

      elif age <= 59:
          print("you are an adult because U R : ", age)

      else :
          print("you are an old model because U R : ", age)
    ```

    - movie ticket price :tickets are priced based on age $12 for adult ( 18 and over ), $8 for chilred, 42 discount on wednesday

    ```python

      price = 8 if age < 18 else 12
      price -=2 if iswed =="Y" or iswed =="y" else 0
      print("Hence, ticket price is : ", price )
    ```
    - grade distribution if, elif, else
    - food distribution based in Ripeness based on colour.
    - activity suggestion based on weather
    - transportation selection based on distance
    - coffee customization : 'small', 'mediam', 'large' with an option of extera shot of 'espresso'.[ order+= "espresso extra shot" if espresso== 'yes' else ""]
    - password checker based on length
    - leap year checker : based on divisibility
    - puppy food suggestion based on age for dog, cat
  
  - Solve 10 loop based questions
    - counting of positive num in given list
    - calculate the sum of even number till the given number
      ```python
        num = int(input("enter limit number : "))
        even_sum = 0 
        if num > 100:
            exit()
        for i in range(1,num+1):
            print("running for : ",i)
            if i % 2 == 0:
                even_sum+=i
                print("satisfy for round : ",i)
        print("sum of even numbers is : ",even_sum)
      ```
    - multiplication table printing : 
      - count the table till 10 for given num but skip the fifth count
      ```python
        print("-: table generator :-")
        num = int(input("enter number : "))
        for i in range(1,11):
            if i == 5:
                print("count : ",i, "skipped ✅")
                continue
            print(num ," * ", i , " = ",num*i)

        print("Sir, task completed successfully!")

      ```
    - reverce String using loop
      ```python
        print("-: String reverse :-")
        string  = input("enter string : ")
        reversed_str="";
        for char in string: 
            reversed_str = char+ reversed_str
        #     #k : uk : muk : amuk : ramuk ✅
        print(reversed_str)
      ```
    - - find the first non-repeted char in String using loop
      ```python
        print("-: non repeted char finder :-")
        new_string = ""
        string  = input("enter String : ")
        
        for char in string:
            if string.count(char) == 1 :
                print("char is : ", char)   
                break;
        print("Done")    
      ```
- **Two day's off** 🛴☕
- **Day 5:**      
    - factorial calculator using while loop
      ```python
        print('-: Factorial calculator :-')
        num = int(input("enter number: "))
        factorial_is = 1
        while num > 0:
            factorial_is *= num
            num -= 1
        print('factorial is : ', factorial_is)
      ```
    - validate input : random number game 
      - keep asking till user enter required number and then give the score based on counts
      ```python
        import random
        required_num = random.randint(1,101)
        print("-: Random number game 🎮 :- \n [ 1 - 100 ]")
        count = 0
        while True:
            in_num = int(input("guss the number : "))
            count +=1
            if in_num > 100 or in_num <= 0:
                print("this is out of range!")
                continue
              
            if in_num == required_num:
                print('congratulations 🎉')
                break
              
            if in_num > required_num:
                print('this is big')

            if in_num < required_num:
                print('this is small')
        if count > 10:
            print('not a good try! Thank you.')
            exit()
        score = (11 - count) * 10
        print("Awosome! you scored : '",score,"' \n Because you answered in ",count," time/times \nThank you.")    
      ```
    - find prime number
    ```python
      print(" -: Prime number chacker :-")
      in_num = int(input("enter the number: "))
      is_prime = True
      if in_num > 1:
          for num in range(2, in_num):
              # print("iteration no. : ",num)
              if (in_num % num) == 0 : 
                  print("Noooooope. \nbecause of ",num)  
                  is_prime = False
                  break    
      print("Number's Prime status : ", is_prime,"\n Thank you.")
    ```
    - Learning : 
      - // operation: ' 5 / 2 = 2.5 ' but [' 5 // 2 = 2 ']
    - check the duplicate item in given list print duplicate item and break the loop 
      ```python
        print("-: Duplicate value detector :- ")
        names = ["kuldeep", "deep", "sonu", "deepika" ,"om"]
        duplicate = False
        for item in names: 
            if names.count(item) > 1:
                print('First duplicate item is: ',item)
                duplicate = True
                break
        print('Duplicate status in list : ', duplicate,"\nThank you.")       
      ```
    - list handler
      - adding
      - removing
      - handling inputs
      ```python 
        mylist = []
        i = 0
        print("-: List handler :- \nTo stop : 'x' \tTo step-back : '<'")
        while True:
            in_item = input("enter item : ")
            if in_item == 'x':
                break    
            elif len(in_item) < 1:
                print('iteration : ',i,"\t List is : ",mylist)
                continue
              
            elif in_item == '<':
                mylist.pop()
                print('iteration : ',i,"\t List is : ",mylist)
                continue
              
            mylist.append(in_item)
            print('iteration : ',i,"\t List is : ",mylist)
            i += 1
        print("mylist is : ", mylist)    
      ```
    - exponential backoff
      - implement strategy that double wait time b/w retries, starting from 1sec and stop after 5 retries
      - we need to use time module
      ```python
        import time
        print('waiting simulation')
        wait_time = 1 # in sec
        max_tries = 5
        current_try = 0
        while current_try < max_tries:
            print("request No. : ",current_try+1,"\t waiting time : ",wait_time,"sec")
            time.sleep(wait_time)
            print('🎇 Happy diwali🎊\t'*(current_try + 1))
            wait_time *= 2
            current_try += 1

        print('Thank you.')
      ```
    - Scopes
      - local scope
      - globle scope
        globle key word used to manupulate globle variables in sub funcions
        ```python
          x = 1
          def func()
            globle x
            x = 5
            print(x) # x = 5 :: overwriting globle x
          print(x) # x = 5 
        ```
      - closurs
        - bag pack : all required things within 
      - return statement
  
- **Day 5:**
  - Basic function syntax:
    - write a function to calculate sqaure of a given number and return
      ```python 
        print("-: Square calculator :-")
        num = int(input("enter number : "))
        def square_of(num):
            return num ** 2

        print("square of ",num,": ",square_of(num))
      ```
  - Sum calculator
    - function that take two params and return their sum 
      ```python
        print("-: Sum finder :-")
        a = int(input("variable 1: "))
        b = int(input("variable 2: "))
        
        def sum_of(a,b):
            return a + b
        print("Sum of ",a,"and ",b,": ",sum_of(a,b))
      ```
  - Polymorphism in function
    - write a function multiply that multiply two number and work on string also
      ```python
        print("-: Multiply hero :-")
        a = input("variable 1: ")
        b = int(input("variable 2 (must to be number): "))
        def multiply (a,b):
            return a * b  
        print("multiplication of given number ",a,"and ",b," : ", multiply(a,b))
      ```
  - Default parameter 
    - create a function that greet user, if data is not provided then show default values
      ```python
        print("-: Welcome Function :-")
        name = input("name : ")
        def greet(name = "user"):
            return "Hello,  "+name+"!\nGreat to see you."
        print(greet(name))
      ```
  - Lambda function :: short hand function notation
    - create a lambda function to calculate cube of given number
      ```python
        print("-: Cube calculator using lambda function :-")
        num = int(input("number: "))
        cube = lambda num : num ** 3
        print('cube of ',num," : ",cube(num))
      ```
  - Function with *args
    - write a fuction that take variable no. of arguments and return their sum
      ```python
        def sum_of(*rest):
            return sum(rest)
        # def sum_of(*rest):
        #   return sum(rest) 
        print("1,2,3,4 : ",sum_of(1,2,3,4))
        print("1,2,3,4,5,6 : ",sum_of(1,2,3,4,5,6))
        print("1,2 : ",sum_of(1,2,))
      ```
  - Function with **kwarg
    - create a function that take number of keyword arguments and print them in format key: value
      ```python
        print("-: **kwargs function")
        def fun(**kwargs):
            for key, value in kwargs.items():
                print(f"{key} : {value}")
        fun(name="kuldeep",age=22, brave="devine")
        fun(name="kuku",age=26)
      ```