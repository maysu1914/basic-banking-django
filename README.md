# basic-banking-django
Basic banking project with basic money transaction feature

# Quick Start
1. pip install -r requirements.txt
2. python manage.py makemigrations
3. python manage.py migrate
4. python manage.py runserver

- (Optional) python manage.py loaddata customers
- (Optional) python manage.py createsuperuser (for admin page)
- (Optional) python manage.py test

# Usage
## Endpoints
GET				'api/customers/':
Listing all customers, their accounts, and transactions of accounts

GET	'api/customer/<int:pk>':
Details of customer

POST			'api/customer/':
Create new customer

GET				'api/accounts/':
Listing all accounts

GET 'api/account/<int:pk>':
Details of account

POST			'api/account/':
Create new Account

GET				'api/transactions/':
Listing all transactions

GET 'api/transaction/<int:pk>':
Details of transaction

POST			'api/transaction/':
Create new transaction

## Models
Customer:
Name

Account:
Customer (FK),
Deposit (Default 500)

Transaction:
Account from (FK),
Account to (FK),
Amount