# Fleet-Management-Dashboard

Welcome to the **Fleet Management Dashboard** project! This repository contains a comprehensive Power BI solution designed to help fleet managers and business leaders monitor and
 optimize fleet performance.

## Project Overview

The Fleet Management Dashboard is tailored to assist fleet managers in efficiently overseeing fleet operations. Key metrics include fuel usage, maintenance expenses, kilometers traveled, 
and driver KPIs. This dashboard provides valuable insights to streamline operations, enhance decision-making, and optimize fleet performance.

## Technologies Used
- Advanced Excel 👨‍💻
- Power BI 📊
- Statistics 📜

## Features

- **Liters Consumed**: Monitor fuel consumption across the fleet.
- **Total Drivers**: Track the number of active drivers.
- **Kilometers Traveled**: Measure the distance covered by the fleet.
- **Fixed Costs**: Keep an eye on fixed expenses associated with fleet management.
- **Fuel Usage**: Analyze fuel usage patterns and identify areas for improvement.
- **Maintenance Expenses**: Track maintenance costs to ensure efficient budgeting.
- **Driver KPIs**: Evaluate driver performance using key performance indicators.

## Dashboard Content

- **Cards**:
  1. Total Liters Consumed
  2. Total Maintenance Cost
  3. Total Fuel Consumed
  4. Total KM Traveled
  5. Total Fix Cost
  6. Total Drive

- **Table**:
  - Details about Driver, Maintenance Cost, Fuel Consumed, KM Traveled, Fix Cost, and Liters Consumed

- **Line Chart**:
  - Trends for the above metrics

- **Filters**:
  - Trailer Type: Dry, Fridge, Reefer
  - Truck Types: Box, Semi-Trailer, Tractor, Trailer

## Measures and Formulas Used

**Date Table**:
```DAX
Date Table = 
ADDCOLUMNS(
    CALENDARAUTO(),
    "Month", FORMAT([Date], "MMM"),
    "Month Number", MONTH([Date]),
    "Year", YEAR([Date]),
    "Quarter", "Q" & FORMAT([Date], "Q"),
    "Day Name", FORMAT([Date], "ddd"),
    "Days", 1
)



## How to Use
1. **Download the Project**: Clone this repository or download the ZIP file.
2. **Open the Power BI File**: Open the `.pbix` file in Power BI Desktop.
3. **Explore the Dashboard: Interact with the visualizations and analyze the data.

## Contributing
Feel free to fork this project, submit issues and pull requests. We appreciate your contributions.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

