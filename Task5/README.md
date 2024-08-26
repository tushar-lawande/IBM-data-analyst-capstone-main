# Task 5 - Dashboarding

In this assignment we will continue working with the Stack Overflow Developer Survey 2019 data to create a dashboard. We will create some visualizations and add them to dashboards using IBM Cognos Analytics. In this dashboard we will create the following:

A **Current Technology Usage** tab containing in a 2x2 rectangle grid:

1. Top 10 Languages
2. Top 10 Databases
3. Platforms
4. Top 10 WebFrames

A **Future Technology Trends** tab containing in a 2x2 rectangle grid:

1. Top 10 Languages desired for the next year
2. Top 10 Databases desired for the next year
3. Desired platforms for the next year
4. Top 10 WebFrames desired for the next year

A **Demographics** tab containing in a 2x2 rectangle grid:

1. Respondent classified by gender
2. Respondent count for countries
3. Respondent count by age
4. Respondent count by gender and classified by education level

## Dataset

The dataset we are going to use in this task comes from the following source: https://stackoverflow.blog/2019/04/09/the-2019-stack-overflow-developer-survey-results-are-in/ under a ODbL: Open Database License.

We are using a modified subset of that dataset contained in the two CSV files ( m5_survey_data_demographics.csv and m5_survey_data_technologies_normalised.csv).

## Dashboard Tabs

### Current Technology Tab

On the Current Technology Usage dashboard tab, we use the data asset m5_survey_data_technologies_normalised.csv and capture the following metrics as visualizations:

- In the first rectangle (Panel 1):
  - Capture Top 10 LanguageWorkedWith.
  - Visualize as a Bar chart.
  - Utilize Bars, Length, Color fields of Bar chart.
  - Include Show value labels feature.
  - Include a proper Chart title.
- In the second rectangle (Panel 2):
  - Capture Top 10 DatabaseWorkedWith.
  - Visualize as a Column chart.
  - Utilize Bars, Length, Color fields of Column chart.
  - Include Show value labels feature.
  - Include a proper Chart title.
- In the third rectangle (Panel 3):
  - Capture PlatformWorkedWith.
  - Visualize as a Word cloud chart.
  - Utilize Words, Size, Color fields of Word cloud chart.
  - Include a proper Chart title.
- In the fourth rectangle (Panel 4):
  - Capture Top 10 WebFrameWorkedWith.
  - Visualize as a Hierarchy bubble chart.
  - Utilize Bubbles, Size, Color fields of Hierarchy bubble chart.
  - Include a proper Chart title.

### Future Technology Tab

On the Future Technology Trend dashboard tab, use the data asset m5_survey_data_technologies_normalised.csv and capture the following metrics as visualizations:

- In the first rectangle (Panel 1):
  - Capture Top 10 LanguageDesireNextYear.
  - Visualize as a Bar chart.
  - Utilize Bars, Length, Color fields of Bar chart.
  - Include Show value labels feature.
  - Include a proper Chart title.
- In the second rectangle (Panel 2):
  - Capture Top 10 DatabaseDesireNextYear.
  - Visualize as a Column chart.
  - Utilize Bars, Length, Color fields of Column chart.
  - Include Show value labels feature.
  - Include a proper Chart title.
- In the third rectangle (Panel 3):
  - capture PlatformDesireNextYear.
  - Visualize as a Tree map chart.
  - Utilize Area hierarchy, Size, Heat fields of Tree map chart.
  - Include Contrast label color feature.
  - Include a proper Chart title.
- In the fourth rectangle (Panel 4):
  - Capture Top 10 WebFrameDesireNextYear.
  - Visualize as a Hierarchy bubble chart.
  - Utilize Bubbles, Size, Color fields of Hierarchy bubble chart.
  - Include a proper Chart title.

### Demographics Technology Tab

On the Demographics dashboard tab, use the data asset m5_survey_data_demographics.csv and capture the following metrics as visualizations:

Use Filters for this tab feature to filter out entries of other types except Man and Woman from the data point Gender.

- In the first rectangle (Panel 1):
  - Capture Respondent classified by Gender.
  - Visualize as a Pie chart.
  - Utilize Segments, Size fields of Pie chart.
  - Include Dispay % feature.
  - Include a proper Chart title.
- In the second rectangle (Panel 2):
  - Capture Respondent Count for Countries.
  - Visualize as a Map chart.
  - Utilize Regions-Locations, Regions-Location color fields of Map chart.
  - Include a proper Chart title.
- In the third rectangle (Panel 3):
  - Capture Respondent Count by Age.
  - Visualize as a Line chart.
  - Utilize x-axis, y-axis fields of Line chart.
  - Include Show value labels feature.
  - Include Show markers feature.
  - Include a proper Chart title.
- In the fourth rectangle (Panel 4):
  - Capture Respondent Count by Gender, classified by Formal Education Level.
  - Visualize as a Stacked bar chart.
  - Utilize Bars, Length, Color fields of Stacked bar chart.
  - Include Show value labels feature.
  - Include a proper Chart title.
