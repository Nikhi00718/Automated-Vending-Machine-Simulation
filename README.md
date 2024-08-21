# Vending Machine Simulator

## Description

his Python program simulates a basic automated vending machine. The machine allows users to select items, insert money, and dispense items. The program makes use of for and while loops, as well as break and continue statements, to control the vending process.

## Features

- **Item Selection:** Choose items from a predefined list using item codes.
- **Payment Handling:** Insert money until the total amount covers the cost of the selected items.
- **Transaction Confirmation:** Confirm or cancel the transaction before finalizing the purchase.
- **Change Management:** Calculate and manage change, with an option to retain change for future purchases.
- **Error Handling:** Handles invalid inputs and insufficient funds.

## Expected Outputs
'''1. Selecting an Item:
When a user selects an item and provides sufficient money, the output will be as follows:

Available items:

Item A - Price: $1

Item B - Price: $2

Item C - Price: $3

Enter the item code to select (A, B, C) or type 'exit' to leave: A

Enter the quantity of the item you need: 2

Insert money ($2 more required): $3

Do you want to confirm the payment (y/n): y

Dispensing item A. Your change is $1.0

Do you want to add the channge to the shopping card (yes/no): no

Take this change: $1.0

*2. Invalid Item Selection:
If the user inputs an invalid item code, the script will display an error message:

Enter the item code to select (A, B, C) or type 'exit' to leave: D

Invalid selection. Please try again.

*3. Insufficient Funds:
If the user does not initially insert enough money, the script will prompt for additional funds:

Enter the item code to select (A, B, C) or type 'exit' to leave: B

Enter the quantity of the item you need: 3

Insert money ($6 more required): $5

Insert money ($1 more required): $1

##Expected Errors
*1.Non-Numeric Input for Quantity:

Enter the quantity of the item you need: two

ValueError: invalid literal for int() with base 10: 'two'

*2.Non-Numeric Input for Money:

Insert money ($3 more required): ABC

ValueError: could not convert string to float: 'abc'
'''

