# credit_card_app
Project Topic
The Luhn Algorithm for validating credit card numbers is used. Write a code that determines whether a credit card number entered by the user is correct or not.

Luhn Algorithm:

First, write the 16 digits of a credit card number with spaces in between. Underline the first digit. Then, skip one and do the same for the other digits. Next, multiply all the underlined digits by 2. For example, let's say our card number is
4 4 3 7 1 2 1 4 5 6 1 8 9 1 7 3. When we take double of the marked numbers, we get
8 6 2 2 10 2 18 14.

Now, add up all the numbers. During this process, if your number is two digits, you should add the digits separately. For instance, instead of 18, think of it as 1+8. In this case, our sum would be 8+6+2+2+1+0+2+1+8+1+4+4+7+2+4+6+8+1+3 = 70. If 70 is divisible by 10, it indicates that the card is valid and no mistakes were made. If a mistake had been made, it wouldn't be evenly divisible by 10.

American Express cards only have 15 digits. In this case, we need to adjust our calculation slightly. In our card number, we'll start by marking the second digit from the left and continue marking every other digit. The process continues the same way. For example, if our card number is 3 7 8 2 8 2 2 4 6 3 1 0 0 0 5.

Sum of marked numbers: (1 + 4) + 4 + 4 + 8 + 6 + 0 + 0 = 27
Sum of unmarked numbers: 3 + 8 + 8 + 2 + 6 + 1 + 0 + 5 = 33.

The sum of the two sets of numbers is 60, which is also a multiple of 10. This is another indicator that no mistake was made. Let's provide one more example. This time, it includes a Diners Club card. These cards have 14 digits and start with 300 or 305. For example, our number is 3 0 5 6 9 3 0 9 0 2 5 9 0 4. Since the number is even (14), we will apply the same technique as with the 16-digit card. We start from the beginning, skip one, mark the numbers, take double, and sum the resulting digits. If you follow the process, you will reach the number 50, which indicates that the entered card number is correct.

Method:

Ask the user for a credit card number.
If the credit card number is 16 digits, validate it as Visa/Mastercard; if it's 15 digits, validate it as American Express; otherwise, give an error.
Provide the program's output as "The credit card you entered is a valid American Express card" or "The credit card you entered is invalid."
You can test your program with the card numbers on the following website: https://docs.adyen.com/development-resources/testing/test-card-numbers
Ensure clean code and adhere to the DRY (Don't Repeat Yourself) principles in your programming.
Please note that this explanation is provided in Turkish, as requested.


