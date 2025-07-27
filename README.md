# Washington-EV-Analysis

This Tableau project, titled "Washington EV Analysis", provides an in-depth exploration of Electric Vehicle (EV) adoption trends in Washington, D.C. The dashboard visualizes key metrics such as EV registrations over time, vehicle types, popular models, and geographic distribution of EV owners. The goal is to help policymakers, urban planners, and EV enthusiasts understand the growth and distribution of electric vehicles in the region.

Data Sourcing & Preparation  
**1. Finding the Dataset**  
   The dataset was sourced from a public repository for Washington, D.C. government data.  
   The specific dataset used: Electric Vehicle Registrations (CSV format).  
   Alternative sources (if needed):  
   U.S. Department of Energy - Alternative Fuels Data Center  
   Kaggle EV Datasets  

   -----------------------------------------------------------------------------------------------------------------------------------------
   
**2. Data Mining & Cleaning**  
  Initial Data Exploration: Opened the CSV in Microsoft Excel and checked for missing values, inconsistencies, and duplicates.  
  Identified key columns: Vehicle Make, Model Year, Electric Range, ZIP Code, Registration Date.  
  Data Cleaning Steps: Removed Duplicates: Used Excel’s Remove Duplicates feature under the Data tab.  
  Handled Missing Values: Deleted rows with critical missing data (e.g., missing Vehicle Make or ZIP Code). Filled in missing Electric Range values with the median where applicable.  
  Standardized Formats: Converted Registration Date to a consistent date format (MM/DD/YYYY). Ensured ZIP Code was stored as text to avoid truncation.  
  Filtered Irrelevant Data: Excluded non-EV vehicles (e.g., hybrids without plug-in capability).  

-----------------------------------------------------------------------------------------------------------------------------------------

**3. Importing Data into Tableau**
The cleaned dataset was imported into Tableau Public by connecting to the CSV file. The data source was configured by verifying column data types—Registration Date was set as a date field, and Electric Range as an integer.

Four primary sheets were created for analysis:

**EV Registrations Over Time:** A line chart with Registration Date (Year-Month) on the X-axis and Number of Registrations (Count) on the Y-axis.
**Top EV Makes:** A bar chart displaying Vehicle Make on the X-axis and Count of Vehicles on the Y-axis.
**Electric Range Distribution:** A histogram grouping Electric Range into 50-mile intervals.
**Geographic Distribution:** A map using ZIP Code for granularity, with a color gradient indicating EV density.

-----------------------------------------------------------------------------------------------------------------------------------------

**Dashboard Creation in Tableau**
1. Dashboard Layout
The dashboard, titled "Washington D.C. Electric Vehicle Adoption Analysis", was designed to provide an interactive overview of EV trends. Key filters included Vehicle Make (multi-select), Model Year (range slider), and ZIP Code (dropdown).

Visualizations incorporated into the dashboard were:

A line chart showing EV registration trends over time.

A horizontal bar chart ranking the most popular EV brands.

A histogram illustrating the distribution of electric ranges.

A geographic heatmap highlighting EV adoption by ZIP code.

2. Interactivity & Usability
To enhance user engagement, tooltips were added to display detailed information when hovering over data points. Dashboard actions were implemented to enable cross-filtering—selecting a specific vehicle make, for instance, would dynamically update the other charts. The dashboard was also optimized for mobile devices using Tableau’s device layout editor.

3. Final Touches
A cohesive color scheme (green/blue tones) was applied to symbolize sustainability. Clear axis titles and annotations were included for readability, along with a brief summary of key findings in text boxes to guide interpretation.

-----------------------------------------------------------------------------------------------------------------------------------------

**Publishing & Sharing**
1. Uploading to Tableau Public
The finalized workbook was saved as a .twbx file and published to Tableau Public, making it accessible to a broader audience. The public link was included in project documentation for easy sharing.
