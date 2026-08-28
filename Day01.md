# DAY - 01

1. **Program to Print Integer Numbers Entered by the User:**

   Write a program where the user is asked to enter an integer number, and the program prints that number back to them. For example:

   - **Input:** **`42`**
   - **Output:** **`You entered: 42`**

   #### Solution:
   <details>
   <summary><b>👀 Click to see the solution</b></summary>

   ```python
   def IntergerNum():
       while True:
           user_input = input("Please Enter an Integer number: ")
           if user_input.isdigit():
               num = int(user_input)
               return num
           else:
               print("Invalid input. That is not a number!")
       
   print("You Entered:", IntergerNum())
   ```

   <details>
   <summary><b>🖥️ Click to see how the console output looks</b></summary>

   ```text
   Please Enter an Integer number: hello
   Invalid input. That is not a number!
   
   Please Enter an Integer number: 45.5
   Invalid input. That is not a number!
   
   Please Enter an Integer number: 42
   You Entered: 42
   ```
   </details>

   </details>

2. **Write a Program to Find the Size of `int`, `float`, `double`, and `char` on Your Computer:**

   Write a program that displays the size of fundamental data types (**`int`**, **`float`**, **`double`**, and **`char`**) on your system. For example:

   - **Output:**
     ```jsx
     Size of int: 4 bytes
     Size of float: 4 bytes
     Size of double: 8 bytes
     Size of char: 1 byte
     ```
   #### Solution:
   <details>
   <summary><b>👀 Click to see the solution</b></summary>

   ```python
     import sys
     import ctypes

     def FindTheSize():
       # user_input=input("Enter to find the size in bytes:")
       print(f"Size of Int: {sys.getsizeof(int())} bytes")
       print(f"Size of Float: {sys.getsizeof(float())} bytes")
       print(f"Size of String: {sys.getsizeof(str())} bytes")

     def FindtheCTypeSize():
        numIntInC=ctypes.sizeof(ctypes.c_int)
        print("Size of int in C:", numIntInC ,"bytes")

     FindTheSize()    
     FindtheCTypeSize()    
     ```

   <details>
   <summary><b>🖥️ Click to see how the console output looks</b></summary>

   ```text
   Size of int: 28 bytes
   Size of Float: 24 bytes
   Size of String: 41 bytes
   Size of int in C: 4 bytes

   ```
   </details>

   </details>
