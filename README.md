  # ![GA Logo](https://camo.githubusercontent.com/6ce15b81c1f06d716d753a61f5db22375fa684da/68747470733a2f2f67612d646173682e73332e616d617a6f6e6177732e636f6d2f70726f64756374696f6e2f6173736574732f6c6f676f2d39663838616536633963333837313639306533333238306663663535376633332e706e67) Exploring Titanic

---

_Author: Dodge McIntosh_

---

In class up until this project, we had been learning all about Pandas and plotting. At this point I was chomping at the bit to get my hands dirty on a real-world dataset.

For this project, I took a depp look at the Titanic manifest. I explored this data to see what can be learned regarding the survival rates of different groups of people.

## Brief Overview of the Workflow:
> - Reading in the data
  - Cleaning the data
  - Basic feature extraction
  - Exploratory analysis
  - Visualizing findings

## Step 1: Reading the data

1. Data drawn from [https://www.kaggle.com/c/titanic/data](https://www.kaggle.com/c/titanic/data)
2. An available data dictionary explains each of the columns. It's important to get familiarized with how the csv is structured.
4. Downloaded the `train.csv` file into this project repo
3. Created an iPython notebook and read the csv in using pandas.

## Step 2: Cleaning the data
> - Searched for and dealt with null values
  - Searched for any discrepancies with data types and dealt with them

## Step 3: Feature extraction
1.  There are two columns that pertain to how many family members are on the boat for a given person. Created a new column called `FamilyCount` which is the sum of those two columns.
3. In order to feed the training data into a classification algorithm, I needed to convert the categories into 1's and 0's using `pd.get_dummies`
  - Created 3 columns: `Embarked_C`, `Embarked_Q` and `Embarked_S`. These columns have 1's and 0's that correspond to the `C`, `Q` and `S` values in the `Embarked` column
  - Did the same thing for `Sex`

## Step 4: Exploratory analysis
- Asking all of the important questions to see what factors influenced survival rates on the Titanic.
- **Most importantly**, would **_I_** have survived?! (Spoiler alert: not even close).

## Step 5: Visualizing findings
Using Matplotlib and Seaborn, I created several charts showing the survival rates of different groups of people. A handful of the charts are basic (Gender, Age, etc), but I really tried looking for something beneath the surface.

## Project Feedback + Evaluation

For this project, I wanted to make sure I was adhering to the following principles throughout:

- **Organization**:	Clearly commented, annotated and sectioned Jupyter notebook.  Comments and annotations add clarity, explanation and intent to the work.  Notebook is well-structured with title, author and sections. Assumptions are stated and justified.
- **Data Structures**: Python data structures including lists, dictionaries and imported structures (e.g. DataFrames), are created and used correctly. The appropriate data structures are used in context. Data structures are created and accessed using appropriate mechanisms such as comprehensions, slices, filters and copies.
- **Python Syntax and Control Flow**:	Python code is written correctly and follows standard style guidelines and best practices. There are no runtime errors. The code is expressive while being reasonably concise.
- **Charting**: Charts (from Pandas, Matplotlib, and Seaborn) are created and used correctly. The appropriate charts are used in context. Charts are created and accessed using appropriate mechanisms.
