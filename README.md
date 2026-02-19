This project analyzes publicly available data from the DKASC solar research center in Alice Springs. 
It compares three systems: a fixed panel from 2008 (BP), a solar tracker from 2008 (Kyocera), and a fixed panel from 2016 (Tindo). 
The goal is to quantify the impact of the technology versus the tracking systems.

Methodology
Data: Obtained from DKASC (Desert Knowledge Australia Solar Centre), with daily frequency throughout 2025.

Cleaning: Processed in R to unify formats and remove duplicates.

Normalization: All raw power values (power_kwh) were normalized by dividing by the installed capacity of each system (capacity_kwp), using the formula:
normalized generation = power kwh / capacity kwp.

The capacities used are:

BP Fixed 2008: 5.0 kWp

Kyocera Tracker 2008: 5.4 kWp

Tindo Fixed 2016: 5.5 kWp

This industry-standard calculation produces values in kWh/kWp, allowing for a fair comparison of technological efficiency regardless of system size. The final dashboards show daily and monthly aggregates of this normalized metric.The base calculation of normalized generation is done with a capacity of 5.0 kW since this is a measurement that all panels reach.

Visualization: Interactive dashboards created in Tableau Public.

Dashboards and Key Findings

Dashboard 1: Overview
Annual Totals: Tindo (2016) leads with 2,076.9 kWh/kWp, followed by Kyocera (1,828.5) and BP (1,499.9).

Monthly Generation: Clear seasonal pattern with peaks in summer (December-February).

Dashboard 2: Comparative Advantages
Monthly Dominance Heatmap and Line Graphic: Tindo dominates all 12 months of the year (green), Kyocera never wins a month.

Dashboard 3: Stability and Consistency
Tracker Advantage (Kyocera vs. BP): The tracker generates between +4 and +9 kWh/kWp more each month. The advantage is greater in summer.

Modern vs. Tracker (Tindo vs. Kyocera): The modern panel outperforms the older tracker in most months. Annual advantage: +13.7%.

Monthly distribution: Tindo (green) is the most stable and productive. Kyocera (orange) shows high variability (greater risk). BP (blue) is stable but obsolete.


Conclusions
Technology improves faster than tracking: A modern fixed panel outperforms an older tracker by 13.7%.
Trackers offer an advantage: 22% better than fixed panels of the same era.
Technological evolution: 38.7% improvement in 8 years (Tindo vs. BP).
Recommendation: Invest in modern panels first. Add trackers only if the panels are current and the budget allows.



Original data: DKASC (https://dkasolarcentre.com.au/)

Tools Used
- Tableau Public (dashboards)
- R (cleanup and analysis)
- Git/GitHub (version control and portfolio)



View the interactive dashboard by clicking here
https://public.tableau.com/views/SolarEnergyAustralia8-YearPerformanceAnalysis/StabilityReliabilityAnalysis?:language=en-GB&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link
