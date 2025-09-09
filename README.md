# Expense Tracker CLI

This is a simple command-line tool for tracking your expenses. It's built with Python and uses a SQLite database to store your expense data.

## Project Overview

The Expense Tracker CLI is a lightweight and easy-to-use tool for managing your personal finances from the command line. It allows you to add new expenses, view a summary of your spending, and filter expenses by category.

This project is designed for developers who are comfortable with the command line and prefer a minimalist approach to expense tracking.

## Features

*   **Add expenses:** Quickly add new expenses with an amount, category, and an optional message.
*   **View expenses:** Get a summary of all your expenses or filter them by a specific category.
*   **Simple data storage:** Uses a local SQLite database to store your data, so you don't need to rely on a third-party service.
*   **Command-line interface:** All operations are performed through a simple and intuitive command-line interface.

## Technologies Used

*   **Language:** Python
*   **Libraries:**
    *   [docopt](https://github.com/docopt/docopt): For parsing command-line arguments.
    *   [tabulate](https://github.com/astanin/python-tabulate): For formatting the output in a clean, tabular format.
    *   [pyinstaller](https://www.pyinstaller.org/): For packaging the application into a standalone executable (optional).

## Installation and Setup

To get this project running on your local machine, follow these simple steps:

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/init050/Expense_Program.git
    cd Expense_Program
    ```

2.  **Create a virtual environment and activate it:**
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```

3.  **Install the dependencies:**
    ```bash
    pip install docopt tabulate
    ```

4.  **Initialize the database:**
    Before you can start adding expenses, you need to create the database and table.
    ```bash
    python spent_app.py --init
    ```

## How to Use

Here are the commands for interacting with the expense tracker:

*   **Add a new expense:**
    ```bash
    python spent_app.py --add <amount> <category> [<message>]
    ```
    *Example:*
    ```bash
    python spent_app.py --add 50.00 "Groceries" "Weekly grocery shopping"
    ```

*   **Show all expenses:**
    ```bash
    python spent_app.py --show
    ```

*   **Show expenses by category:**
    ```bash
    python spent_app.py --show <category>
    ```
    *Example:*
    ```bash
    python spent_app.py --show "Groceries"
    ```

## Future Improvements

*   **Edit and delete expenses:** Add commands for editing and deleting existing expenses.
*   **Date filtering:** Allow users to filter expenses by a specific date range.
*   **Data visualization:** Add a feature to generate simple charts and graphs to visualize spending habits.
*   **Configuration file:** Use a configuration file to manage database settings and other preferences.
