# Blockchain_InvestigationREADme 

I would like to welcome you to my Blockchain Research, and I hope you find my content useful. Feel free to drop a comment if you need any help for me to explain or if there are any issues with the code. 
Without further ado, in this GitHub repository contains all my research which I have documented down. I recommend reading the “Technical Documentation” first as I’ve gone into a deeper detail of explain my work; two of the import pages are the “Technical Architecture” and “ERD” for you to get a overall understanding of how things flow.  
All the “Notebook*.py” are Notebooks that I used in Microsoft Fabric to extract and transform my data. Once the data has been filtered & transformed to meet my requirements, I saved the data to their corresponding tables; simultaneously I created a email function to send the data to the specified recipients. 

 
Description of what each NoteBook Does: 


{Notebook: Hourly Price Live/ Email for BTC/ETH/XRP}-Email Alerting  
In this code I've created a requests function to extract the specified CRYTPOs: Current Price,Hourly Price Change. After this has been extracted the data is updated within the table. This table is updated very hour. 
This allows you to understand the HOURLY PRICE CHANGE of each crypto-currency. 
In addition, I collected extra data (this is not saved to the table) and also created a email format to send the data (along with the extra data collected) to the recipients within the table dbo_Email_Names (table in fabric containing Email and corresponding names) 

{Notebook: All Time High Data}  
In this code I've created a requests function to extract the specified CRYTPOs: All Time High Price, Date (which that all time high price was). After this has been extracted the data is updated within the table. This table is updated every day. 
This allows you to understand all the ALL-TIME HIGHS of each crypto currency. 

{Notebook: Daily HIGH/LOW Price}  
In this code I've created a requests function to extract the specified CRYTPOs: Daily High Price, Daily Low Price, Date. After this has been extracted the data is inserted within the table. This table is updated every day. 
This allows you to understand all the HIGHEST AND LOWEST price of each crypto-currency it was on that DAY 

{Notebook: Daily Price History} 
In this code I've created a requests function to extract the specified CRYTPOs: Current Price, Date. After this has been extracted the data is inserted within the table. This table is updated every day. 
This allows you to understand the DAILY PRICE HISTORY of each crypto currency. 
 
{Notebook: Daily Price Live} 
In this code I've created a requests function to extract the specified CRYTPOs: Current Price,Daily Price Change. After this has been extracted the data is updated within the table. This table is updated every day. 
This allows you to understand the DAILY PRICE CHANGE of each crypto-currency since the last updated on 12:00 DAY BEFORE.  

{Notebook: Hourly Price History} 
In this code I've created a requests function to extract the specified CRYTPOs: Current Hour Price, Current Time. After this has been extracted the data is inserted within the table. This table is updated every hour. 
This allows you to understand the HOURLY PRICE  of each crypto-currency every hour. 
 
{Notebook: Top 3 Gainers email} 
In this code I've created a requests function to gather the top 3 crypto current "Gainers" for the day and then use this information to construct a email. Once this email is created it is sent to the following recipients within dbo_Email_Names 
