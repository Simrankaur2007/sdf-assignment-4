# PiXELL Transaction Report

#Description

This project involves modifying and troubleshooting the `pixel_transaction_data.py` Python script to process transaction data from a CSV file. The script reads transaction records, validates them, and reports the results.


## Author
[Simran Kaur]


### Assignment Description

This project is related to an assignment that aims to ensure the correctness and accuracy of software programs and the appropriate use of exception handling. As a student, the goal is to improve the quality of the "pixell_transaction_report" program.



### Code Modifications

#### Exception Handling

The code has been modified to include exception handling. We wrapped the code that reads the CSV file in a try-except block to handle potential exceptions. If the file is not found (FileNotFoundError), an error message is displayed. Additionally, we added a generic exception handler to capture any other unexpected errors.

#### Data Validation

Data validation has been implemented to ensure the input data is correct:

1. **Transaction Type Validation**: We added code to validate the transaction type. If the transaction type is not in the list of valid types, the record is marked as invalid.

2. **Transaction Amount Validation**: We implemented validation for the transaction amount. If the amount cannot be converted to a float (i.e., it's not numeric), the record is marked as invalid.

#### Collecting Invalid Records

Invalid records are now collected in a list named `rejected_records`. This list contains tuples, where each tuple contains the invalid record itself and an error message explaining why it's invalid.

### Initial Test

Before making modifications, the code was initially tested with a single valid record in the input file to ensure it executed without errors.

### Troubleshooting

The code was further tested and debugged to ensure it produced the expected results. Any issues that arose were identified and fixed.

### Incorporating Additional Test Data

The code was tested with incremental test data, adding one record at a time to the input file. This helped ensure that the program worked correctly with various data scenarios.

### Final Review

A final review of the code was conducted to verify that it produced correct results and complied with PEP8 standards. Inline comments were added for clarity.

### Usage

To use the code, ensure that the `bank_data.csv` file contains valid transaction records. You can then run the `pixel_transaction_data.py` script to process the data and generate the transaction report.

