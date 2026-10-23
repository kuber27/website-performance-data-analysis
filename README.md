# Website Performance Data Analysis

## Project Overview

This project explores website performance data using Python to understand user behavior, traffic patterns, engagement metrics, and acquisition channel performance.

The analysis focuses on identifying traffic trends over time, comparing website acquisition channels, examining user engagement, and understanding how website activity varies throughout the day.

The project demonstrates practical applications of data cleaning, exploratory data analysis (EDA), data aggregation, and visualization.

## Objectives

* Analyze website traffic and user activity over time.
* Examine the relationship between users and sessions.
* Compare traffic across different acquisition channels.
* Identify channels with higher average engagement time.
* Compare engaged and non-engaged sessions by channel.
* Investigate hourly traffic patterns.
* Present findings through clear and interpretable visualizations.

## Tools and Technologies

* **Python** — Data analysis and processing.
* **Pandas** — Data cleaning, transformation, grouping, and aggregation.
* **NumPy** — Numerical operations.
* **Matplotlib** — Data visualization.
* **Seaborn** — Statistical visualization and heatmaps.
* **Jupyter Notebook** — Interactive analysis and documentation.

## Dataset

The project uses website analytics data containing metrics such as:

| Column                              | Description                                    |
| ----------------------------------- | ---------------------------------------------- |
| Channel Group                       | Traffic acquisition channel                    |
| DateHour                            | Date and hour associated with the observation  |
| Users                               | Number of users                                |
| Sessions                            | Number of sessions                             |
| Engaged sessions                    | Sessions meeting the engagement criteria       |
| Average engagement time per session | Average time users actively engage per session |
| Engaged sessions per user           | Engagement-related ratio                       |
| Events per session                  | Average number of events per session           |
| Engagement rate                     | Proportion of sessions classified as engaged   |
| Event count                         | Total recorded events                          |

The dataset contains hourly observations from April–May 2024, covering multiple acquisition channels.

## Data Preparation

The following data preparation steps were performed:

1. Imported the dataset using Pandas.
2. Corrected the column names using the first row of the dataset.
3. Removed the original header row from the data.
4. Converted the `DateHour` column into a datetime format.
5. Converted analytical metrics into appropriate numeric data types.
6. Extracted the hour from the datetime column.
7. Examined data types and descriptive statistics.

## Exploratory Data Analysis

### 1. Website Traffic Over Time

Analyzed user and session activity over time using line charts to examine fluctuations in website traffic.

### 2. Acquisition Channel Analysis

Compared the total number of users across acquisition channels, including:

* Direct
* Email
* Organic Search
* Organic Social
* Organic Video
* Referral
* Unassigned

### 3. Average Engagement by Channel

Calculated average engagement time per session for each acquisition channel to compare how users interact with the website.

### 4. Engaged vs. Non-Engaged Sessions

Compared engaged sessions with non-engaged sessions across acquisition channels using grouped bar charts.

### 5. Hourly Traffic Analysis

Created a heatmap to examine how traffic varies by hour and acquisition channel.

### 6. Engagement Rate and Sessions Over Time

Visualized engagement rate and session trends over time to explore changes in website activity and user engagement.

## Key Observations

Based on the visualizations generated in the notebook:

* Organic Social contributes the largest total user volume among the displayed acquisition channels.
* Organic Video has the highest average engagement time per session in the channel comparison.
* Direct traffic has more non-engaged sessions than engaged sessions in the aggregate comparison.
* Organic Social and Referral show higher engaged-session totals than non-engaged-session totals.
* Hourly traffic patterns vary by acquisition channel, with substantial differences in activity throughout the day.

These observations are descriptive and reflect the displayed dataset. Further statistical analysis would be needed to establish causes or determine whether the patterns generalize beyond this period.

## Visualizations

The notebook includes:

* Website sessions and users over time.
* Total users by acquisition channel.
* Average engagement time by channel.
* Engaged versus non-engaged sessions.
* Hourly traffic heatmap by acquisition channel.
* Engagement rate and sessions over time.

Screenshots can be added to a `screenshots/` directory and embedded in this section.

Example:

```markdown
![Traffic by Hour and Channel](screenshots/traffic_heatmap.png)
```

## Project Structure

```text
website-performance-data-analysis/
│
├── Website Data Analysis.ipynb
├── data/
│   └── data-export.csv
├── screenshots/
│   ├── traffic_heatmap.png
│   ├── channel_users.png
│   ├── engagement_by_channel.png
│   └── sessions_over_time.png
├── README.md
└── requirements.txt
```

The structure is illustrative. Include only the files and directories that actually exist in your repository.

## How to Run the Project

### 1. Clone the repository

```bash
git clone https://github.com/YOUR-USERNAME/website-performance-data-analysis.git
```

### 2. Navigate to the project directory

```bash
cd website-performance-data-analysis
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Launch Jupyter Notebook

```bash
jupyter notebook
```

Open `Website Data Analysis.ipynb` and run the cells.

Ensure the dataset is stored in the expected location or update the CSV path in the notebook.

## Skills Demonstrated

* Data cleaning and preprocessing
* Exploratory Data Analysis (EDA)
* Datetime conversion and feature extraction
* GroupBy operations and aggregation
* Descriptive statistics
* Time-series visualization
* Comparative channel analysis
* Heatmap visualization
* Data interpretation and analytical communication

## Future Improvements

* Add a statistical analysis of channel-level engagement rates.
* Investigate daily and weekly traffic patterns.
* Build an interactive dashboard using Plotly or Streamlit.
* Add automated data-quality checks.
* Explore relationships between traffic volume and engagement.
* Develop a predictive model for website traffic forecasting.

## Author

**Kuber Singh**

Aspiring Data Analyst | Data Science Student

Interested in data analytics, Python, SQL, statistical analysis, and machine learning.

---

If you find this project useful, feel free to explore the notebook and share feedback.
