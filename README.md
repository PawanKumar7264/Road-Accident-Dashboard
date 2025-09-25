# Road-Accident-Interactive-Dashboard
 
### 1. Project Title / Headline
Accident Analytics: Interactive Accident Dashboard  
A dynamic, interactive data visualization tool built to analyze accident data, focusing on severity, casualties, weather conditions, and contributing factors for better safety insights.

### 2. Short Description / Purpose
This dashboard serves as a comprehensive accident monitor. Its purpose is to present accident statistics in a clean, interactive, and visually intuitive format, allowing users to quickly identify patterns in severity, road conditions, weather impacts, and vehicle involvement to inform safety policies and prevention strategies.

### 3. Tech Stack
The dashboard was built using the following tools and technologies:  
• 📈 Microsoft Excel – Main data visualization platform used for report creation.  
• 📂 Excel Data Tools – Data transformation and cleaning for reshaping and preparing the data.  
• 🧠 Excel Formulas – Used for calculated measures, dynamic visuals, and conditional logic.  
• 📝 Data Modeling – Relationships established among tables for keys like Accident_Date, Year, Accident_Severity, Number_of_Casualties, Road_Type, Weather_Conditions, Vehicle_Type to enable filtering and aggregation.  
• 📁 File Format – .xlsx for development and .png for dashboard previews.

### 4. Data Source
Source: Provided Excel file ("DataSet_accident data1234.csv.xlsx") containing accident records from 2021-2022.  

Raw Data Structure: The data is structured across multiple sheets. Sheet1 contains raw row-level accident details (e.g., Accident_Severity, Accident Date, Year, Light_Conditions, Number_of_Casualties, Road_Surface_Conditions, Road_Type, Urban_or_Rural_Area, Weather_Conditions, Wind Condition, Vehicle_Type). Sheets like Sheet3 and DATA SET provide pre-aggregated summaries, such as total casualties by severity (Fatal: 6,593; Serious: 58,586; Slight: 344,510) and by vehicle type (e.g., Car: 326,922 casualties). The dataset includes over 300,000 rows, truncated in the input for brevity.  

Excel Data Transformation: Used Excel’s built-in data tools as an ETL process.  

Extraction: Imported from the Excel file, handling multiple sheets using Power Query within Excel.  

Transformation: Cleaned and flattened the data by merging sheets, handling blanks/nulls (e.g., in Year or Vehicle Type), converting serial dates (e.g., 44197 to readable formats using DATE function), and creating calculated columns with formulas (e.g., SUMIFS for aggregations like total casualties per year: 2021: 217,500; 2022: 192,189). Ensured consistency in categories (e.g., combining "Raining" and "Snowing" under Weather_Conditions).

### 5. Features / Highlights
• Business Problem  
Road safety organizations, urban planners, and insurance companies lack a centralized tool to analyze accident trends. Manual reviews of raw data are inefficient, leading to delayed insights on high-risk conditions (e.g., wet roads or rural areas). This results in poor resource allocation for safety measures, higher casualty rates, and increased economic costs from accidents.  

Key questions such as:  
- Safety Planning: Which weather or road conditions lead to the most severe accidents?  
- Vehicle Analysis: How do casualty rates differ by vehicle type (e.g., cars vs. trucks)?  
- Trend Identification: Are accidents more common in urban vs. rural areas, or under certain light conditions?  

• Goal of the Dashboard  
Improve Safety Measures: Provide a unified view to identify risk factors and optimize interventions like road improvements or weather alerts.  
Mitigate Casualties: Highlight patterns to prevent fatalities and serious injuries through data-driven policies.  
Enhance Decision-Making: Offer a single source of truth for accident data, enabling proactive strategies over reactive responses.  
Increase Efficiency: Save time by replacing manual analysis with interactive filters and visuals.  

• Walkthrough of Key Visuals  
1. Total Casualties and Severity Breakdown  
Visual Type: Pie chart with data labels and summary tables.  
Purpose: To give an immediate overview of overall impact and severity distribution.  
Detailed Functionality:  
- A summary cell shows the grand total (409,689 casualties) using SUM.  
- The pie chart, created via Excel’s chart tools, breaks down by Accident_Severity: Fatal (1.61%, 6,593), Serious (14.3%, 58,586), Slight (84.09%, 344,510).  
- PivotTables and slicers allow filtering by year (2021 vs. 2022) or area (Urban: 250,540; Rural: 159,149). This is essential for prioritizing severe cases.  
 
2. Casualties by Vehicle Type  
Visual Type: Bar chart.  
Purpose: To analyze involvement by vehicle category and identify high-risk types.  
Detailed Functionality:  
- X-axis: Vehicle types (e.g., Car, Truck, Bike).  
- Y-axis: Sum of casualties (e.g., Car: 326,922; Truck: 32,782; Bike: 33,047) using SUMIFS.  
- Bars are color-coded by severity via conditional formatting. Shows cars account for ~79.8% of casualties. Useful for targeted safety campaigns (e.g., bike helmets, truck regulations).  


3. Casualties by Road and Weather Conditions  
Visual Type: Stacked column chart.  
Purpose: To reveal environmental factors contributing to accidents.  
Detailed Functionality:  
- X-axis: Road_Surface_Conditions (Dry: 273,602; Wet: 113,575; Frost: 16,098; Snow: 6,414).  
- Stacked by Weather_Conditions (e.g., Fine, Raining, Snowing) using PivotTables.  
- Highlights trends like higher casualties on wet roads during rain. Filterable by Wind Condition (e.g., High Winds) using slicers.  

 
4. Yearly and Area-Based Trends  
Visual Type: Line chart with data filters.  
Purpose: To track changes over time and by location.  
Detailed Functionality:  
- X-axis: Years (2021: 217,500; 2022: 192,189).  
- Y-axis: Casualties, with lines for Urban vs. Rural using VLOOKUP and PivotTables.  
- Filters for Light_Conditions (Daylight: 299,280; Darkness: 110,409) and Road_Type (e.g., Single Carriageway: 303,874) via Excel slicers.  

5. Road Type Distribution  
Visual Type: Column chart.  
Purpose: To visualize infrastructure-related risks.  
Detailed Functionality:  
- Displays casualties by Road_Type (e.g., Dual Carriageway: 66,188; Roundabout: 26,107) using PivotTables.  
- Color-coded by Urban/Rural, showing single carriageways dominate (74.2%).  

• Business Impact & Insights  
Improved Safety: Identifies hotspots (e.g., wet rural roads) for targeted interventions, potentially reducing casualties by 10-20%.  
Risk Mitigation: Early warnings for conditions like frost or high winds to alert drivers.  
Data-Driven Policies: Supports decisions on infrastructure upgrades or education campaigns, lowering accident rates.  
Cost Savings: Reduces economic impact through prevention.

### 6. Screenshots / Demos
![Dashboard Preview]( https://github.com/PawanKumar7264/Road-Accident-Dashboard/blob/main/Screenshot%202025-09-26%20002447.png)
