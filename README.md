# Shopping Cart System

## Overview

This Python project consists of two main classes, `ItemToPurchase` and `ShoppingCart`, along with a set of functions that implement a shopping cart system. The functionality is wrapped in a user-interactive menu within the `print_menu()` function, which is driven by the `main()` function.

## Classes

### `ItemToPurchase` Class

The `ItemToPurchase` class models an item that can be added to the shopping cart. It has the following attributes:
- **item_name**: The name of the item.
- **item_price**: The price of the item.
- **item_quantity**: The quantity of the item.
- **item_description**: A description of the item.

The class provides two methods:
- **`print_item_cost()`**: This method prints the cost of the item by multiplying its price by its quantity.
- **`print_item_description()`**: This method prints the description of the item.

### `ShoppingCart` Class

The `ShoppingCart` class models the shopping cart itself. It contains attributes and methods to manage a collection of `ItemToPurchase` objects:
- **customer_name**: The name of the customer owning the cart.
- **current_date**: The date associated with the cart.
- **cart_items**: A list that stores `ItemToPurchase` objects.

The class provides several methods:
- **`add_item(item)`**: Adds an item to the cart.
- **`remove_item(item_name)`**: Removes an item by name. If the item is not found, it outputs a specific message.
- **`modify_item(item_to_purchase)`**: Modifies the details of an item in the cart based on the provided `ItemToPurchase` object. If the item is not found, it outputs a specific message.
- **`get_num_items_in_cart()`**: Returns the total quantity of all items in the cart.
- **`get_cost_of_cart()`**: Returns the total cost of all items in the cart.
- **`print_total()`**: Prints the details of all items in the cart and the total cost. If the cart is empty, it outputs a specific message.
- **`print_descriptions()`**: Prints the descriptions of all items in the cart.

## Functions

### `print_menu(cart)`

The `print_menu(cart)` function provides a menu-driven interface for the user to interact with the shopping cart. It continuously prompts the user to choose an option until they choose to quit. The options include:
- Adding an item to the cart.
- Removing an item from the cart.
- Changing the quantity, price, or description of an item.
- Printing the descriptions of all items in the cart.
- Printing the total cost and details of the cart.
- Quitting the menu.

Each option corresponds to a method in the `ShoppingCart` class and performs the respective action based on user input.

### `main()`

The `main()` function initializes the shopping cart by prompting the user to enter their name and the current date. It then creates a `ShoppingCart` object and calls the `print_menu(cart)` function to start the interactive menu.

## 

This code effectively demonstrates the use of classes and methods to build a functional shopping cart system in Python. The `ItemToPurchase` and `ShoppingCart` classes encapsulate the data and operations related to items and the cart, respectively. The interactive menu provides a user-friendly way to manage the cart's contents, showcasing the practical application of object-oriented programming principles in Python.
