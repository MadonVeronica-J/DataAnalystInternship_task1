# DataAnalystInternship_task1
## Data Cleaning and Preprocessing
Dataset used : Customer Personality Analysis
Source : Kaggle
Tools : Google Colab / Python(pandas)

### Reading the dataset:
-The dataset is read using pandas and different columns are saved under single column. Thus the columns were seperated using split function.

### Checking for null values:
-The dataset is checked for null value and no null values were found.

### Checking for duplicates:
-The dataset is chencked for the duplicated in the ID column and also the entire dataset and no duplicates were found.

### Standardizing text values:
-Education and Marital_Status columns were checked for unique values.  <br> 
-In Marital_Status column values such as 'YOLO', 'Absurd', and 'Alone' were present which was the standardized to 'Single'.

### Renaming column headers to be uniform:
-Column headers were renamed such that it has no whitespaces and consistent capitalization.

### Fixing Data Types:
-Every column had object data type, thus, it was converted to Int64 and datetime respectively.

### Dropping columns that are not needed for analysis:
-Column id serves no purpose in analysis and thus it is dropped.  <br> 
-year_birth column which mentions which year the customer is born is converted to age column so that it would better represent which age group prefers certain item.  <br>
-dt_customer column which tells us the day when the customer enrolled is converted to customer_since_days column to find how long the person has been a customer as this would help find the long term trend
