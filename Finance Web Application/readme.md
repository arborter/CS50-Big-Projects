
This web app allows anyone who registers an account to buy stocks, sell stocks, get a quote for a stock, and view their portfolio as well as their current monies and their history of transactions. 


What the application uses:
This application utilizes Python in the backend to communicate with the server and execute commands for the GET and POST methods. The application utilizes SQLite for the database, Flask for the web framework, and HTML, CSS, as well as JINJA for the front end. I also use an API to get stock price data in real time from IEX Cloud.

I use two tables in the database: one for the users, and one for the transactions enacted by any user.



Details on the app.py file:


Register:
I created a register page where a user can create an account through a username and a password. The username and passwords are stored in the SQLite database. Moreover, the passwords are stored using the generate_password_hash() function from werkzeug, so the password is stored as a hash and hides the actual password when querying the database for passwords. 

Should the user not type anything for any text field in the HTML file, an error message will be displayed stating what the user is missing. 



Buy:
We can buy a stock. We can also check by way of executing commands to the database if the user has sufficient funds to purchase a stock. Once a stock is purchased, the database table will update for the user's transactions with information regarding the stock bought, at what price, and when.

Should the user not have sufficient funds, an error message is displayed.




Quote:

We can get a quote for any stock and find out at what price any stock sought in the text field would cost.

Should the user not type a correct symbol of the stock in the text box, an error message will be displayed. 


Index:
This is the homepage for the user once logged in. Their homepage displays the user's portfolio. The portfolio here is composed of the stocks the user owns, the available funds, and the price of each stock holding.


Sell:
A user can sell any share of his stocks. The stock sold will update the SQL table for the user's transactions and state therein that something was sold. Should the user type more shares than the user possesses, an error message will be displayed stating that the user has insufficient shares. 

History:
This window shows a list of a users transactions: what time something was sold or bought and what shares were sold or bought.

