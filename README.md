
🚀 Amazon Sales Analysis Power BI Dashboard 
📈Welcome to the Power BI project repository focusing on a comprehensive Sales Analysis of Amazon Products.
This solution showcases the complete data workflow—from data cleaning and modeling to advanced DAX usage and dynamic visualization.
The final dashboard is designed to be dynamic and interactive.

🎯 Key Performance Indicators (KPIs)
Four essential measurable quantities (KPIs) were required to provide a high-level view of how the business is performing, including total sales and quantity sold.
Note that the creation of a Date Table using DAX was mandatory for these Time Intelligence calculations to function correctly.

📅💰 Year to Date (YTD) Sales
This major metric measures the overall revenue performance for the current, latest year available in the dataset (for example, 2022).
It is calculated using the TOTALYTD DAX function.

📉📈 Quarter to Date (QTD) Sales
This tracks sales trends and performance within the latest quarter, comparing it against previous quarters.

📦🛒 YTD Products Sold
This represents the total number of products sold on the Amazon platform within the current year.
This calculation uses the TOTALYTD function applied to the COUNT of a clean, reliable field like Product Category.

⭐ YTD Reviews / Feedback
Calculates the total number of feedback entries received.
This is crucial for gauging the product satisfaction rating and is calculated using TOTALYTD combined with the SUM of the 'Number of Reviews'.

📊 Visualization Requirements
The dashboard features various charts designed to provide detailed insights by diving into the granularity of the data.

🗓️ Sales by Month
A Line or Area Chart visualization used to identify monthly sales patterns and seasonal peaks.
Analysis showed high sales volumes in September, October, November, and December, often linked to festive seasons.

📅 Sales by Week
Implemented as a Column Distribution Chart to analyze short-term sales performance within the month or week.

🗂️🔥 Sales by Category
A Matrix Chart (which can also be viewed as a Text Map or Heat Map) is used to compare sales performance across diverse product categories such as Menswear, Shoes, Audio/Video, and Sports against various measures like YTD Sales and QTD Sales.
Conditional Formatting with gradient colors is applied to highlight high and low values within the matrix.

🏆 Top Five Products by YTD Sales
A Horizontal Bar Chart designed to spotlight the five highest-performing products based on their Year-to-Date revenue.

👍 Top Five Products by YTD Reviews
A Horizontal Bar Chart identifying the five products that have received the maximum number of positive feedback or reviews.

🔎 Interactive Elements
To allow users to view the data from different angles, the dashboard includes key filters (slicers).

🛍️ Product Category Filter
Allows filtering by categories like cameras, shoes, or car accessories.

🗓️ Quarter Filter
Allows the analysis of specific performance periods such as Quarters 1 and 4.
This required creating a custom 'Quarter' field using DAX functions like QUARTER and CONCATENATE to display labels like "QTR 1".

🛠️ Technical Implementation & Skills
The project leverages several key tools and advanced Power BI concepts.

🧰 Tools Used
Power BI (Version June 2023 was used, but the latest version is always recommended)
MS Office Excel (Version 2016 or later) used for initial data storage and manipulation.

⚙️ Core Concepts

🧼 Data Quality and Cleaning
Data was imported and checked in the Power Query Editor.
Crucial fields like Date and Price were verified to ensure they were 100% valid with 0% errors or blanks.

🔗 Data Modeling
A dedicated Date Table (Calendar Table) was created using DAX functions such as CALENDAR, MIN, and MAX.
This is necessary for all Time Intelligence functionality.

🔄 Relationship Establishment
A One-to-Many (1:*) relationship was established between the Date Table (Primary Key) and the Amazon Data Table (Foreign Key).
This is the recommended relationship type for connecting these two tables.

🔢 Custom Month Sorting
To ensure that the "Sales by Month" chart sorted correctly (January to December) instead of alphabetically, a 'Month Number' column was created using the MONTH DAX function to enable proper custom sorting.

🧮 DAX Usage
Extensive use of Time Intelligence functions (TOTALYTD), as well as standard functions such as SUM, COUNT, and FORMAT, was implemented for metric calculation.

📊 Data Landscape

📏 Size
The dataset comprises approximately 89,082 rows (almost 90,000 rows).

🧾 Fields
The data includes six to seven fields such as Product Category, Product Description, Price (in dollars), Number of Reviews, Ship Location (City/Country), and Order Date.

🧠 Data Study Principle
A critical best practice applied was the thumb rule that 60% to 70% of the project time should be dedicated to studying the data to fully understand its flow, hierarchy (for example, Product Category > Product > Price), and domain terminology.



