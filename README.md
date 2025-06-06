🏦 Bank Statement Project
📘 Project Overview
This project simulates a basic banking system using Python. It models a bank account that allows users to:

Debit an amount

Credit an amount

Check the account balance

The functionality is implemented through an object-oriented approach using classes.

🛠️ Technologies Used
Python 3

Jupyter Notebook

📂 Project Structure
account Class
Method	Description
__init__	Initializes the account with balance and number
debit()	Deducts amount from account balance
credit()	Adds amount to account balance
get_bal()	Returns current balance

✅ Example Usage
python
Copy
Edit
class account:
    def __init__(self, balance, account_no):
        self.balance = balance
        self.account_no = account_no

    def debit(self, amount):
        self.balance -= amount
        print("Rs", amount, "is debited from your account")
        print("Total balance = ", self.get_bal())

    def credit(self, amount):
        self.balance += amount
        print("Rs", amount, "is credited in your account")
        print("Total balance = ", self.get_bal())

    def get_bal(self):
        return self.balance

# Create and use an account
account1 = account(12500, 11225588)
account1.debit(12000)

🔍 Possible Enhancements
Add transaction history tracking
Implement overdraft limits
Export statements to a CSV or PDF
GUI using Tkinter or Web UI with Flask

