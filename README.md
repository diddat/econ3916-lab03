# Honest vs. Misleading Visualizations

## Objective

Explore how data visualization choices can change the way economic data is interpreted and identify techniques for creating accurate and honest visualizations.

## Methodology

* Recreated **Anscombe's Quartet** to demonstrate how datasets can have similar summary statistics while having very different visual patterns
* Calculated a **Lie Factor of 49.0** for a truncated-axis revenue chart and redesigned the chart using an honest baseline
* Used FRED average hourly earnings data (`AHETPI`) and deflated it to **2020 dollars** to analyze real wage trends
* Created four versions of the real wage series using:

  * A full y-axis starting at $0
  * A truncated y-axis
  * A cherry-picked time period
  * A logarithmic y-axis
* Performed a four-step exploratory data analysis (EDA) of World Bank GDP data, examining structure, distributions, relationships, and anomalies
* Built an interactive visualization using `ipywidgets` and Matplotlib that allows users to change the wage series, time period, y-axis floor, and y-axis scale while displaying a live Lie Factor

## Key Findings

* A truncated y-axis can make a relatively small change appear dramatically larger than it actually is
* The **49.0 Lie Factor** from the revenue example demonstrated how strongly visualization choices can exaggerate an effect
* Nominal wages and inflation-adjusted real wages can tell different stories because nominal values include the effects of changing prices
* Cherry-picking a time period can hide important long-term trends
* Logarithmic scales can change how growth is visually perceived and should be clearly identified to readers
* Summary statistics alone are not always enough to understand a dataset, as demonstrated by Anscombe's Quartet
* Honest data visualization requires checking the axis, time period, units, transformations, and underlying data before drawing conclusions
