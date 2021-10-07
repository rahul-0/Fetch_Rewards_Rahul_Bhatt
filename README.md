# Fetch_Rewards_Rahul_Bhatt
Repo consisting answers and explanations to the Assessment Project for Fetch Rewards.

**Data Quality Issues:** 
As a part of the first steps of understanding the dataset. I loaded the JSON file in Notepad++ and on observing the file, I found that the JSON had a dictionary inside of a dictionary and that was an invalid format and due to which parsing the file was the first Data Quaity problem I noticed.
This posed as an issue, but I resolved it by loading the JSON files in Microsoft Power BI, which had an automatic AI based backend processor which understood and auto-corrected this issue of invalid format.
I found the Date field to be in an invalid format.
There were a lot of incomplete and Null data fields.
The Dimension Table(Users) that I used as a part of the Data Modelling Task had multiple duplicates whereas it should have been unique.
When joining the Receipt and Brand Tables as a part of my modelling, I found out that there were mulitple barcodes that were not assigned to any product and vice versa as well.
The Barcode in the Recepits table posseses Product Level Information which should be in Brands table. It is not normalised.
After processing the JSON in Power BI, I was saving them as CSV in Excel, where I noticed that Receipt Number was not unique and I observed repeating Receipt numbers.
To further improve upon my processing, I removed rewards based information from receipts as it was adding redundancy to the data and I added it to the Brand table for better processing.
