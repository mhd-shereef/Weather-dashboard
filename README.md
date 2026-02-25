🌦️ Weather Dashboard (API-Based | Power BI)

Welcome! 👋
This dashboard shows you live weather data pulled directly from a weather API and visualized in Power BI.
You’re not looking at static files here — every refresh fetches fresh data from the internet.

This repo is meant to help you understand how API data flows into Power BI, how it’s transformed, and how insights are calculated and displayed.

🔍 What You’ll Get From This Dashboard

When you open the file, you’ll be able to:

View current weather metrics like temperature, humidity, and wind speed 🌡️💧🌬️

See clean KPIs instead of raw API responses

Interact with visuals that update automatically on refresh

Learn how real-world BI dashboards connect to external systems

🧰 Tools Used (and Why They Matter)

Power BI → For modeling, DAX, and visualization

Power Query → To connect to the API and clean the data

DAX → To calculate meaningful metrics

Weather API → Source of real-time weather information

Each tool has a specific role, just like in production BI systems.

🚀 How This Works (Step by Step)
1️⃣ Opening the File

This project uses a Power BI Template (.pbit) file.

When you open it:

Power BI will ask you for the required API details

This keeps your API key safe and not hard-coded

👉 Enter your API key and continue.

2️⃣ Fetching Data From the API 🌐

Once you proceed:

Power Query sends a web request to the weather API

The API responds with JSON data

This happens automatically — no manual downloads

You’re now working with live data, not saved files.

3️⃣ Cleaning and Shaping the Data 🔄

The raw API response isn’t user-friendly, so Power Query:

Expands nested JSON fields

Removes unnecessary attributes

Renames columns to readable names

Sets correct data types (numbers, text, date/time)

By the time data loads, it’s already analysis-ready.

4️⃣ Calculations Using DAX 📐

Instead of showing raw values, the dashboard uses DAX measures to calculate:

Average temperature 🌡️

Minimum and maximum values

Humidity percentage 💧

Wind speed insights 🌬️

These measures:

Update automatically when data refreshes

Stay consistent across all visuals

5️⃣ Exploring the Dashboard 📊

Now you’re in the dashboard.

You’ll notice:

KPI cards for quick understanding

Clean visuals focused on clarity

No clutter or unnecessary charts

Everything you see is driven by the API data and DAX logic behind it.

🔄 Refreshing the Data

Whenever you click Refresh:

Power BI calls the API again

New data is fetched

Transformations run automatically

DAX recalculates

Visuals update

This is exactly how enterprise dashboards behave.

📂 Why This Is a Template File (.pbit)

This project is shared as a template so that:

Your API key is never exposed 🔐

Anyone can reuse the dashboard logic

The same structure works for different users

Project Demo :
