🏨 Hotel Booking Data Cleaning & Transformation using Power Query
📌 Project Overview

This project focuses on cleaning and transforming raw hotel booking datasets using Microsoft Excel Power Query.

The objective was to convert unstructured booking and room data into an analysis-ready dataset by applying multiple preprocessing techniques used in real-world analytics.

🛠 Tools Used

✔ Microsoft Excel
✔ Power Query Editor
✔ CSV Files

📂 Dataset Used

The following raw datasets were used in this project:

-[bookings_data.csv](https://github.com/muyeedbashir/Hotel-Booking-PowerQuery-Project/blob/main/bookings_data.csv)
-[rooms_data.csv](https://github.com/muyeedbashir/Hotel-Booking-PowerQuery-Project/blob/main/rooms_data.csv)
🔍 Data Cleaning & Transformation Steps
✔ Step 1: Imported CSV Files

Loaded both raw datasets into Excel using From Text/CSV and opened them inside Power Query Editor.

✔ Step 2: Changed property_id Data Type

Converted property_id from Number to Text format.

✔ Step 3: Standardized Property Names

Replaced inconsistent entries:

Atliq bay → Atliq Bay

✔ Step 4: Cleaned property_type

Removed leading and trailing spaces using Trim Transformation.

✔ Step 5: Split city|city_code

Separated combined city and city code column into:

city
city_code
✔ Step 6: Created Availability Status

Conditional logic applied:

successful_bookings = capacity → Sold Out
Else → Vacant
✔ Step 7: Created occ% Column

Calculated occupancy ratio using:

successful_bookings / capacity

Converted result into percentage format.

✔ Step 8: Merged Two Tables

Merged:

bookings_data
rooms_data

using room_id to add room_class.

✔ Step 9: Extracted month_name

Derived month names from the date column for monthly trend analysis.

📈 Key Skills Demonstrated

✔ Data Cleaning
✔ Data Transformation
✔ Merge Queries
✔ Conditional Columns
✔ Custom Columns
✔ Occupancy Calculation
✔ Date Transformation

📸 Project Screenshots
-[Raw data](https://github.com/muyeedbashir/Hotel-Booking-PowerQuery-Project/blob/main/Raw%20dataset.png)
-[power query editor](https://github.com/muyeedbashir/Hotel-Booking-PowerQuery-Project/blob/main/power%20query%20editor.png)
-[cleaned data](https://github.com/muyeedbashir/Hotel-Booking-PowerQuery-Project/blob/main/Final%20cleaned%20output.png)

Power Query Applied Steps

Final Cleaned Output

📁 Project Files
[Cleaned Excel Output](https://github.com/muyeedbashir/Hotel-Booking-PowerQuery-Project/blob/main/hotel_booking_cleaned.xlsx.xlsx)
🚀 Outcome

Successfully converted raw booking records into a structured dataset ready for:

Occupancy Analysis
Monthly Booking Reports
Dashboard Building
Hotel Performance Insights
💼 Analytics Insight

This project reflects one of the most important real-world data analyst responsibilities:

transforming messy operational data into decision-ready business information.
