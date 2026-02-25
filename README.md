# Weather-dashboard
🌦️ API-Based Weather Dashboard (Power BI)
📖 Detailed Project Explanation

This project demonstrates how external API data can be integrated into Power BI to build a dynamic and reusable weather analytics dashboard.
Instead of relying on static datasets, the dashboard pulls live weather data at refresh time, making it suitable for real-world reporting scenarios.

The project is intentionally built using a Power BI Template (.pbit) file to:

Protect sensitive information (API keys)

Allow easy reuse by other users

Separate logic from credentials

🔄 Why API-Based Data Matters

Most beginner dashboards use CSV or Excel files.
This project focuses on API consumption, which is closer to how production BI systems work.

Benefits:

🌐 Real-time or near real-time data

🔁 Automatic updates on refresh

📉 No manual file maintenance

🧠 Stronger data engineering skills

🧰 Technical Stack (Explained)
🟡 Power BI

Used as the main BI platform for:

Data modeling

DAX calculations

Dashboard creation

User interaction

🔄 Power Query (ETL Layer)

Power Query acts as the ETL engine:

Extract

Uses the Web connector to call the weather API endpoint

Sends parameters such as:

City / location

Measurement units (metric)

Transform

Parses the JSON response

Expands nested records and lists

Filters unnecessary attributes

Renames fields for clarity

Converts data types correctly (number, text, datetime)

Load

Loads clean, structured tables into the Power BI data model

This mirrors real-world data pipelines where raw API responses must be shaped before analysis.

📐 DAX (Analytics Layer)

DAX is used to convert raw data into meaningful insights.

Examples of what DAX handles:

Aggregations (Average, Min, Max)

KPI calculations

Context-aware metrics

Dynamic values that respond to filters

DAX ensures:

Accurate calculations across visuals

Performance-efficient reporting

Business-ready metrics instead of raw numbers

📊 Dashboard Design Logic

The dashboard is designed with decision-making in mind, not just visuals.

KPI Cards

Used to highlight:

🌡️ Current / Average Temperature

💧 Humidity Level

🌬️ Wind Speed

These provide at-a-glance insights.

Charts & Visuals

Trend visuals show how weather metrics vary

Comparisons allow quick pattern recognition

Layout avoids clutter and focuses on clarity

Every visual is backed by a DAX measure to ensure consistency.

📂 Why .pbit Instead of .pbix?

Using a Power BI Template file is a deliberate design choice.

Advantages:

🔐 API key is not stored

📦 File is shareable on GitHub

🔁 Users can reuse logic with their own credentials

🧪 Safer for public repositories

When opening the file, Power BI prompts the user to enter:

API key

Location (if parameterized)

🚀 Step-by-Step Usage Flow (Expanded)

1️⃣ Open the .pbit file in Power BI Desktop
2️⃣ Enter required API parameters
3️⃣ Power Query executes the API request
4️⃣ JSON response is transformed into tables
5️⃣ Data model refreshes
6️⃣ DAX measures recalculate
7️⃣ Dashboard updates automatically

This flow mimics enterprise BI refresh cycles.

🎯 Skills Demonstrated

This project validates hands-on ability in:

API integration (not mock data)

Data transformation logic

Analytical thinking with DAX

Dashboard usability principles

Secure sharing of BI assets

🔮 Possible Extensions (Realistic)

These are technically feasible, not hypothetical:

⏱️ Scheduled refresh via Power BI Service

📅 Historical weather storage using incremental refresh

🌍 Multi-location comparison using parameters

🗺️ Geographic visuals with map layers

🧠 Who This Project Is For

Aspiring Data Analysts

Power BI developers learning APIs

BI portfolios that need real-world relevance

Recruiters evaluating applied BI skills
