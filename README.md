# EcoScanner - Empowering value driven consumption with a simple scan of a barcode!

Forked to be added to my profile. 

Tired of misleading green packaging crowded into the aisles of Whole Foods? Too busy to read every single ingredient on a label while 
also conducting in-depth research about a company's supply chain and manufacturing practices? Enter EcoScanner, transforming a simple 
scan of a barcode into an easily understandable score from 1-10 that evaluates how environmentally-friendly any product is!


### System Components
The application has 3 components - a frontend mobile application, a backend server that exposes an API endpoint, and a database. The mobile application scans the barcode and queries the backend API with the code. The backend scrapes the web to collect data about the product and brand and calculates the EcoScore accordingly, returning this data and its components. It also uses the database to speed up the process.

<b> I was independently responsible for both the backend API and the database. </b> The files I worked on can be found on the Python branch inside the "EcoScanner" directory. The most important files are app.py (using sql), app2.py (using firebase), eco_sql_lib.py, and transfer_brands_sql.py.

### Technologies I Used
Backend:
- Flask app with Python
- nltk library for Natural Language Processing to better identify products
- urllib, requests, and BeautifulSoup for web-scraping and parsing
- Backend first hosted on Heroku (serverless solution), then transitioned to AWS EC2 micro-instance. I was responsible for all the infrastructure setup as well.

Database:
- Began with Firebase (noSQL solution), which eventually became <i> overly </i> unstructured.
- Redesigned and implemented database in PostgreSQL, communicating with python psycopg2 library
