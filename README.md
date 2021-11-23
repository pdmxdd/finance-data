# Repository of Scripts related to finances

## Data Collection: Historical

Credit Card Statements
  - Discover
  - Chase
  - UsBank

Checking Statements
  - UsBank

Savings Statements
  - Discover

## Data Collection: Ongoing

- script that checks emails for Transaction alerts from credit cards

## Data Transformation

- all expense records should look the same
- all profit records should look the same

### Expenses

- Account Type (credit, checking, savings)
- Account Name (Discover, UsBank, Chase)
- timestamp (yyyy/mm/dd:hh:mm:ss)
- amount (float)
- vendor (string)
- description (string, couple of sentences)
- categorized (true/false)
- locked (true/false)
- id (hash of timestamp+amount+vendor)

# Deliverable(s)

1. [ ] Bash script that converts PDFs to plain text files
2. [ ] Python module that writes expense data (see above) to CSV file
  - must be tested
3. [ ] python module that extracts expense data (see above) from plain text file
  - must be tested
  - module may contain submodules for each type of account (see above) as each statement will probably be a little different
4. [ ] python script that takes command line arguments of text file to read and csv file to write to
  - script uses modules mentioned in previous two steps to extract and write 

This all results in one CSV file that contains all of the historical expense data associated with the three credit cards.
