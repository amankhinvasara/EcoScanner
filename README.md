# EcoScanner - Empowering value driven consumption with a simple scan of a barcode!

Forked to be added to my profile. 

Tired of misleading green packaging crowded into the aisles of Whole Foods? Too busy to read every single ingredient on a label while 
also conducting in-depth research about a company's supply chain and manufacturing practices? Enter EcoScanner, transforming a simple 
scan of a barcode into an easily understandable score from 1-10 that evaluates how environmentally-friendly any product is!


### Architecture
The application has 3 components - a mobile application that scans the barcode, a backend server that exposes an API endpoint, and a database.
I was indepedently responsible for both the backend API and the database. The  files I worked on can be found on the Python branch inside 
the "EcoScanner" directory. The most important files are app.py (using sql), app2.py (using firebase), eco_sql_lib.py, and transfer_brands_sql.py.
