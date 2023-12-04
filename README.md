# Armstrong
def is_armstrong_number(num):
    if not num.isdigit():
        print("Please enter a valid number.")
        return False

    num_digits = len(num)
    total = sum(int(digit) ** num_digits for digit in num)
    
    return int(num) == total

# Example: Check if a number is an Armstrong number
number = input("Enter a number: ")
if is_armstrong_number(number):
    print(f"{number} is an Armstrong number.")
else:
    print(f"{number} is not an Armstrong number.")
