# Project-tableau
 Global agricultural Trade Analisis
For the annotation you can either annotate the area, and write the insight manually, or you can annotate the Mark, and just keep the Product Name reference.
Link del projecto en youtube: https://youtu.be/iVd3OgTmnxs?si=vkxuB2xHYnfeqxo8
Global Agricultural Trade Analysis: Instructions
Follow the steps in this reading item. Once you are done, you can move on to the Assignment, where you will answer a quiz based on your findings.

Background
As a data analyst at a Business Intelligence consulting firm,  you’ve been asked to analyze international trade data for a major agricultural conglomerate. The client produces, processes, and trades food commodities globally, and is looking to diversify, find emerging markets, and strengthen supply chains. Your manager needs visualizations of key agricultural products to support global expansion plans, focusing on both imports (market demand) and exports (competitive landscape and trade opportunities).  

# Global Agricultural Trade Analysis: Instructions

Follow the steps in this reading item. Once you are done, you can move on to the Assignment, where you will answer a quiz based on your findings.

# **Background**

As a data analyst at a Business Intelligence consulting firm,  you’ve been asked to analyze international trade data for a major agricultural conglomerate. The client produces, processes, and trades food commodities globally, and is looking to diversify, find emerging markets, and strengthen supply chains. Your manager needs visualizations of key agricultural products to support global expansion plans, focusing on both imports (market demand) and exports (competitive landscape and trade opportunities).

For this assignment you will be using a filtered version of the [International Trade Data from the  Atlas of Economic Complexity Dataverse](https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/YAVJDF)

From the available variables you will only be working with:

- **Export Value:** export value (in USD).
- **Import Value:** import value (in USD).

## **Hints:**

If you get stuck or have doubts about how to solve any of the exercises, you can look into [this document](https://docs.google.com/document/d/1b44cJFCBJD-PFO6qTEkw30VjTRQq5FekHHunvHdWbqo/edit?usp=sharing) for hints.

# **Step 1: Copy the starter workbook**

Begin by copying [this starter Workbook](https://public.tableau.com/views/C5M2Assignment-StarterWorkbook/Sheet1?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link). The Workbook has all the data connections in place so you can start building your charts. You can find the original data used in the Workbook in [this folder](https://drive.google.com/drive/folders/1JU9XeeaIVvyDgmuA4bf98d8JrTLuhaQB?usp=drive_link).

1. Open [Tableau Public](https://public.tableau.com/), and log into your account.
2. Follow [this link](https://public.tableau.com/views/C5M2Assignment-StarterWorkbook/Sheet1?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link) to access the Workbook.
3. Click on the Make a Copy button.
4. Click on the Publish button to start saving your changes.
5. Take a couple of minutes to explore the tables and their connections.
6. Now you are ready to start working!

# **Step 2: Create visualizations**

## **Exercise 1: Market overview visualization**

It is important for the client to identify the biggest players in agricultural trade. Understanding top exporters and importers helps them find potential trade partners and assess competition.

1. Rename the worksheet to “Total Exports by Country”.
2. Drag the field “**Country Name**” into the *Rows* shelf and “**Export Value**” into the *Columns* shelf*.*
3. Drag the field “**Product Name**” into *Color* in the Marks card*.*
4. Using the *Show Me* panel, create a **stacked bars** chart showing the results.
5. Sort the bars in descending order, so the country with most exports appears first.
6. Show mark labels.

## **Exercise 2: Strongest trade relationships analysis**

You decide to identify key trade relationships between countries by understanding which countries consistently trade with each other.

1. Create a new Worksheet and name it “Trade Partners” .
2. Create a new Calculated Field called “Total Trade”, which the sum of Exports and Imports between countries .
3. Create a **heatmap** comparing the “**Total Trade**” for each country pair. Have “**Country Name**” in the *Rows* shelf and “**Partner Country Name**” in the *Columns* shelf*.*
To clarify, if "Country Name" is Brazil and "Partner Country Name" is the USA, then "Export Value" is what Brazil sold to the USA, and "Import Value" is what Brazil bought from the USA.
4. Filter the rows and columns so that you only show the 10 country pairs with highest “Total Trade”.
    1. Go to the *Rows* shelf.
    2. Click the arrow on “**Country Name**”.
    3. Select the option *Filter* from the dropdown menu.
    4. When the filter menu appears, select the option **Top/Botton**, and choose the “**By Field**” option. Then repeat for the columns.
5. Customize the graph (optional):
    1. Rotate the labels in the horizontal axis.
    2. Adjust the size of the cells in the heatmap for better interpretability.
    3. If needed, change the color scale to improve interpretability.
6. Add an annotation showing the countries with the highest trade.

## **Exercise 3: Analyzing trade partners**

Consider the trade between China and Brazil, you decide to investigate this relationship a little deeper.

1. Create a new Worksheet with the name "China-Brazil".
2. Create a **lines chart** showing the time evolution of the **imported** and **exported** amounts for each product. You only need to filter the pair once. For example, if you keep Country Name: Brazil and Partner Country Name: China, the the Export Value represents the amount that Brazil exported to China, and the Import Value has the amount that China exported to Brazil.
3. Tune the vertical axis:
    1. Change the y-axis labels from Export Value and Import Value to “Brazil Exports” and “China Exports”.
4. Annotate the highest Exported product by each country.

## **Exercise 4: US imports**

Your client is interested in trading in the US markets. They want to understand which were the most in-demand categories in the last reported year.

1. Create another sheet Called “US Imports”.
2. In this new sheet drag the "**Product Name**" and "**Import Value**".
3. Add a filter to show only the imports of the United Stated of America (use the **Product Name** field).
4. Add another filter to show only the values for the **Year** 2022.
5. Using the *Show Me* panel, create a pie chart.
6. Show the percentage of each product, instead of the total value.
7. Change the title to "US Imports (2022)".

## **Exercise 5: Analyzing Agricultural Trade Trends**

In order to anticipate market trends and prepare for future changes, you want to see how agricultural trade has evolved over time.

1. Create a new worksheet called Imports Over Time.
2. Create a **line chart** showing the total “**Import Value**”.
3. Break it down by “**Product Name**”.

## **Exercise 6: Imports by Country - Map**

Your client wants to understand which countries import the most agricultural products and how demand varies across different products. By creating a map visualization, they can quickly identify key import markets and track trends by product.

1. Create a new sheet called Imports Map.
2. Create a **map chart** where the *colors* represent total “**Import Value**”, and the *detail* is the “**Country Name**”. Dragging **Country Name** into *Detail* in the Marks card tells Tableau to draw one mark per country, allowing **Import Value** to be colored separately for each country.
3. Add the “**Product Name**” field to Filters, and select show filter.
4. Create another filter for “**Year**”, and select the year 2022.
5. Adjust the color scale so that the map is easier to read.

Once you finish all of this steps, you are ready to move on to the Graded Assignment, and answer the questions.
