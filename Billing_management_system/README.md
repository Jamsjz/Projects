# Operations

## 1. Adding a New Record (`addRecord` Function)
- Prompts the user to input customer information (name, phone number, and usage in minutes).
- Calculates the total bill based on usage.
- Adds the new record to the `customers` array.

## 2. Viewing List of Records (`viewRecords` Function)
- Prints a table header.
- Iterates through the `customers` array and prints each customer's information.

## 3. Modifying a Record (`modifyRecord` Function)
- Takes a phone number as input to identify the record to be modified.
- Prompts the user to enter the new usage in minutes.
- Updates the total bill based on the new usage.

## 4. Viewing Payment (`viewPayment` Function)
- Takes a phone number as input to identify the record to be viewed.
- Prints the name, phone number, usage, and total bill for the specified customer.

## 5. Deleting a Record (`deleteRecord` Function)
- Takes a phone number as input to identify the record to be deleted.
- Shifts the remaining records to fill the gap created by the deleted record.

## 6. Displaying Menu and Main Loop (`displayMenu` and `main` Functions)
- Displays a menu with options for different operations.
- Takes user input to execute the chosen operation.
- The program continues to run until the user chooses to exit.
