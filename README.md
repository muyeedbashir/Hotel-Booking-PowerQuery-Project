# 🏨 Hotel Booking Data Cleaning & Transformation using Power Query

---

## 📌 Project Overview

This project focuses on cleaning and transforming raw hotel booking datasets using **Microsoft Excel Power Query**.

The objective was to convert unstructured booking and room datasets into an analysis-ready format by applying multiple preprocessing techniques commonly used in real-world data analytics workflows.

---

## 🛠 Tools Used

- Microsoft Excel
- Power Query Editor
- CSV Files

---

## 📂 Dataset Used

The following raw datasets were used in this project:

- [bookings_data.csv](https://github.com/muyeedbashir/Hotel-Booking-PowerQuery-Project/blob/main/bookings_data.csv)
- [rooms_data.csv](https://github.com/muyeedbashir/Hotel-Booking-PowerQuery-Project/blob/main/rooms_data.csv)

---

## 🔍 Data Cleaning & Transformation Steps

### ✔ Step 1: Imported CSV Files

Loaded both raw datasets into Excel using the **From Text/CSV** option and opened them in Power Query Editor.

---

### ✔ Step 2: Changed `property_id` Data Type

Converted the `property_id` column from Number format to Text format for consistency.

---

### ✔ Step 3: Standardized Property Names

Replaced inconsistent entries:

`Atliq bay` → `Atliq Bay`

---

### ✔ Step 4: Cleaned `property_type`

Removed unnecessary leading and trailing spaces using **Trim Transformation**.

---

### ✔ Step 5: Split `city|city_code`

Separated the combined city and city code column into:

- `city`
- `city_code`

---

### ✔ Step 6: Created `Availability Status`

Conditional logic applied:

- `successful_bookings = capacity` → Sold Out
- Else → Vacant

---

### ✔ Step 7: Created `occ%` Column

Calculated occupancy ratio using:

`successful_bookings / capacity`

Converted the result into percentage format.

---

### ✔ Step 8: Merged Two Tables

Merged the following datasets using `room_id`:

- `bookings_data`
- `rooms_data`

Added the `room_class` column into the main booking table and reordered columns accordingly.

---

### ✔ Step 9: Extracted `month_name`

Derived month names from the `date` column to prepare the dataset for monthly trend analysis.

---

## 📈 Key Skills Demonstrated

- Data Cleaning
- Data Transformation
- Merge Queries / Joins
- Conditional Columns
- Custom Columns
- Occupancy Calculations
- Date Extraction
- Query Editing

---

## 📸 Project Screenshots

### Raw Dataset Preview
![Raw Dataset](https://github.com/muyeedbashir/Hotel-Booking-PowerQuery-Project/blob/main/Raw%20dataset.png)

---

### Power Query Applied Transformations
![Power Query Steps](https://github.com/muyeedbashir/Hotel-Booking-PowerQuery-Project/blob/main/power%20query%20editor.png)

---

### Final Cleaned Output
![Final Output](https://github.com/muyeedbashir/Hotel-Booking-PowerQuery-Project/blob/main/Final%20cleaned%20output.png)

---

## 📁 Project Files

- [Cleaned Excel Output](https://github.com/muyeedbashir/Hotel-Booking-PowerQuery-Project/blob/main/hotel_booking_cleaned.xlsx.xlsx)

---

## 🚀 Final Outcome

Successfully transformed raw hotel booking data into a clean, structured, and analysis-ready dataset that can be directly used for:

- Occupancy Analysis
- Booking Trend Monitoring
- Room Utilization Reporting
- Dashboard Building

---

## 💼 Business Understanding

This project reflects one of the most common real-world responsibilities of a data analyst:

> transforming messy operational business data into reliable decision-ready information.
