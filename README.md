# Restaurant-Analysis

This Python script is designed to analyze sales and menu data for a hypothetical restaurant, aiming to consolidate the information into a comprehensive report. The process involves several key steps, detailed as follows:

1. **Importing Necessary Libraries**: The script begins by importing the `csv` library for reading CSV files and the `Path` class from `pathlib` for file path operations.

2. **Setting File Paths**: It sets the paths to the `menu_data.csv` and `sales_data.csv` files, which contain details about the restaurant's menu items and sales transactions, respectively.

3. **Initializing Data Structures**: Two lists, `menu` and `sales`, are initialized to hold the data from the respective CSV files. Additionally, a dictionary named `report` is initialized to store the consolidated sales report.

4. **Reading CSV Data**: The script reads the menu and sales data from their respective files, skipping the header row and appending each row of data to the `menu` and `sales` lists.

5. **Analyzing Data**: The core of the script involves analyzing the sales data with regards to the menu items. For each item sold (from the sales data), it checks if the item exists in the menu data. If so, it calculates and tracks metrics such as total quantity sold, total revenue, total cost, and total profit for each item.

6. **Report Generation**: For items found in both the sales and menu data, the script updates the `report` dictionary with the calculated metrics. This involves incrementing counts, revenue, cost, and profit for each matching item based on the quantity sold and the item's price and cost.

7. **Error Handling**: If a sales item does not match any item in the menu data, a message is printed to indicate the mismatch. This step ensures that only valid matches contribute to the report metrics.

8. **Output**: Finally, the script prints the total number of records processed and writes the compiled report to a text file named `report.txt`. Each line of the report file contains a menu item's name followed by its aggregated metrics.

The script effectively bridges the data between sales transactions and menu offerings to provide valuable insights into the performance of each menu item, highlighting areas of success and potential improvement.
