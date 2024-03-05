# Calculator.py
Calculator Explanations
Function Definitions:
Each function corresponds to a specific arithmetic operation that the calculator can perform. Addition(x, y), Subtraction(x, y), Multiplication(x, y), and Division(x, y) are straightforward functions that take two numbers as input and return the result of the respective operation. Second_power(x) calculates the square of a number. Square_root(x) calculates the square root of a number. These functions runs the core logic of the calculator's operations, making the code easier to understand. The code imports the math module to use the sqrt() function for calculating square roots. It also checks if the input is negative and returns an error message in such cases.

Display Menu Function (display_menu()):
This function is responsible for printing the menu options to the user. The menu provides a simple interface for the user to select the desired operation. It uses print() statements to display each option clearly, making it easy for the user to understand the available choices.

Get Operation Choice Input (get_operation_choice()):
This function prompts the user to input their choice of operation. It uses a while loop to repeatedly prompt the user until a valid choice is entered. It ensures that the input is a valid integer between 1 and 7, corresponding to the menu options. If the input is invalid, it prompts the user to enter a valid choice until they do so.

Get Numbers Function (get_numbers()):
This function is responsible for getting numeric input from the user. It prompts the user to enter two numbers. It uses a while loop to repeatedly prompt the user until valid numeric input is provided. It ensures that the input is valid (numeric) and handles exceptions (ValueError) if non-numeric input is provided. Once valid numeric input is provided for both numbers, they are returned as a tuple.

Main Function (main()):
The main() function serves as the as the main logic/Core of the calculator. It runs in a loop that repeatedly displays the menu, gets the user's choice, and performs the corresponding operations until the user chooses to exit. Within the loop, the menu is displayed, and the user's choice is obtained using get_operation_choice(). Based on the user's choice, the appropriate action is taken: For arithmetic operations (1-4) (addition, subtraction, multiplication, division), two numbers are obtained using get_numbers(), and the corresponding operation is performed. For special operations (5 or 6) (second power, square root), a single number is obtained, and the operation is performed. It handles invalid choices gracefully by providing feedback to the user and prompting them to enter a valid choice. If the user chooses to exit (7), it breaks out of the loop, a goodbye message is displayed and ends the program.

Execution Check (if name == "main":):
This conditional block ensures that the main() function is executed only if the script is run directly as the main program. If the script is imported as a module in another script, the main() function will not be executed automatically, allowing other scripts to utilize the functions defined in this script without running the calculator interface.
