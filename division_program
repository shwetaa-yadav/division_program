
#Write a Python program that prompts the user for two integer values and displays the 
#result of the first number divided by the second, with exactly two decimal places displayed. 


def validate_data(value):
    try:
        if not value:
            raise ValueError("Input cannot be empty.")
        if value.isalpha():
            raise ValueError("Input must be a number.")
        return int(value)
    except ValueError as e:
        print(f"Error: {e}")
        return None


def get_integer(prompt):
    while True:
        user_input = input(f"Enter {prompt}: ")
        validated = validate_data(user_input)
        if validated is not None:
            return validated


def perform_division(num1, num2):
    try:
        result = num1 / num2
        return f"{result:.2f}"
    except ZeroDivisionError:
        return "Error: Cannot divide by zero."


def run_division_program():
    num1 = get_integer("the numerator (first number)")
    num2 = get_integer("the denominator (second number)")
    
    result = perform_division(num1, num2)
    print(f"\nResult: {num1} / {num2} = {result}")


if __name__ == "__main__":
    run_division_program()

