# Basic technologies for building a website:
* HTML5
* CSS
* Javascript
* JQuery

# Requirements
* VSCode
* Browser (Chrome, Safari, FireFox, IE)

===========> HTLM5
Official Website: http://www.w3.org/TR/html5/
* DOCTYPE
* html
* head
* body
===========> CSS
===========> JAVA
*1 to Get Data from data files
    # Note: If we write HTML and Javascript in a code and testing using local files or remote files, we need to use Async Function. Otherwise, we can get 'CORS' error.

*2 to filter data for report charts
    # The projects applies multiple .json files as data source for charts in the website. One file may be used for more than one chart.

*3 to build charts in the website using JavaScript libraries
    1) 'Chart.js' is a free JavaScript library for making HTML-based charts. It supports chart types like Area Chart, Bar Chart, Bubble Chart, Doughnut and Pie Charts, Line Chart, Mixed Chart Types, Polar Area Chart, Radar Chart, and Scatter Chart. According to data characteristics in this project, Line Chart, Bar Chart will be used to analyze data.
    2) 'Google Charts' is also applied to generate a Canada GeoChart where provinces are shown.
    3) Table is created for source data as well.

*4 to fill the filtered data into the charts

*5 to set to refresh the webpage every 15 minutes
    # When Cloud DataCenter receives updated data from data source, it starts automatically to calculate the data for reporting and save it as remote .json files in s3 bucket (bucket for data).
    # Static website hosted in another s3 bucket (bucket for website) will build reports/charts based on the files in the data bucket.
    # The HTML refreshes and retrieves data every 15 minutes to make sure the website auto updates the charts.
 
   
===========> Data Analysis
* Line Chart 1 & 2 :
    # The chart shows comparison among four main categories, Food, Cosmetics, Energy and Tabacco. According to the line chart, we can see how the prices for these categories have been growing from year 1995.
* Bar Chart:
    # The chart shows the latest price info for common products like milk and steak.
* Map Chart:
    # The chart shows all the provinces in Canada. Additionally, price comparison among regions can be calculated and shown in the chart.

