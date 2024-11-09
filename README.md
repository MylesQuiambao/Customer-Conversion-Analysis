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

# Step 4: Analyze
For my analysis, I've used pivot tables to aggregate the data, which is organized in a separate worksheet. <br/>

  • Ride Count: Members have a 56% higher total ride count than casual users (Members: 366,668; Casual: 205,319). <br/>
  • Average Ride Length: Casual riders have a higher average ride length by 2 minutes and 33 seconds (Members: 8m22s; Casual: 10m55s). <br/>
  • Rides Per Day of Week: Members consistently ride more than casual users, peaking at 58,879 on Wednesdays. Casual riders peak on Saturdays at 41,048, still less than members' 47,341 on the same day. <br/>
  • Ride Length by Day of Week: Members' average ride length is relatively stable, varying only by 1m50s from Monday (8m50s) to Friday (7m). Casual riders show a more noticeable downtrend from 13m41s on Monday to 6m31s on Friday, then spike to 10m16s on Saturday and peak at 16m04s on Sunday. <br/>
  • Rides Per Hour: Members' rides peak at 24,184 at 8:00 AM and 38,936 at 5:00 PM. Casual riders peak at 20,078 at 5:00 PM. <br/>
  • Top Months for Rides: For members, the top months are June (41,975), July (43,735), and August (46,136). For casual users, the same months are top with 29,987, 33,030, and 31,033 rides, respectively. <br/>

  # Step 5: Share
After creating visualizations from the aggregated data in my analysis stage, I will then share these with my team before I present them to key stakeholders so that I may gather insight and critique. <br/>

Here's what I learned throughout my data analysis:

![image](https://github.com/user-attachments/assets/5430d281-9a44-49eb-b28a-74949a19ff62) <br/>
Casual riders have a higher average ride length by 2 minutes and 33 seconds
