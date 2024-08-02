# TempWebScraping
Python code to pull temperature data from Wikipedia pages of Prague, Czech Republic and Santiago, Chile. I created a final plot of daily mean temperature in degrees Celcius, with one colored line for each of the two countries (red being Santiago and blue being Prague).

I used web scraping to extract tables related to temperature data using read_html in Python. The data comes from two Wikepedia pages. One is for the country of Prague, Czech Republic and the other is for Santiago, Chile.

The webpages containing the data are: <br>
https://en.wikipedia.org/wiki/Prague <br>
https://en.wikipedia.org/wiki/Santiago <br>


Since Prague is in the northern hemisphere and Santiago is in the southern hemisphere, the graph of daily mean temperature over a year span shows two lines that are "U-shaped" opposite of each other. Prague experiences summer mid-year, while Santiago experiences winter mid-year. The temperature data was in a format where with #C (#F), with the Celcius temperature listed first and the Fahrenheit temperature listed after in parentheses with a space in between. I had to split up the Celcius and Fahrenheit temperatures for each country, remove the ending parentheses, and convert all the values to floats. There were also an extraneous row for the column name and for a yearly daily average temperature, so I removed these rows.

The final plot is seen below:

<img src = "/assets/img/PragueSantiagoTemps.png">
