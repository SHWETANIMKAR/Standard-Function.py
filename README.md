# Standard Functions in Pandas

This project explores standard statistical functions in Pandas using a Hospital Patient dataset.

### Dataset
Patient data with columns: Patient_ID, Age, Gender, Department, City, Treatment_Cost, Hospital_Stay
Cities: Nagpur, Pune, Mumbai

### What I learned

1. Statistical Functions
- df["Age"].mean() - Average age = 43.3
- df["Age"].std() - Shows how spread out the age values are
- df["Treatment_Cost"].mean() - Average cost = 50000
- df["Treatment_Cost"].std() - Variation in treatment cost
- df[Department=="Cardiology"]["Age"].std() - Variation for specific department

2. Handling Missing Values
- df.isnull() & df.isnull().sum() - To find and count missing values
- df.dropna() - Remove rows with missing data
- df.dropna(subset=["Age"]) - Remove rows where only Age is missing
- df["Age"].fillna(40) - Fill missing with fixed value
- df["Age"].fillna(df["Age"].mean()) - Fill missing with mean value (44.75)

### Tech Used
- Python
- Pandas
- Jupyter Notebook

This is part of my Day 9 Pandas learning journey.
