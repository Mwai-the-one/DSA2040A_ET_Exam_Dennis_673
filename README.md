Education Data Analysis — California School Dataset\

This project performs data extraction, transformation, and analysis on a dataset containing information about schools across California counties.
The analysis focuses on racial composition, grade-level distribution, and school types per county using Python, Pandas, and SQLite.

🧠 Project Overview\

The dataset (raw_data.csv) contains detailed information about schools, including:

Academic year and school identifiers

County and district details

Enrollment by race and grade

School characteristics (type, level, funding, etc.)

This project automates the following steps:

Extract — Load raw CSV data into Python.

Transform — Clean and prepare data (handle missing values, create date fields).

Load (ETL) — Store processed data in a SQLite database and extract the most recent academic year.

Analyze — Generate descriptive insights and visualizations.

🧩 Technologies Used\
Tool	Purpose
Python 3.13	Core programming language
Pandas	Data manipulation and analysis
SQLite3	Lightweight database for queries
Matplotlib / Seaborn	Data visualization
NumPy	Numerical operations
Datetime	Handling date and time formats

🗂️ Project Structure\
ET_Exam_Dennis_Mwai_673/
│
├── raw_data.csv
├── raw_data.db
├── incremental_data.csv
├── incremental_data.db
├── data_analysis.py      ← (This script)
└── README.md             ← (You are here)

⚙️ How It Works
1️⃣ Data Extraction
Reads the dataset from CSV.
Displays the first few rows and column names for inspection.

2️⃣ Data Transformation
Checks for missing values (dataset has none).
Creates a new date column using the academic year.

3️⃣ Data Loading to SQLite
Establishes a SQLite connection.
Saves the full dataset to a local database.
Extracting the Latest Academic Year
Retrieves the most recent year’s records.
Exports the result to both .csv and .db formats.

📈 Insights Generated
Analysis	Output	Key Takeaway
Racial Makeup	Bar chart	Shows racial diversity per county
Grade Distribution	Pie chart	Reveals grade-level enrollment patterns
School Type	Grouped bar chart	Highlights how school types vary by county
