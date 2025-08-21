# DDS--personal-financial-tracker

Personal-Finance-Tracker

🔹 Project Overview

This system helps users manage their personal finances by:

Recording income & expenses as transactions.

Tracking savings goals.

Allowing search, filter, and sort on transactions.

Storing data persistently using file handling.

Displaying an ASCII bar chart for monthly spending (bonus feature).

🔹 Features in Detail

Transaction Management
Each transaction stored in a structure:

struct Transaction { int id; char type[10]; // "Income" or "Expense" char category[30]; float amount; char date[15]; // e.g. "2025-08-19" };

Stored in an array of structures.

Sorting, Searching, Filtering
Sort transactions by date, amount, or category.

Search by category (e.g., "Food").

Filter (e.g., expenses > $100).

Savings Goal Tracking
User sets a monthly savings goal.

Program compares income - expenses with the goal.

Displays progress (met/not met).

File Handling
Save transactions to a file (finance.txt).

Load transactions when the program starts.

ASCII Bar Chart (Bonus)
For each month, print total spending in bar form. Example:

Jan: ####### ($700) Feb: ### ($300) Mar: ########## ($1000)

(# = $100)

🔹 How to Run

Compile the program:

g++ finance_tracker.cpp -o finance_tracker
