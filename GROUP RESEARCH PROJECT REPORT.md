# Group Research Project Report

## Team Members:
1. hamid
2. Behrad Khamenehmohammadi 
3. ... 
4. ... 
5. ... 

## Declaration
... 

## Introduction
hi how are you?

## Methodology

### Survey Design

The survey was designed to get a view of public perceptions of electric cars across three generations, focusing on Generation Z. This research aimed to provide actionable insights for the marketing department in an automotive company in order to better align strategies with consumer attitudes and preferences.

To ensure a comprehensive understanding of the generations’ opinion, the survey included a variety of question types:
- **Likert Scale Questions**: These questions measured for example respondents' attitudes toward electric cars on a scale from 1 (strongly disagree) to 5 (strongly agree), which was one of our survey’s key primer data sources. They addressed topics such as environmental impact, affordability, and technological appeal. This format enabled us to identify trends and subtle differences in perception across demographic groups.
- **Multiple-Choice Questions**: These questions explored factors influencing respondents’ likelihood of purchasing an electric car. Options included cost, charging infrastructure, maintenance, and brand reputation, allowing participants to select multiple factors that shaped their decisions.
- **Yes/No Questions**: Simple binary questions provided direct insights into specific perceptions, such as whether respondents viewed electric cars as practical or believed they were affordable.
- **Open-Ended Questions**: To complement quantitative data too, participants were offered to share additional thoughts, suggestions, or concerns in their own words. These qualitative responses offered additional insights to our team.

The survey was designed to be short and easily understandable, requiring only 5–10 minutes to complete.

The final survey can be accessed through this link: https://docs.google.com/forms/d/1Xb3nvls27Mth0lLDyDlT7EFrK2yDOdNp9GOzV6Fl1Go/edit

---

### Sampling Method

Our sample consisted of 72 respondents, evenly distributed across three age groups: Generation Z (12–27 years), Millennials (28–43 years), and a group named "Others" (44+ years). This segmentation allowed for meaningful comparisons of generational differences in attitudes toward electric cars.

Participants were selected using a **convenience sampling** approach. The survey link was distributed through social media platforms, email, chat messages and university networks. While this method ensured time- and cost-effective data collection, it also had limitations, such as potential biases in demographic representation, but the even distribution across age groups helped us mitigate this limitation, allowing for balanced generational analysis.

The final results of the survey can be accessed through this link: https://docs.google.com/spreadsheets/d/1GyM7JHhVxcj0OoRC747jSfet3JVdP77eJH2KR-wtbiI/edit?gid=341420139#gid=341420139

---

### Data Collection Process

The survey was conducted online using **Google Forms**, a tool chosen for its user-friendliness and compatibility with various devices. The form remained open for approximately one week, giving respondents flexibility to participate at their convenience. This approach allowed for rapid and efficient data collection.

When closing the survey, the raw data was exported in **CSV format** for further analysis. The dataset was cleaned by us to ensure accuracy and consistency. This involved only a few steps, such as removing incomplete responses, eliminating duplicates.

Data analysis was conducted using **Python**, with a particular focus on the **Seaborn library** for creating visualizations. Descriptive statistics, like mean scores were calculated to summarize responses. Additionally, bar charts and other visual tools were used to illustrate differences in perception across age groups. Open-ended responses were manually reviewed.

## Results
##Data Format and Structure:
The survey responses are stored in a CSV file, which includes:
1. **Demographics:**
Age group and gender.
2. **Perceptions and Attitudes:**
Responses to questions about general perception of electric cars, likelihood to purchase, and perceived importance for climate change.
3. **Behavioral Insights:** Questions related to past experiences with electric cars, such as whether respondents have driven or been a passenger in one.

#Steps to Achieve the Analysis
To address the objective, we'll go through the following steps in the project:
1.   **Setup and Data Loading:** We’ll start by setting up the environment with necessary libraries and loading the CSV data to ensure everything is ready for analysis.
2.   **Data Cleaning and Preprocessing:**
Here, we’ll examine the dataset for issues like missing values, inconsistent formatting, and extra whitespace in column names. This step ensures our data is clean and standardized for accurate analysis.
3. **Generation Segmentation:**
We’ll create a new column to categorize respondents into generational groups (e.g., Generation Z, Millennials) based on their age group. This segmentation allows us to make generational comparisons.
4. **Extracting Relevant Data for Analysis:**
We’ll select only the relevant columns related to perception and attitudes for analysis. Dropping irrelevant columns helps to focus on key information.
5. **Data Transformation for Quantitative Analysis:**
Certain survey responses (e.g., "Yes" or "No" answers) will be converted into numerical values to allow statistical comparisons.
6. **Calculating Averages by Generation:**
For each generation, we’ll calculate average values for perception scores and likelihood to consider buying an electric car. This step provides numerical insights into how perceptions differ among generations.
7. **Visualization of Results:**
Finally, we’ll visualize the differences in perception and attitudes across generations using bar charts. This step will clearly display trends and help answer the initial research question.
8. **Conclusion and Interpretation:**
Based on the visualizations and calculated metrics, we’ll interpret the findings to determine if Generation Z has a more positive perception of electric cars.
#Step 1: Setting Up the Environment and Importing Data
In this step, we’ll import the necessary libraries for data analysis and visualization. This is essential because each library has a specific role in handling and visualizing our data:

pandas: Used for loading, cleaning, and manipulating our survey data.
seaborn: Allows us to create clear and aesthetically pleasing visualizations.
matplotlib.pyplot: Provides additional customization options for our plots.
#Step 2: Data Cleaning and Preprocessing
In this step, we’ll clean up the data by removing any extra spaces from column names. This ensures consistency when referring to columns in our code, especially if some columns have leading or trailing spaces. We’ll also quickly review the column names to make sure they’re what we expect.
#Step 3: Generation Segmentation
In this step, we’ll categorize respondents into generational groups (such as Generation Z and Millennials) based on their age group. This segmentation will help us compare the perceptions of electric cars across different generations.
#Step 4: Extracting Relevant Data for Analysis
In this step, we’ll select only the columns relevant to our analysis, focusing on the generational group, perception of electric cars, likelihood of purchasing in the next 5 years, and belief in their importance for climate change. This allows us to concentrate on the data needed for answering our research question.
#Step 5: Data Transformation for Quantitative Analysis
In this step, we’ll convert specific responses, like "Yes" and "No," to numerical values. This conversion will allow us to calculate meaningful averages for each generation, making it easier to compare their beliefs quantitatively.
#Step 6: Calculating Averages by Generation
In this step, we’ll calculate the average perception scores and likelihood to consider purchasing electric cars for each generation. This gives us a summary view of how each generation perceives electric cars and their interest in them.
Based on the results, Generation Z has a generally positive perception of electric cars, with an average score of 2.33 for overall perception and 2.71 for the likelihood of purchasing one in the next five years. This score is slightly lower than that of Millennials, whose perception and likelihood scores are 2.54 and 2.54, respectively. Interestingly, the Other age group has the highest likelihood score of 3.07, suggesting stronger interest in purchasing electric cars, though this group’s general perception of electric cars (2.60) is similar to the other generations.

Regarding the belief in electric cars' importance for climate change, Millennials hold the strongest conviction, with a score of 0.79, indicating that nearly 80% of this group sees electric cars as essential for addressing climate issues. Generation Z also shows a high level of support (0.71 or 71%), while the Other age group demonstrates more skepticism, with a lower score of 0.47 (47%). These results indicate that Millennials and Generation Z generally see electric cars as beneficial, particularly for environmental efforts, while the Other age group may have more varied views on their impact.
#Step 7: Visualization of Results
In this step, we’ll create bar charts to visually compare how each generation perceives electric cars. Visualizations help us see trends and differences more clearly than numerical tables, making it easier to interpret the findings.
## Discussion
... 

## Conclusion
... 

## Reflection
... 

## References
Link to our survey: https://docs.google.com/forms/d/1Xb3nvls27Mth0lLDyDlT7EFrK2yDOdNp9GOzV6Fl1Go/edit
We did not use any references, just like with the presentation, we used what we learned in class.
