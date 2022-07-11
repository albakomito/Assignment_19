# Assignment 19
Assignment 19 


## Step 1 (fintech_finder.py, ln 34-183)
In this section  we Import Ethereum Transaction Functions from crypto_wallet.py into our fintech_finder.py file. Specifically, we: 
* Import the `generate_account`,  `get_balance`, and send_transaction` functions (alongside w3). 
* Use the candidate information provided as part of the starter code (we'll creating a folder in our repo named 'Images' from which our code will pull the different candidates' profile pictures). 
* The candidate information consists of a candidate database (a dictionary with nested lists), a list of candidate names, and the 'get_people' function that displays the candidate information (consisting of their names, Ethereum account addresses, their 'Fintech Finder' rating, and hourly rate). 
* Prepare the streamlit application and sidebar headers. 
* Create a variable account that calls the 'generate_account' function (ln 131-134).
* Write the client's Ethereum account address to the sidebar (ln 135-140). 
* Define a new `st.sidebar.write` function that will display the balance of the customer’s account (ln 141-152). 
* Populate the sidebar as follows (ln 153-183): 
  * Create a select box to choose a FinTech Hire candidate. 
  * Create a input field to record the number of hours the candidate worked. 
  * Identify the FinTech Hire candidate. 
  * Write the Fintech Finder candidate's name to the sidebar.
  * Identify the FinTech Finder candidate's hourly rate. 
  * Write the inTech Finder candidate's hourly rate to the sidebar. 
  * Identify the FinTech Finder candidate's Ethereum Address. 
  * Write the Fintech Finder candidate's Ethereum Address to the sidebar. 
  * Write the Fintech Finder candidate's name to the sidebar

## Step 2 (fintech_finder.py, ln 184-287)
In this sections we sign and execute a payment transaction. Specifically, we: 
* Write the equation that calculates the candidate’s wage, by defining the 'wage' variable as the product of hours and the list item `candidate_database[person][3]`. 
* Write the `wage` calculation to the Streamlit sidebar
* Call the `send_transaction` function and pass into it w3, account, candidate address and the wage variable. 
* Note: in the 'send_transaction` function, we create an if statement within our sidebar that will: 
   * Create a markdown 'Validated Transaction Hash' for our transaction hash. 
   * Write the returned transaction hash to the screen. 
   * Celebrate our successful payment with balloons in streamlit. 
* Use the get_people() function (given to us in the starter code that writes Fintech Finder candidates in our Streamlit User Interface. 

## Step 3 (fintech_finder.py, ln 288- 321) 
We inspect the transaction by: 
* Sending a test transaction by using the application’s web interface, and then looking up the resulting transaction hash in Ganache.
* My account address, balance and TX count can be found below: 


* A screenshot of one of my transactions with the candidate can be found below: 

