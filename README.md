<h1>Credit Card Validator</h1>

<h2>Overview</h2>

This is a C++ console application that validates credit card numbers using the **Luhn Algorithm**. It takes input from the user, checks if the card number is valid, and displays the result.
The tool is useful for understanding how checksum algorithms work in real-world systems like payment gateways and card verification processes.

<h2>Luhn Algorithm</h2>

The **Luhn Algorithm** (also known as the "modulus 10" or "mod 10" algorithm) is a checksum formula used to validate identification numbers such as credit card numbers.
1. Starting from the rightmost digit (check digit), move left and **double every second digit**.
2. If the result of doubling is a **two-digit number**, add those digits together (e.g., 8 × 2 = 16 → 1 + 6 = 7).
3. **Sum** all digits (both modified and unmodified).
4. If the total sum is divisible by **10**, the number is considered **valid**.

<h2>Usage</h2>

1. Clone this repository.
   
   <pre>git clone https://github.com/Sanidhya-pawar/Credit-Card-Validator.git</pre>

3. Compile the C++ program in C++ compiler.
   
   <pre>g++ main.cpp -o main</pre>

5. Run the program.
   
   <pre>./main</pre>

<h2>Example Output</h2>
<pre>Enter a Credit Card Number #: 4001 5900 0000 0001
4001 5900 0000 0001 is Valid

Enter a Credit Card Number #: 5267 3181 8797 5449
5267 3181 8797 5449 is Valid</pre>

<h2>Program Explanation</h2>

* The program begins by prompting the user to enter a credit card number. Typing 'exit' will terminate the program.

* It validates the input to ensure it contains only numeric digits. If the input is invalid, the user is prompted again.

* Once a valid input is received, the program applies the Luhn Algorithm to determine whether the card number is valid.

* Based on the result, it displays "Valid!" or "Invalid!" accordingly.

* This project offers a straightforward implementation of the Luhn Algorithm using C++ to validate credit card numbers.

