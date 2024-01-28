# Filename: number_classifier.py

# Function to check if a number is even
def is_even(number):
    return number % 2 == 0

# Function to classify the number and return a message
def classify_number(user_input):
    if user_input == 0:
        return "The entered number is zero."
    elif is_even(user_input):
        return "The entered number is even."
    else:
        return "The entered number is odd."

# Main function to execute the program
def main():
    try:
        # Prompt user for input
        user_input = int(input("Enter a number: "))
        
        # Call the classify_number function and print the result
        result_message = classify_number(user_input)
        print(result_message)
    
    except ValueError:
        # Handle invalid input
        print("Invalid input. Please enter a valid number.")

if __name__ == "__main__":
    # Run the main function when the script is executed
    main()
