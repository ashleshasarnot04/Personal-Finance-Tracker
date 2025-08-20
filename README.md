# Personal-Finance-Tracker

Project Overview

The system assists users in handling their personal  financial data through the following features:

The system tracks user income together with their expense transactions.

The system  enables users to track their savings objectives.

The system enables users to find transactions through search functions and process them  with filter functions and sorting options.

The system keeps data stored permanently through file-handling techniques.

The  system shows monthly spending through an ASCII bar chart as an additional feature.

 Features in Detail

1. Transaction Management

Every recorded transaction exists inside a structure named:

struct Transaction {

    int id;
    char type[10];   // "Income" or "Expense"
    char category[30]; 
    float amount;
    char date[15];   // e.g. "2025-08-19"

};

The transactions exist as an array of structures.

2. Sorting, Searching,  Filtering

Users can arrange transactions according to date sequence and amount size and category grouping.

Users can  search through the transactions by selecting categories such as "Food".

Users can filter their expenses by selecting  criteria such as amounts exceeding $100.

3. Savings Goal Tracking

Users establish their monthly savings objectives  through the system.

The program evaluates the difference between income and expenses in relation to the savings goal.

The system shows users whether they have reached their savings goal or not.

4. File Handling

Users  can save their financial transactions in the file named finance.txt.

The system retrieves financial transactions from storage during  program initialization.

5. ASCII Bar Chart (Bonus)

The system displays monthly spending totals with bar charts  which represent the amount spent. Example:

Jan: ####### ($700)

Feb:  ### ($300)

Mar: ########## ($1000)

(#
