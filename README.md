## Pharmacy/Medical Store Management System Documentation

### Overview:

This C program implements a simple Pharmacy/Medical Store Management System using a console-based interface. The system allows users to add medicines to an inventory, display the current inventory, and exit the program.

### Code Structure:

1. **Medicine Structure:**
    - The program defines a structure named `Medicine` to represent individual medicines. Each medicine has three attributes: `name` (string), `quantity` (integer), and `price` (float).

    ```c
    struct Medicine {
        char name[50];
        int quantity;
        float price;
    };
    ```

2. **Function Definitions:**

    - **`displayMedicine` Function:**
        - Displays the details of a given medicine.

    - **`addMedicine` Function:**
        - Allows the user to input details for a new medicine and adds it to the inventory. The function takes an array of medicines (`medicines`) and a count of existing medicines (`count`) as parameters.

    - **`displayInventory` Function:**
        - Displays the entire inventory of medicines. If the inventory is empty, it prints a corresponding message.

3. **Main Function:**

    - The `main` function initializes an array of `Medicine` structures named `medicines` with a capacity for 100 medicines. It also maintains a `count` variable to keep track of the number of medicines in the inventory.

    - It utilizes a `do-while` loop to repeatedly display a menu of options to the user until the user chooses to exit (`choice == 0`).

    - The menu provides the following options:
        - **1. Add Medicine:** Calls the `addMedicine` function to add a new medicine to the inventory.
        - **2. Display Inventory:** Calls the `displayInventory` function to show the details of all medicines in the inventory.
        - **0. Exit:** Exits the program.

    - The program uses a `switch` statement to execute the chosen option and handles invalid choices with a default case.

### Usage:

1. **Adding Medicine:**
    - Select option 1 from the menu.
    - Enter the name, quantity, and price of the medicine when prompted.

2. **Displaying Inventory:**
    - Select option 2 from the menu.
    - The program will display details for each medicine in the inventory.

3. **Exiting the Program:**
    - Select option 0 from the menu.
