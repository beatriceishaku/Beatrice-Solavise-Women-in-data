```python
# Program to calculate average marks and display grade

# Ask the user to enter marks for Math, Science, and English
try:
    math = float(input("Enter your Math marks (0 - 100): "))
    science = float(input("Enter your Science marks (0 - 100): "))
    english = float(input("Enter your English marks (0 - 100): "))

    # Check if all inputs are valid (between 0 and 100)
    if 0 <= math <= 100 and 0 <= science <= 100 and 0 <= english <= 100:
        # Calculate average
        average = (math + science + english) / 3

        print(f"\nYour average score is: {average:.2f}")

        # Special cases first
        if average == 100:
            print("Wow! You got a perfect score")
        elif average == 0:
            print("Oh no! You failed everything")
        # Grade conditions
        elif average >= 90:
            print("Excellent! You got an A")
        elif 80 <= average <= 89:
            print("Very Good! You got a B")
        elif 70 <= average <= 79:
            print("Good! You got a C")
        elif 60 <= average <= 69:
            print("Needs Improvement! You got a D")
        else:
            print("Fail! You got an F")
    else:
        print("Invalid input. Try again!")

except ValueError:
    print("Invalid input. Please enter numeric values only!")

```

    Enter your Math marks (0 - 100):  50
    Enter your Science marks (0 - 100):  60
    Enter your English marks (0 - 100):  70


    
    Your average score is: 60.00
    Needs Improvement! You got a D



```python

```
