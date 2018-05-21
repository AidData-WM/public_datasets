###Using Data in a GIS
AidData has developed Introduction to GIS Training Modules for QGIS (which is free and open source). This training is oriented towards new users of spatial information with the purpose of improving understanding and ability to use spatial information. The instructional tutorial will help users to join spatial information with other data, calculate new variables, and create cartographic outputs.  
QGIS Training Module: https://github.com/AidData-WM/public_datasets/raw/master/documentation/QGIS%20Tutorial%20Final.zip   

###Using Data in Spreadsheets  
Microsoft Excel has known limitations when working with TSV and CSV files that have character encodings like UTF8 (the character encoding of the AidData CSV Data). To avoid potential problems with character encodings, please use the “From Text” command on the Data menu when opening the CSV files. Double-clicking on the files to open in Excel or saving them as CSV from Excel may result in character encoding problems.  
For instructions, see this link: http://bit.ly/18hp7pL  

Additionally, AidData provides all final tabular data as comma separated files. If asked by your software which delimiter to use, you should select comma. PLEASE BE CAREFUL TO ONLY USE ONE DELIMITER (not for example, comma and TAB).  

The five (5) files in the research release are related as follows:  
1) The projects.csv table is the main table. It contains one row per project. The unique id is the project_id field.  
2) The locations.csv table is the locations table. It contains one row per location. It is related to the projects table by the project_id field. Each project may have many locations. The unique id is the project_location_id field.  
3) The transactions.csv table is the transactions (financials) table. It contains one row per transaction. It is related to the projects table by the project_id fields in each table. Each project may have many transactions. The unique id is the transaction_id field.  
4) The ancillary.csv table contains all ancillary data for the projects table. It contains any ancillary data for the project table. It is related to the projects table by the project_id fields in each table. There is no unique field for the ancillary table.  
5) The locations_ancillary.csv table contains all project locations for which secodary sources were used for their confirmation or addition. It can be related to the locations table via the project_location_id field. It is also the unique id for this table.
