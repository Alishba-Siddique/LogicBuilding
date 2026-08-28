# DAY - 01

1. **Program to Print Integer Numbers Entered by the User:**

   Write a program where the user is asked to enter an integer number, and the program prints that number back to them. For example:

   - **Input:** **`42`**
   - **Output:** **`You entered: 42`**

   #### Solution:

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
   <summary><b>👀 Click to see how the console output looks</b></summary>
   
   ```text
   Please Enter an Integer number: hello
   Invalid input. That is not a number!
   
   Please Enter an Integer number: 45.5
   Invalid input. That is not a number!
   
   Please Enter an Integer number: 42
   You Entered: 42
   ```
   </details>
   
