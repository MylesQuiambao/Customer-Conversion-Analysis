# Customer-Conversion-Analysis
Conducted thorough data cleaning and analysis using Excel to uncover patterns between casual users and members. Findings support a data-driven marketing campaign proposal for executive approval.

# Abstract
As a junior data analyst at Cyclistic, a bike-share company in Chicago, my role is to support the marketing team in maximizing annual memberships. Through data analysis, I investigated the usage patterns of casual riders and annual members to devise a strategy for converting casual users into members. Utilizing Cyclistic's internal data, I conducted thorough data cleaning and analysis, leveraging pivot tables and visualizations to highlight key insights. I discovered that casual users typically use the service for leisure and errands, while members predominantly commute. Key findings suggest targeting casual users with promotions during high-usage months (June-August) and on weekends (Saturdays, Sundays, Mondays) to optimize conversion efforts. These insights will guide the development of a data-driven marketing campaign aimed at boosting membership and securing approval from Cyclistic executives.

# Step 1: Ask
The business task is to utilize the data provided to create meaningful insight and pleasing yet sensible and easy-to-understand visualizations. I would need to determine the difference on how casual users use the service compared to annual members so that the marketing may be able to come up with a plan on how to convert the casual users into members since annual members bring in more revenue for the company.

# Step 2: Prepare
For my analysis, I will be using Cyclistics' internal data which has been maintained and organized by its data engineers. The data was downloaded here. (Note: The datasets have a different name because Cyclistic is a fictional company. For this case study, the datasets are appropriate and will enable you to answer the business questions. The data has been made available by Motivate International Inc. under this license.)
I've downloaded the data and given the limited capability of Excel to handle large amounts of data, I only took a reasonable 10% randomized sample size for each month of the year 2023 from the total data at my disposal to avoid data bias using Python. I've practiced clear naming conventions for the files to maintain a proper structure and organization of files. Since the data is from a first-person party, this would indicate that the data is reliable, original, comprehensive, current, and cited.

# Step 3: Process
I've chosen Excel since I believe it would suffice when it comes to the analysis and visualization phases of my entire process. Since the data has been maintained by the company's data engineers, barely any cleaning was needed for my analysis but as best practice, I've checked for any errors. <br/>

  • Checked for duplicates.<br/>
  • Trimmed any whitespace that could be found.<br/>
  • Checked the filters on each field to check for format inconsistencies or typos.<br/>
  • Removed fields that would be unnecessary for my analysis.<br/>
     - start_station_name, start_station_id, end_station_name, end_station_id, start_lat, start_long, end_lat, end_long.<br/>
  • Referenced start_time and end_time (Fields that contain the Date and Time of the start and end of the ride) <br/>
      to add new columns to separate the time of the ride for easier analysis.<br/>
  • Extracted started_ at to create columns for month, month_text, and day_of_the_week.<br/>
  • Subtracted start_time from end_time to create a column for ride_length.<br/>
  • Extracted hour from start_time to create a new column for start_time_hour.<br/>
  • Applied proper capitalization formatting on values for member_casual and rideable_type fields.<br/>
