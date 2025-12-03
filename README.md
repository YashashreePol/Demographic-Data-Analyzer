# Demographic-Data-Analyzer
A comprehensive data analysis project utilizing the Pandas library to explore demographic trends, salary, education, and work patterns within the Adult Income Dataset.
That's a vital addition for any public project\! Adding a **License section** clarifies the terms under which others can use, modify, and distribute your code. I'll also add a **Contributing section**, which is standard practice to encourage community involvement.

Here is the updated and expanded `README.md` content:

-----

# 📊 Demographic Data Analyzer

A Python project using the **Pandas library** to analyze the **Adult Income Dataset** (often derived from the U.S. Census Bureau data). This project calculates key demographic statistics related to education, race, gender, work hours, and salary.

## 🚀 Getting Started

These instructions will get you a copy of the project up and running on your local machine.

### Prerequisites

You need **Python 3** and the **Pandas library** installed.

```bash
pip install pandas
```

### Files

  * **`demographic_data_analyzer.py`**: Contains the primary Python function, `calculate_demographic_data()`, which performs all the analysis.
  * **`adult.data.csv`**: The dataset containing the demographic records. **(Ensure this file is in the same directory as the Python script.)**

### Running the Analysis

Simply run the main function from your script or an interactive Python session:

```python
import demographic_data_analyzer

# The function prints the results by default
demographic_data_analyzer.calculate_demographic_data() 
```

-----

## 🔬 Analysis Questions & Results

The `calculate_demographic_data` function generates the following statistics:

1.  **Race Count:** The number of individuals representing each unique race.
2.  **Average Age of Men:** The mean age of all male respondents, rounded to one decimal place.
3.  **Bachelors Degree Percentage:** The percentage of people in the dataset who have a Bachelor's degree.
4.  **Higher Education Wealth:** The percentage of people with advanced education (**Bachelors, Masters, or Doctorate**) who earn $>\text{50K}$.
5.  **Lower Education Wealth:** The percentage of people without advanced education who earn $>\text{50K}$.
6.  **Minimum Work Hours:** The minimum number of hours a person works per week.
7.  **Rich Percentage (Minimum Hours):** The percentage of people who work the minimum number of hours per week and earn $>\text{50K}$.
8.  **Highest Earning Country:** The country that has the highest **percentage** of people earning $>\text{50K}$.
9.  **Highest Earning Percentage:** The actual percentage of people earning $>\text{50K}$ in that country.
10. **Top Occupation in India:** The most popular occupation for those who earn $>\text{50K}$ in India.

### Example Output

```
Number of each race:
 White          27816
 Black          3124
 Asian-Pac-Islander      1039
 Amer-Indian-Eskimo      311
 Other          271
Name: race, dtype: int64
Average age of men: 39.4
Percentage with Bachelors degrees: 16.4%
Percentage with higher education that earn >50K: 46.5%
Percentage without higher education that earn >50K: 17.4%
Min work time: 1 hours/week
Percentage of rich among those who work fewest hours: 10.0%
Country with highest percentage of rich: Iran
Highest percentage of rich people in country: 41.9%
Top occupations in India: Prof-specialty
```

-----

## 💻 Key Pandas Methods Used

This project utilizes several powerful Pandas features for efficient data manipulation:

  * pd.read_csv()`**: Reads the dataset into a DataFrame.
  * .value_counts()`**: Used to count unique occurrences.
  * Boolean Indexing**: Filters data based on complex conditions.
  * .mean()` and `.min()`**: Aggregation functions.
  * .isin()`**: Checks if an element's value is present in a list.
  * .idxmax()`**: Finds the index label corresponding to the maximum value.
  * .iloc[0]` and `.index[0]`**: Retrieves the value and label of the maximum result, respectively.

-----


## 📜 License

This project is licensed under the **MIT License** - see the `LICENSE` file for details.

*(Note: You will need to create a separate file named `LICENSE` containing the full MIT License text to comply with this section.)*
