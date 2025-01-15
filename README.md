This Java program is a simple currency converter that uses hardcoded exchange rates to convert an amount from one currency to another. Below is an elaborate description of the program:


---

1. Program Structure

The program is structured into several steps:

Step 1: Input Base and Target Currencies

The program prompts the user to enter the base currency (the currency they have).

The user is then prompted to input the target currency (the currency they want to convert to).

These inputs are converted to uppercase to ensure consistent comparisons.


Step 2: Input the Amount

The user is asked to input the amount they wish to convert.

This amount is stored as a double to handle both whole numbers and decimal values.


Step 3: Hardcoded Exchange Rates

A method named getExchangeRate is defined, which contains hardcoded exchange rates for specific currency pairs (e.g., USD to INR, EUR to USD, etc.).

The method takes the base and target currencies as input and returns the corresponding exchange rate.

If no exchange rate is available for the provided currency pair, the method returns -1 to indicate an error.


Step 4: Perform Conversion

The program checks if a valid exchange rate is returned by the getExchangeRate method.

If valid, the conversion is performed by multiplying the input amount by the exchange rate.


Step 5: Display Result

The result is displayed in a formatted message, showing the original amount, base currency, converted amount, and target currency.

If no valid exchange rate is found, an error message is displayed.



---

2. Key Components

a. Input Handling

The Scanner class is used to take inputs from the user (currencies and amount).

Inputs are sanitized by converting them to uppercase for consistent comparison.


b. Exchange Rate Handling

Hardcoded exchange rates are defined in the getExchangeRate method.

This method uses conditional statements (if-else) to determine the exchange rate based on the base and target currencies.


c. Conversion Logic

The conversion formula is straightforward:


\text{Converted Amount} = \text{Amount} \times \text{Exchange Rate}

d. Output Formatting

The printf method is used for formatted output, ensuring the converted amount is displayed with two decimal places.



---

3. Example Run

Case 1: Valid Conversion

Input:

Base Currency: USD
Target Currency: INR
Amount: 100

Output:

100.00 USD is equal to 8275.00 INR


Case 2: Invalid Currency Pair

Input:

Base Currency: INR
Target Currency: GBP
Amount: 100

Output:

Conversion rate not available for the selected currencies.



---

4. Enhancements

This program can be further improved by:

1. Dynamic Exchange Rates: Fetching real-time rates from an API like OpenExchangeRates or Forex APIs.


2. Support for More Currencies: Adding more currency pairs to the getExchangeRate method.


3. Error Handling: Adding validations for invalid inputs (e.g., non-numeric amounts).


4. User Interface: Creating a graphical user interface (GUI) for better user interaction.




---

5. Learning Objectives

By implementing this program, one can:

Understand how to use conditional statements and methods in Java.

Learn about handling user inputs with the Scanner class.

Gain familiarity with basic arithmetic operations and formatted output in Java.


