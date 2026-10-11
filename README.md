==============================================================
STOCK PORTFOLIO TRACKER
==============================================================
A simple console Python program that calculates your
stock portfolio's total value using manually defined prices.

Project: Python Programming Internship (CodeAlpha) - Task 2
Author : Gireeshwarareddy
File  : stock_portfolio_tracker.py
--------------------------------------------------------------

ABOUT THE PROJECT
--------------------------------------------------------------
The user inputs which stocks they have and how many shares of a
stock they own. Each stock's price is manually defined in a

hardcoded dictionary and used to calculate the value of each
holdings, with an overall summary of the investment's total
value displayed. The results may optionally be saved to a file.
No internet connection or additional libraries are needed.
--------------------------------------------------------------
STOCKS AVAILABLE
--------------------------------------------------------------

The program contains 10 stocks with example prices (in USD):
AAPL  333.69
TSLA  370.59
GOOGL  343.50
MSFT  517.53
AMZN  251.52
LLY  1142.85
META  728.08
AVGO  355.14
NVDA  233.95
NFLX   67.06
--------------------------------------------------------------
FEATURES
--------------------------------------------------------------
- Hardcoded dictionary of stock prices (decimal values supported)
- Supports multiple stocks and quantities in one run
- Case-insensitive input (aapl, AAPL and Aapl all work)
- Rejects input stocks that are not in the price list
- Rejects invalid quantity of shares (letters, zero, negative numbers)
- Adds quantities of the same stock entered twice
- Displays a per stock breakdown and the total value of the investment
- Optionally saves the summary to a .txt file
--------------------------------------------------------------
CONCEPTS USED
--------------------------------------------------------------
- Dictionaries
- input() and print()
- Basic arithmetic
- while loops and if/else
- Functions
- Exception handling (try/except)
- File handling (open, write)
- f-string formatting
--------------------------------------------------------------
REQUIREMENTS
--------------------------------------------------------------
- Python 3.8 or newer
- No additional libraries
--------------------------------------------------------------
HOW TO RUN
--------------------------------------------------------------
1. Keep the file task-2.py in a folder
2. Open a terminal / command prompt in that folder
3. Run:
python stock_portfolio_tracker.py
(On some systems use: python3 stock_portfolio_tracker.py)
--------------------------------------------------------------
HOW TO USE
--------------------------------------------------------------
1. The program lists the available stocks and their prices
2. Type a stock symbol (e.g. AAPL) and press Enter
3. Type in the quantity of shares you own and press Enter
4. Repeat as many times as you want to add stocks
5. Type 'done' when you have finished
6. The summary and total are displayed
7. Choose 'y' to save the summary to a file, or 'n' to skip
--------------------------------------------------------------
SAMPLE RUN
--------------------------------------------------------------
Welcome to the Stock Portfolio Tracker!
Available stocks and their prices:
AAPL  $333.69
TSLA  $370.59
GOOGL $343.5
MSFT  $517.53
AMZN  $251.52
LLY  $1142.85
META  $728.08
AVGO  $355.14
NVDA  $233.95
NFLX  $67.06
Enter stock symbol (or 'done' to finish): aapl
Enter quantity of AAPL: 10
Added 10.0 share(s) of AAPL.
Enter stock symbol (or 'done' to finish): tsla
Enter quantity of TSLA: 5
Added 5.0 share(s) of TSLA.
Enter stock symbol (or 'done' to finish): done
========================================
PORTFOLIO SUMMARY
========================================
AAPL   10.0 shares x $333.69 = $3,336.90
TSLA   5.0 shares x $370.59 = $1,852.95
----------------------------------------
TOTAL INVESTMENT       $5,189.85
========================================
Save this summary to a file? (y/n): y
Enter filename (e.g. portfolio.txt): portfolio.txt
Saved! Check the file 'portfolio.txt' in your project folder.
--------------------------------------------------------------
PROJECT STRUCTURE
--------------------------------------------------------------
stock_portfolio_tracker.py    Main program
README.txt    Project documentation
portfolio.txt  Output file (created only if you save)
--------------------------------------------------------------
CODE OVERVIEW
--------------------------------------------------------------
show_available_stocks() Prints the stock list with prices
get_quantity(symbol)   Asks for a valid quantity (loops until valid)
build_portfolio()    Collects stock + quantity pairs from the user
calculate_total()    Computes each holding's value and the total
print_summary()     Displays the formatted summary
save_to_file()      Optionally writes the summary to a file
main()          Runs the program from start to finish
--------------------------------------------------------------
CHANGING THE STOCK PRICES
--------------------------------------------------------------
Open stock_portfolio_tracker.py and edit the stock_prices dictionary at the top
of the file. Keep the symbols in UPPERCASE:
stock_prices = {
"AAPL": 333.69,
"TSLA": 370.59,
"XYZ": 100.00   <- add new stocks like this
}
--------------------------------------------------------------
POSSIBLE IMPROVEMENTS
--------------------------------------------------------------
- Save the output as a .csv file as well
- Use whole-number shares only (float to int)
- Load prices from a file (not hardcoded)
- Add a feature to remove or edit an entered stock
- Fetch prices from an API (advanced)
--------------------------------------------------------------
NOTE
--------------------------------------------------------------
The prices used in this project are fixed example values and do
not represent live market prices. This program is for learning
purposes only and is not financial advice.