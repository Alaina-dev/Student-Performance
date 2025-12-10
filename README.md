# Student-Performance
This exercise focuses on cleaning, exploring, analysing, and visualising a student dataset using Python and the pandas library. The project demonstrates a complete beginner-friendly data workflow, starting from loading raw data, identifying data quality issues, correcting them, answering analysis questions, saving a cleaned dataset, and finally producing basic visualisations.
## Tools and technologies
This project is completed using Python as the main programming language. The primary library used for data manipulation and analysis is pandas. Data visualisation is created using matplotlib. The project is developed and executed in Google Colab, with files stored and accessed through Google Drive.
## Dataset description
The dataset used in this exercise is [student.csv](student.csv). It contains student-level information including id, name,class,mark,gender. The raw dataset includes several common real-world data quality issues such as missing values, inconsistent categorical labels, duplicated records, and incorrect data types. These issues make the dataset unsuitable for direct analysis without proper cleaning and preparation.
## Data cleaning and Output
The data cleaning process begins with loading the raw dataset into a pandas DataFrame and inspecting its structure using functions such as `head()`, `info()`, and `describe()`. Missing values are identified using `isna()` and handled using appropriate methods such as replacing with statistical values or marking as unknown where applicable. Duplicate records are detected and removed to avoid double counting during analysis.
Data types are checked and corrected, particularly for numeric columns that may have been stored as text. Categorical values such as gender and class names are standardised by correcting spelling mistakes, removing extra spaces, and unifying letter casing to ensure consistency across the dataset. After completing all cleaning steps, the dataset is validated again to confirm that it is free of errors and ready for analysis.

After cleaning, the dataset is saved as a new file named [Students_data_cleaned.csv](Students_data_cleaned.csv). This cleaned file serves as the final, reliable version of the data for data nanlysis later. 
## Data analysis and output 
The student.csv dataset was loaded into a pandas DataFrame and explored using the first five rows, dataset information, and summary statistics to understand its structure, data types, and overall mark distribution.
Basic indexing and slicing were used to select individual columns, multiple columns, the first few rows, and to filter students belonging to Class Four.

For data manipulation, a passed column was created based on whether a student’s mark was greater than or equal to 60, the mark column was renamed to score, and the temporary passed column was later removed. Aggregation techniques were applied to calculate the average mark by class, the number of students in each class, and the average mark by gender.

Advanced operations included creating a pivot table showing marks by class and gender, generating a new grade column based on score ranges, and sorting the dataset by mark in descending order. Finally, the updated dataset containing the new grade column was exported to a new CSV file [new student performance.csv](new student performance.csv). Simple visualisations was created to display class distribution.
## How to run the project
To run this project, upload the student.csv file to your Google Drive and mount Google Drive in Google Colab. Load the dataset using pandas, follow the cleaning steps in the notebook,the cleaned dataset will be automatically saved back to Google Drive as a new excel file after execution. Run the analysis and visualisation cells in order,a new dataset will be automatically saved back to Google Drive as a new CSV file. All visualisations will be displayed directly in the notebook output.
## Key learning outcomes
This project develops essential data analysis skills including loading datasets, inspecting data structure, identifying data quality problems, handling missing values, removing duplicates, standardising categorical values, correcting data types, exporting cleaned data, and producing basic data visualisations. It also reinforces the importance of following a structured data analysis workflow used in real-world data projects.
## Author and attribution
This project was created by the author as a hands-on Python data cleaning and visualisation exercise for learning and practice purposes. The dataset is used for educational demonstration only.
