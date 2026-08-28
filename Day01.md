# DAY - 01

1. **Program to Print Integer Numbers Entered by the User:**

   Write a program where the user is asked to enter an integer number, and the program prints that number back to them. For example:

   - **Input:** **`42`**
   - **Output:** **`You entered: 42`**

### Try It Yourself

[![Run in Browser](https://shields.io)](https://onecompiler.com)

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
