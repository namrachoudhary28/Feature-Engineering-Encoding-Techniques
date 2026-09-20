# Feature Engineering - Encoding Techniques

This repo shows how I converted categorical data into numerical format for Machine Learning models.

### Dataset Used: Loan Dataset

#### 1. Label Encoding
- **Columns:** Languages (Python, SQL, Excel, etc.)
- Converted text labels into numbers like 0, 1, 2
- Used for: Binary / low-cardinality data where order doesn't matter much
- Tool: `sklearn.preprocessing.LabelEncoder`

#### 2. One Hot Encoding
- **Columns:** Gender, Married
- Created separate binary columns (0/1) to avoid giving false ranking to categories
- Used for: Nominal data
- Tool: `sklearn.preprocessing.OneHotEncoder`

#### 3. Ordinal Encoding - 1
- **Column:** Size (Small, Medium, Large)
- Applied custom order: Small < Medium < Large
- Used for: Data where rank matters

#### 4. Ordinal Encoding - 2
- **Column:** Property_Area (Rural, Semi-Urban, Urban)
- Applied custom order: Rural < Semi-Urban < Urban

**Tech Stack:** Python, Pandas, Scikit-Learn
