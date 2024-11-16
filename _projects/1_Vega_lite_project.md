---
name: Homework 6
tools: [Python, HTML, vega-lite]
description: This is my Homework 6 submission
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---






# Homework 6


<vegachart schema-url="{{ site.baseurl}}/assets/json/plot1.json" style="width: 100%"></vegachart>

## Visualization 1: Distribution of Licenses by Type

- **Description**: This bar chart shows the distribution of different license types, with each bar representing a unique license category. The y-axis indicates the count of records for each license type, providing insight into the volume of licenses issued for each category.
- **Design Choices**: Categorical encoding is applied to the x-axis for license types, and quantitative encoding on the y-axis for the count of records. Each license type is represented by a unique color, allowing for easy differentiation across categories. This color scheme was chosen to make it simple for users to visually identify each license type without the need for an external legend.
- **Data Transformations**: The data was grouped by license type to aggregate the counts. This transformation was done to focus on the volume of each license category rather than individual records.
- **Purpose**: The goal of this visualization is to help users quickly understand which license types are most common and observe the distribution across categories. This can reveal dominant licenses in the dataset, providing a straightforward way to compare issuance volumes.


<vegachart schema-url="{{ site.baseurl}}/assets/json/plot2.json" style="width: 100%"></vegachart>

Visualization 2: Heatmap of License Issuance by Month and Year

- **Description**: This heatmap visualization shows the count of licenses issued, segmented by month and year. Each cell represents a specific month and year combination, with the color intensity indicating the volume of licenses issued during that time period.

- **Design Choices**: A heatmap was chosen to effectively convey temporal data and highlight patterns in license issuance across months and years. The x-axis represents the month, and the y-axis represents the year, providing a clear layout for exploring trends over time. The color gradient moves from light to dark shades to indicate lower to higher counts, making it easy to spot periods with more frequent license issuances.

- **Data Transformations**: The dataset was filtered by license type to allow users to explore issuance trends for specific categories. Data was aggregated by month and year to calculate the count of records for each cell in the heatmap.

- **Purpose**: The goal of this visualization is to help users identify seasonal or temporal trends in license issuance. By observing the color variations, users can quickly determine whether certain times of the year or specific years saw an increase in license issuance for particular license types. This can assist in planning and understanding patterns related to licensing demand.

## Search The Data & Methods

<!-- these are written in a combo of html and liquid --> 

<div class="left">
{% include elements/button.html link="https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_data/main/licenses_fall2022.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/devanshk220304/devanshk220304.github.io/blob/main/Hw6.ipynb" text="The Analysis" %}
</div>

