# Debugging-a-Sales-Data-Workflow

## Project Overview

This project is focused on loading and checking data from a CSV file named 'sales.csv'. It involves various steps to ensure the integrity and correctness of the data. The primary goal is to perform data quality checks and identify any discrepancies or issues within the dataset.

## Project Structure

The project consists of a Python script containing the following components:

1. **Importing Libraries:**
   - The script begins by importing the necessary Python libraries, including `pandas` and `numpy`.

2. **Data Loading:**
   - The data is loaded from the 'sales.csv' file using the `pd.read_csv()` function.

3. **Step 1: Check the Loaded Data:**
   - This step checks whether the data was loaded correctly by comparing the number of columns to an expected value. If the shape of the loaded data is different from the expected shape (17 columns), a message is displayed to prompt further investigation. Otherwise, a success message is printed.

4. **Step 2: Data Integrity Check:**
   - In this step, data integrity checks are performed on the loaded dataset.
   - The data is grouped by the 'Date' column, and statistics like mean and standard deviation of the 'Total' column are calculated.
   - A threshold is defined as three times the standard deviation.
   - Upper and lower bounds are established based on the mean and threshold for each date.
   - Two conditions ('Condition_1' and 'Condition_2') are created to check data integrity.
   - A new column 'Tax_calculated' is added to the data, representing the calculated tax.
   - A new condition ('Condition_3') is created to check the correctness of the tax calculation.
   - All three conditions are used in an if statement to detect any issues with the data.
   - Depending on the results of the conditions, either a message indicating a successful data integrity check or a message suggesting further investigation is printed.

## Usage

To use this project, follow these steps:

1. Ensure you have Python installed on your system.

2. Place the 'sales.csv' file in the same directory as the Python script.

3. Run the Python script, which will load and check the data.

## Conclusion

This project provides a structured approach to loading and performing data integrity checks on a dataset from a CSV file. It helps identify and flag any potential data quality issues, ensuring the reliability of the data for further analysis or processing.

For any questions or concerns about this project, please contact the project owner.

Thank you for using this data integrity check script!
