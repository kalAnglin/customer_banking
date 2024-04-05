# Customer_Banking 

I worked with a LA on AskBSC-307244 and tutor Mohammed Fauwaaz in a Tutor Session on BCS to complete this assignment.

## Overview

Create a customer banking system utilizing modularity of functions as a block of resuable code that allows the users to calculate and track interest earned on a savings and CD accounts based on the user's starting balance, interest rate, and account maturity.

## Purpose
By running this application, user will be able to enter their savings and CD account information, see the interest earned, and view updated balances after a specified number of months.

## Business Advantage

### Savings Account [^1]

![Savings Account Benefit](https://github.com/kalAnglin/customer_banking/blob/main/images/savings_account.jpeg)

- This program is designed to illustrate the following benefits to the users by calcutating and updating balance after a specific number of months:
1. Earn a Return: Although savings accounts typically do not yield a big return it is a steady and reliable one. The APY national average according to the FDIC is .59% which is still bigger return than just stashing cash.[^2] 
2. Small Initial Investment: Another benefit is in comparison to other investments, such a real estate & mutual investments, most savings accounts have a very low minimum balance, if any. In other words, you are guaranteed some type of return regardless of the deposit amount.

### CD Account [^3]

![CD Benefit](https://github.com/kalAnglin/customer_banking/blob/main/images/CD_account.jpeg)

- By providing the user with an application to calculate and track the interest earned on a cd account, the user is presented with the following benefits:
1. The APY national average for a one-year CD is 1.73% which almost three times the APY for CD.[^4] If setting money for large future purchase is in the cards, CD provides a good way to keep funds in a safe place and earn interest.
2. CD Attributes: If there is a concern regarding the inability to withdraw from a CD, there are options. Some CDs allow users to withdraw with no penalities. Terms of a CD also impact the interest rate, typically longer CDs have higher rates than shorter ones; however some CDs do allow a bump-up or rate increase during the term.

## Landscape

This customer banking program fits right into the current financial landscape geared around creating a personal finance strategy, which typically involves earning some interest at minimal risk. High-yield savings accounts are a great option with some online-only banks offering an APY of 5.35%. As mentioned there is less flexibility to withdraw from a traditional CD account within the term period, but CD ladder is another alternative. CD ladders provide the opportunity to open multiple CDs with staggering maturity dates, which provides access to portions of money at regular monthly intervals. The customer application is specifically beneficial in this scenario by helping the user determine the CD term length and corresponding interval access based on the interest that would be earned.[^5]

## Results

### Importing Class & Creating Functions

Account class from account.py file was separately imported into the savings and cd account functions, which allowed an instance of the account class to be created and the balance and interest parameters passed to the account class in each individual function. The interest earned was calculated (balance * interest_rate/100 * months/12) and assigned to a variable and the account balance was updated by adding the interest earned to the balance and then assigning it to a variable in eaach individual function. The updated balance was passed to the set balance using the instance of the account class and the update balance and interest earned were returned by the respective function.

### Create Main Function

The savings and cd account functions were imported to into the main fuction. User input statments were created to prompt the user to set the balance, interate rate, and months for the savings and cd account. The main function was called to the run the customer_banking application which utilized the savings and cd account funtions to print out the interest earned and corresponding increase in the savings and cd account balance to two decimal places and thousandths based on the initial balance and APY variables the user entered.

## Recommendations

### Savings Account APY & CD Term Period

- For the purpose of making this application more plausible or realistic, it may be helpful to limit the user input in regards to APY for savings account so it resembles the national average. Similary, a more plausible application of the progam would be to have the APY vary based on the CD term period.


[^1]: https://www.usnews.com/banking/articles/benefits-of-having-a-savings-account
[^2]: https://www.bankrate.com/banking/savings/average-savings-interest-rates/
[^3]: https://www.nerdwallet.com/article/banking/cd-certificate-of-deposit
[^4]: https://www.bankrate.com/banking/cds/cd-rates/
[^5]: https://www.bankrate.com/banking/savings/low-risk-ways-to-earn-higher-interest/

