# __EXPENSE TRACKER__

## Video Demo: <https://youtu.be/XXgztD9k4Kc>

### Description of the Project: _Expense Tracker_

Expense tracking is important for the financial health of our personal or professional budget. How about an application that does all this work for you, and you just need to feed the information? My project "Expense tracker" is a simple and user-friendly software application designed to help individuals manage their daily expenses efficiently and to analyze the expenses by storing them in a systematic tabular form.

The project provides a graphical user interface (GUI) built using the Tkinter library in Python, allowing users to easily add and view expenses in real-time. The main objective of this project is to enable users to track their spending, gain insights into their financial habits, and maintain better control over their finances. Why did I choose Tkinter? Tkinter lets you create desktop applications. It offers a variety of widgets like buttons, labels, and text boxes that make it easy to develop apps. And a GUI provides an intuitive and user-friendly design, making it easy for users to interact with the application. The input fields and buttons are well-labeled, guiding users through the expense management process.

PROCESS:

Database Connectivity: This is how I create the database. I called the "init" function for the connectivity.

- Import sqlite3
- Create a connection object, "connectionObjn = db.connect(“expenseTracker.db”)"
- Create cursor object, "curr = connectionObjn.cursor()"
- Execute required query
- Commit

I followed the above steps in every function that requires interaction with the database. Then, I need to create a table, so the query statement is written accordingly. Then, when the user enters a date of the expenditure, after that the system will store the same in dateEntry. For the name of the user and expense details like title and the amount spent are asked and stored in Title and Expense, respectively. There is a submit button that calls the SubmitExpense method.

KEY FEATURES:

1. SubmitExpense: Users can input their expenses by choosing a date (MM/DD/YY), their name (Name), expense title (Title) and amount spent (Expense) and stores it in "Etable" in a new row. It will store each of these rows in the database for future references.

1. ViewExpenses: The Expense Tracker displays all recorded expenses in a tabular format using the Treeview widget of Tkinter. It presents details such as the date, expense title, and amount. This allows users to access their recorded expenses even after closing and reopening the application.

DESIGN:

- Window App:

1. Import Tkinter
1. Import *
1. I had to create a variable to store the body of the GUI.
1. The function "root.title()" adds the title.
1. The function "mainloop()" runs the app and closes the body.
1. The function root.geometry() gives the dimensions of the app.

- LABELS: NAME, TITLE, EXPENSE

For every label I used "StringVar" which holds a string data where I can set a text value and retrieve it. For "Date", I pass the variable to textvariable parameter for the Entry widget. Then, I used the function "grid()" to position the widgets in a grid layout. I decided to use the color "DodgerBlue2" for a more friendly background.

All things considered, the Expense Tracker with Tkinter GUI is a useful tool for managing personal finances. This project helps users take greater financial control and make wise financial decisions by providing tools for tracking daily spending, creating budget objectives, and analyzing financial patterns.

Stefano Ribera,
edX: Stefano-Ribera,
GitHub: stefanoribera
