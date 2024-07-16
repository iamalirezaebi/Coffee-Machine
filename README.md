
Coffee Machine Project
This is a simple console-based coffee machine simulation written in Python. The program allows users to order different types of coffee, checks for sufficient resources, processes payments, and deducts the used resources from the machine's inventory. This project is part of the "100 Days of Code: The Complete Python Pro Bootcamp for 2023" by Angela Yu.

### Table of Contents
#### Features
#### Project Structure
#### Requirements
#### Usage
#### How It Works
#### Menu and Resources
#### Functions
#### Example Interaction
#### Features
Offers three types of coffee: Espresso, Latte, and Cappuccino.
Checks if there are sufficient resources before making the coffee.
Processes coin input from the user and calculates the total amount.
Determines if the transaction is successful based on the amount paid.
Dispenses coffee and deducts the used resources from the inventory.
Provides a report of current resources and profit when requested.
#### Project Structure
MENU: Dictionary containing details of the available coffee options, their ingredients, and costs.
resources: Dictionary containing the initial quantities of water, milk, and coffee available in the machine.
Various functions to handle the operations of the coffee machine.
Main loop to interact with the user.
#### Requirements
Python 3.x
#### Usage
Clone the repository or download the Python script.
Run the script using a Python interpreter.

python coffee_machine.py
Follow the on-screen prompts to interact with the coffee machine.
#### How It Works
Menu and Resources
The MENU dictionary defines the available coffee options (espresso, latte, cappuccino) along with their required ingredients and costs. The resources dictionary defines the initial amounts of water, milk, and coffee available in the machine.

#### Functions
is_resource_sufficient(order_ingredient): Checks if there are enough resources to make the selected coffee. Returns False if resources are insufficient and prints a message indicating which resource is lacking.
is_transaction_successful(money_received, drink_cost): Checks if the money received is sufficient to cover the cost of the coffee. If sufficient, adds the cost to the profit and returns True, else returns False and prints a refund message.
process_coins(): Prompts the user to input the number of coins and calculates the total money received.
make_coffee(drink_name, order_ingredients): Deducts the required ingredients from the resources and prints a message serving the coffee.
Main Loop
The main loop runs continuously, prompting the user for their choice of coffee. It handles commands to turn off the machine (off) and to print a report of current resources (report). If a coffee is selected, it checks for sufficient resources, processes the payment, and if successful, makes the coffee.

#### Example Interaction
vbnet

What would you like? (espresso/latte/cappuccino): latte
Please insert coins.
How many quarters?: 10
How many dimes?: 0
How many nickels?: 0
How many pennies?: 0
Here is $0.0 in change.
Here is your latte ☕️. Enjoy!

What would you like? (espresso/latte/cappuccino): report
Water: 100ml
Milk: 50ml
Coffee: 76g
Money: $2.5
Conclusion
This coffee machine project demonstrates basic principles of Python programming, including working with dictionaries, functions, loops, and user input. It is a good example of a simple, interactive console application.
