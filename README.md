# Credit-Risk-Model
Data cleaning and manipulation Using Numpy library


This script is designed to preprocess loan data stored in a CSV file named "loan-data.csv". It performs various data cleaning and manipulation tasks to prepare the data for further analysis. The preprocessing steps include handling missing values, converting string data to numeric format, normalizing currencies, and sorting the dataset. 


1. Importing the Packages:
   - This section imports necessary packages, such as NumPy, and sets print options for better readability of the data.

2. Importing the Data:
   - Reads the loan data from the CSV file into a NumPy array, handling delimiter, skipping headers, and stripping whitespace.

3. Checking for Incomplete Data:
   - Identifies and counts missing values in the dataset.

4. Splitting the Dataset:
   - Splits the dataset into string and numeric columns based on the presence of missing values.

5. Re-importing the Dataset:
   - Reads the string and numeric columns separately from the CSV file into NumPy arrays.

6. Creating Checkpoints:
   - Defines a function to create checkpoints to save intermediate results during preprocessing.

7. Manipulating String Columns:
   - Processes string columns such as issue date, loan status, term, grade, subgrade, verification status, URL, and state address.

8. Manipulating Numeric Columns:
   - Processes numeric columns such as ID, funded amount, loaned amount, interest rate, total payment, and installment.

9. Currency Change:
   - Converts currency from USD to EUR, considering the exchange rate provided in a separate CSV file.

10. Creating the "Complete" Dataset:
    - Combines the preprocessed string and numeric data into a single dataset.

11. Sorting the New Dataset:
    - Sorts the dataset based on a unique identifier, typically ID.

12. Storing the New Dataset:
    - Saves the preprocessed dataset to a new CSV file named "loan-data-preprocessed.csv".
