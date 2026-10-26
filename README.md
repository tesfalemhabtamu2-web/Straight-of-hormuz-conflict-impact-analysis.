# Strait of Hormuz Conflict Impact Analysis

Strait of Hormuz Conflict Impact Analysis

1. Project Overview

This research project examines changes in Brent crude oil prices around the geopolitical conflict event dated February 28, 2026. It uses Python and publicly available oil price data to explore possible implications for global energy markets and supply chains.

2. Research Objectives

- Analyze Brent crude oil price trends before and after the selected event date.
- Compare average oil prices across two periods.
- Develop practical skills in Python, data analysis, and research visualization.
- Establish a foundation for further research on maritime trade and supply chain disruptions.

3. Preliminary Findings

The initial analysis found the following average prices:

Measure| Result
Average price before the event| $68.37 per barrel
Average price after the event| $109.52 per barrel
Difference| $41.15 per barrel
Percentage difference| 60.19%

These are preliminary descriptive results based on the selected periods. They do not prove that the conflict caused the price increase. Other market conditions may also have influenced oil prices.

4. Data and Tools

- Data source: Brent crude oil price series accessed through FRED, sourced from the U.S. Energy Information Administration.
- Programming language: Python
- Tools: Google Colab, pandas, and Matplotlib
- Data format: CSV
- Visualization: Brent crude oil price chart

5. Repository Contents

- "01_brent_oil_price_analysis.ipynb": Initial analysis and visualization.
- "02_oil_price_reliability_check.ipynb": Statistical summaries and reliability checks.
- "brent_oil_prices.csv": Oil price dataset.
- "brent_oil_price_chart.png": Saved oil price chart.

Note: Update the filenames above if your actual repository uses different names or folders.

6. Limitations

This project uses a before-and-after comparison. It does not establish causation, account for all external market influences, or independently measure shipping activity through the Strait of Hormuz. Further analysis is required.

7. Researcher

Tesfalem Habtamu
Logistics and Supply Chain Management
Addis Ababa University

8. Project Status

Initial oil price analysis completed. Further work will explore shipping activity, maritime trade, and potential supply chain implications.
 9. Data Visualizations

#Brent Crude Oil Prices Over Time

![Brent crude oil price trend](brent_oil_price_chart.png)

Average Oil Prices Before and After the Selected Event

![Comparison of average Brent crude oil prices](brent_oil_price_comparison.png)

The line chart illustrates daily Brent crude oil price movements. The bar chart compares average prices in the selected 60-calendar-day periods before and after February 28, 2026.

These visualizations show descriptive price differences. They do not establish that the conflict caused the observed increase.


10. Maritime Shipping Analysis

Preliminary Findings

The preliminary analysis of IMF PortWatch data shows a substantial decrease in reported daily ship arrivals across five vessel categories in the 60-day period following February 28, 2026. The combined daily average decreased from 68.07 before the selected event to 5.03 afterward, representing an approximate decline of 92.61%.

The largest percentage decreases were observed in roll-on/roll-off vessels (100%), container ships (95.51%), and tankers (94.61%). These results indicate a major change in recorded maritime activity during the comparison period.

However, the findings should be interpreted cautiously. PortWatch uses AIS-based vessel tracking, which can be affected by signal interruptions, GPS interference, spoofing, and vessels not transmitting. The before-and-after comparison also does not establish that the conflict alone caused the observed decline.

Data source: IMF PortWatch, Strait of Hormuz monitoring dashboard.

Method:** Comparison of average daily reported vessel counts across two 60-calendar-day periods surrounding February 28, 2026.

Visualization

![Average daily ship arrivals before and after the selected event](ship_arrivals_comparison.png)

11.  Combined Maritime Shipping and Cargo Analysis

This analysis compares reported vessel arrivals and estimated cargo volume during the 60 days before and after February 28, 2026, the selected event date.

The combined dataset presents average daily values for five vessel categories: container ships, dry bulk carriers, general cargo ships, roll-on/roll-off vessels, and tankers. It helps compare changes in recorded maritime activity and estimated cargo movement following the event.

 [Download the combined Hormuz analysis](combined_hormuz_summary.csv)

The results describe changes in the available data and do not, by themselves, establish that the conflict caused every observed change. AIS signal disruptions, GPS jamming, spoofing, and vessels switching off tracking systems may affect recorded vessel movements. Estimated cargo volume should also be interpreted as an estimate rather than official customs trade data.

Data Files

- `ship_arrivals_comparison.csv`: Summary of daily average vessel counts and percentage changes.
- `ship_arrivals_comparison.png`: Comparison chart for the five vessel categories.


Reported Vessel Arrivals: Before vs. After the Event

![Comparison of reported vessel arrivals before and after the February 28, 2026 event](vessel_arrivals_comparison.png)

Key Findings

1. Global Oil Prices

The comparison of Brent crude oil prices over the 60-day periods before and after February 28, 2026, showed an increase in the average price from **$68.37 to $109.52 per barrel**, representing a rise of approximately 60.19%

2. Reported Maritime Activity

The average daily number of reported vessel arrivals across the five categories declined from approximately **68.07 to 5.03**, a decrease of about **92.61%**.

The largest recorded declines were in roll-on/roll-off vessels, container ships, and tankers. These results indicate a substantial reduction in recorded maritime activity during the selected post-event period.

3. Estimated Cargo Volume

The estimated cargo volume data also showed substantial declines across the five vessel categories. Tankers and container ships experienced particularly large reductions in the available data.

These estimates provide additional evidence of changes in maritime activity, but they should not be interpreted as direct measurements of official trade or customs volumes.

Limitations of the Study

1. Short observation period:** The analysis compares two 60-day windows and may not capture longer-term effects.
2. Causality:** A before-and-after comparison cannot establish that the conflict alone caused the observed changes. Other economic, political, and market factors may have contributed.
3. AIS data reliability:** GPS jamming, AIS spoofing, and vessels switching off tracking systems may affect the accuracy of recorded vessel movements.
4. Estimated cargo volume:** Cargo estimates are not equivalent to verified customs records or actual delivered cargo.
5. Data coverage:** Results depend on the completeness, accuracy, and definitions of the downloaded datasets.

Conclusion

The preliminary findings show that the period following February 28, 2026, was associated with higher average Brent crude oil prices and substantially lower recorded maritime activity in the selected Strait of Hormuz datasets. The findings highlight the importance of this strategic chokepoint to energy markets and maritime supply chains.

Further research using longer observation periods, additional control variables, and more robust statistical methods is needed before drawing strong conclusions about the causal impact of the conflict.


### Statistical Test of Brent Oil Prices

A Welch's independent-samples t-test was conducted to compare daily Brent crude oil prices during the 60 calendar days before and after February 28, 2026.

The average price increased from $68.37 per barrel before the selected event date (43 observations) to $109.52 per barrel afterward (41 observations), representing an increase of approximately 60.19%.

The test produced a t-statistic of 18.678 and a p-value of 8.82 × 10⁻²³. The difference was statistically significant at the 5% level.

These results provide strong evidence that average Brent prices differed between the selected periods. However, the test does not establish that the conflict alone caused the increase. Because daily prices may be correlated over time, further analysis using methods appropriate for time-series data is recommended.
