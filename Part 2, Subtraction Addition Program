def get_number_input(prompt):
    while True:
        try:
            return float(input(prompt))
        except ValueError:
            print("Invalid input. Please enter a valid number.")

def calculator():
    """
    Performs either addition or subtraction based on user input.
    """
    operation_map = {
        '+': 'addition',
        '-': 'subtraction',
        'addition': '+',
        'subtraction': '-'
    }

    while True:
        op_input = input("Do you want to perform Addition (+) or Subtraction (-)?: ").strip().lower()
        if op_input in operation_map:
            # Standardize the operation symbol for consistent logic
            operation = operation_map.get(op_input, op_input) 
            print(f"You chose {operation_map[operation]}." if operation in ['+', '-'] else f"You chose {op_input.capitalize()}.")
            break
        else:
            print("Invalid input. Please enter '+' or '-' for the operation.")

    num1 = get_number_input("Enter the first number: ")
    num2 = get_number_input("Enter the second number: ")

    if operation == '+':
        result = num1 + num2
        print(f"The sum of {num1} and {num2} is: {result}")
    elif operation == '-':
        result = num1 - num2
        print(f"The difference between {num1} and {num2} is: {result}")

# Call the calculator function to run the program
calculator()
