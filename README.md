# HR Analytics Project

## Project Overview

This HR Analytics project was developed during my internship at a Microsoft Silver Partner company. The project focuses on providing insights into the organization's human resources data, specifically related to leaves, work-from-home (WFH), and timesheets. The primary data source for this project is the company's HR portal, with data extracted to Excel files. The project involved loading the data into Power BI, cleaning it, establishing relationships between tables, applying DAX functions, and creating comprehensive reports.

## Data Source and ETL Process

The data for this project came from the company's HR portal and was initially exported as Excel files. My responsibilities included:

- **Data Loading**: Importing the Excel files into Power BI.
- **Data Cleaning**: Handling missing values, correcting inconsistencies, and ensuring data quality.
- **Table Relationships**: Creating logical relationships between tables (e.g., employee data, leave entitlements, WFH logs, and timesheets).
- **DAX Functions**: Using DAX to perform advanced calculations and create meaningful metrics for the reports.

## Report Structure

The report contains three main pages:
1. **Leaves Page**:
    - Provides insights into the different types of leaves taken by employees, such as Casual, Sick, and Earned leaves.
    - Shows leave entitlement for each employee, including how many leaves were applied for, approved, rejected, or cancelled.
    - Performance metrics indicate the balance between applied leaves and those actually taken.
  
2. **WFH (Work From Home) Page**:
    - Tracks employees' work-from-home days on a monthly basis.
    - Monitors compliance with the organization's WFH policy (e.g., 6 days per month limit).
    - Includes conditional formatting to flag employees who exceed the allowed WFH limit.
  
3. **Timesheets Page**:
    - Displays timesheet data for employees, including the number of hours worked over a specific period.
    - Visualizes timesheet submissions for periods ranging from 5 to 7 days.
    - Week calculations ensure consistency by capping at 52 weeks per year to avoid issues with 53-week years.

## Key Features and Metrics

- **Leave Entitlement and Utilization**:
    - Visualizes how many leaves each employee is entitled to, how many they applied for, and the status of those applications (approved, rejected, cancelled).
  
- **Work From Home Tracking**:
    - Monitors monthly WFH days for each employee.
    - Highlights any discrepancies (e.g., exceeding 6 WFH days in a month) using conditional formatting (red for over limit, green for within limit).

- **Timesheet Submission and Weekly Analysis**:
    - Tracks timesheet submissions over flexible periods (5-7 days).
    - Ensures weekly reporting consistency, with a custom DAX formula to handle weeks correctly (capping at 52 weeks).

## Technical Stack

- **Data Source**: HR portal data extracted into Excel files.
- **Tools**: Power BI for data visualization and report creation.
- **DAX (Data Analysis Expressions)**: Used extensively for custom metrics, calculated columns, and conditional formatting.
  
  
## Challenges and Solutions

1. **Handling 53-Week Year Issues**:
    - The default DAX `WEEKNUM` function was adjusted to cap at 52 weeks to maintain consistency in timesheet reporting.

2. **Conditional Formatting Based on WFH Limits**:
    - Applied DAX measures and rules-based conditional formatting to highlight employees exceeding their monthly WFH limit.

## Future Enhancements

- **Expand Report Scope**: Include more HR KPIs such as overtime analysis, employee satisfaction metrics, and attrition rates.
- **Interactive Dashboards**: Enable interactive drill-downs for deeper insights into individual employee performance and trends.
- **Automated Data Refresh**: Set up automated data refresh schedules to keep the report up-to-date without manual intervention.

## Conclusion

This project serves as a comprehensive HR analytics tool that helps the organization track employee leaves, WFH compliance, and timesheet submissions. The insights generated by this report can assist HR managers in making data-driven decisions and optimizing workforce management.
