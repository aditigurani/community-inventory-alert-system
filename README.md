# community-inventory-alert-system

1. Project Overview

The **Community Inventory Alert System** is a Python-based project designed to help small shops, community stores, and inventory managers track stock levels and identify items that need restocking.

The program records the quantities of items sold, updates the current inventory, and displays a report showing which items have low stock.

 2. Problem Statement

Small community stores may find it difficult to manually monitor inventory and identify products that are running low. This project provides a simple command-line system to update inventory based on daily sales and highlight items that require restocking.

 3. Objectives

* Track the stock of predefined inventory items.
* Record quantities sold.
* Update inventory after sales.
* Identify items below the minimum stock threshold.
* Display a restock report and a full inventory status report.
* Validate user input and handle invalid entries.

 4. Main Features
 Inventory Tracking
The program maintains stock quantities for items such as Milk, Bread, Eggs, Sugar, Tea, Rice, Biscuits, and Oil.

 Sales Entry
Users enter the item name and quantity sold. The program checks whether the item exists and whether the entered quantity is valid.
Low-Stock Alerts

Items with stock below the minimum stock threshold are identified for restocking.

Restock Report

The program displays a list of items that need restocking and their current quantities.

 Inventory Status Report

The program displays the current quantity and status of each inventory item.

 5. Technologies Used

Programming Language: Python 3
Development and Testing Platform: OneCompiler
Version Control and Repository: GitHub

 6. Requirements

* A web browser
* Internet connection
* Access to OneCompiler for running the Python program

 7. How to Run

1. Open the Python program in OneCompiler.
2. Make sure the complete `main.py` code is present.
3. Click the **Run** button.
4. Enter the item sold when prompted.
5. Enter the quantity sold.
6. Continue entering sales or type `done` to finish.
7.Review the restock report and full inventory report.

 8. How the System Works

The program starts with a predefined inventory.

The user enters the items sold during the day and the quantities sold.

The program then:

1. Checks whether the entered item exists.
2. Checks whether the quantity is a valid number.
3. Rejects negative quantities.
4. Rejects a sale quantity greater than the available stock.
5. Records valid sales.
6. Updates the inventory.
7. Checks which items are below the minimum stock threshold.
8. Displays the restock report.
9. Displays the complete inventory with its current status.

9. Stock Alert Logic

The minimum stock threshold is set to 5 units.

- If an item's stock is below 5, its status is `LOW`.
 -If an item's stock is 5 or greater, its status is `OK`.

Items with a `LOW` status are included in the restock report.

 10. Data Structures Used

Dictionary: Stores inventory item names and their quantities.
List: Stores sales entered during the current program session.
Tuple: Stores each sale as an item name and quantity.
Set: Helps avoid duplicate items in the restock list.

11. Input Validation and Error Handling

The program checks that:

* The item exists in the inventory.
* The quantity entered is a valid integer.
* The quantity is not negative.
* The quantity sold does not exceed the available stock.

Invalid entries display an appropriate message and allow the user to continue.

12. Limitations

* The inventory is predefined in the source code.
* Inventory changes are not permanently saved between program runs.
* The program uses a command-line interface.
* New inventory items cannot currently be added through the program.
* Historical sales are not permanently stored.

 13. Future Enhancements

Possible future improvements include:

* Adding new inventory items through the program.
* Saving inventory data in a file or database.
* Generating daily, weekly, and monthly reports.
* Adding user authentication and different user roles.
* Creating a graphical user interface.
* Adding automated tests.
* Adding permanent sales history.

 Conclusion
 
The Community Inventory Alert System demonstrates how Python can be used to manage basic inventory operations, process sales input, validate quantities, and identify items requiring restocking.

The project provides a foundation for developing a more complete inventory management system in the future.


