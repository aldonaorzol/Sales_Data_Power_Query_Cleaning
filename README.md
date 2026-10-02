# Sales_Data_Power_Query_Cleaning

Table:
- order_ID,
- date,
- category,
- sales_channel,
- amount_zl,

Data cleaning:

Excel:
1. Parsing Delimited Data -> Data -> Text to columns -> Comma
2. ctrl+t ->Create table
3. Importing data into Power Query -> Get Data from Table/Range

Power Query:
1. Uploading a CSV file so that Polish characters are read correctly, e.g. OdzieĹĽ, ogrĂłd
New Source -> File -> Text/CSV

Before:

<img width="834" height="590" alt="image" src="https://github.com/user-attachments/assets/49f62102-aadb-432d-b026-065538b3eba8" />

After:

<img width="830" height="582" alt="image" src="https://github.com/user-attachments/assets/7aa5dfe6-c5ce-44a6-a045-e68b0bf23760" />



2. Normalization of numeric value formats:

Transform -> Replace Values -> from a dot to a comma

The data type in the 'amount_zl' column was changed to 'Currency'.

<img width="160" height="542" alt="image" src="https://github.com/user-attachments/assets/5f3e0764-4727-4679-beec-c851e0bf16a3" />

3. This table shows that the data contains no duplicate orders, errors, or NULL values.

<img width="829" height="162" alt="image" src="https://github.com/user-attachments/assets/e84cc731-c60d-41b0-9d5f-6d5f3525680b" />

4. Replace Values -> translate values from polish to english

<img width="702" height="307" alt="image" src="https://github.com/user-attachments/assets/11c5d77f-2159-4e39-83af-0fd6afd4ec79" />

5.  Close & Apply
