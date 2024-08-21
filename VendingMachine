a = [1, 2, 3]  # Amount of the items
b = ["A", "B", "C"]  # Item codes
total_inserted = 0  # Track total money inserted by the user

# This while loop will continue until the user types 'exit'
while True:
    print("\n")
    print("Available items: ")
    
    # This loop prints all the items with their respective prices
    for item, price in zip(b, a):
        print(f"Item {item} - Price: ${price}")

    # Ask the user for their item choice
    selection = input("Enter the item code to select (A, B, C) or type 'exit' to leave: ").upper()
    
    # If the user types 'exit', the program will terminate
    if selection == 'EXIT':
        print("Thank you for using the vending machine. Goodbye!")
        break

    # Check if the selection is valid
    elif selection not in b:
        print("Invalid selection. Please try again.")
        continue

    # Ask the user for the quantity of the item they need
    no = int(input("Enter the quantity of the item you need: "))

    # Calculate the total amount required based on the item price and quantity
    item_price = a[b.index(selection)]
    wanted_amount = item_price * no

    # Loop until the user inserts enough money
    while total_inserted < wanted_amount:
        money = float(input(f"Insert money (${wanted_amount - total_inserted} more required): $"))
        total_inserted += money
        
    # Confirm the payment from the user
    cho = input("Do you want to confirm the payment (y/n): ").lower() 
    if cho == "n":
        print("Transaction cancelled.")
        break

    # If payment is confirmed and sufficient, dispense the item and calculate change
    if total_inserted >= wanted_amount:
        change = total_inserted - wanted_amount
        print(f"Dispensing item {selection}. Your change is ${change}.")

    # Ask the user if they want to add the change to the shopping card
    change_cho = input("Do you want to add the change to the shopping card (yes/no): ").lower()
    if change_cho == "yes":
        total_inserted = change  # Retain the change for future purchases
    else:
        total_inserted = 0  # Reset total_inserted and provide the change to the user
        print(f"Take this change: ${change}")
