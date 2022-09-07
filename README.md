# WebScraping_Challenege-
In this assigmnent for web scraping

Scraping

MongoDB and Flask Application

Submission

Part 1: Scraping

Complete your initial scraping using Jupyter Notebook, BeautifulSoup, Pandas, and Requests/Splinter.

Create a Jupyter Notebook file called mission_to_mars.ipynb. Use this file to complete all your scraping and analysis tasks. The following information outlines what you need to scrape.
NASA Mars News

Scrape the Mars News Site and collect the latest News Title and Paragraph Text. Assign the text to variables that you can reference later.
JPL Mars Space Images—Featured Image

Visit the URL for the Featured Space Image site here.

Use Splinter to navigate the site and find the image URL for the current Featured Mars Image, then assign the URL string to a variable called featured_image_url.

Use Pandas to convert the data to a HTML table string.

Mars Hemispheres

You will need to click each of the links to the hemispheres in order to find the image URL to the full-resolution image.

Save the image URL string for the full resolution hemisphere image and the hemisphere title containing the hemisphere name. Use a Python dictionary to store the data using the keys img_url and title.

Append the dictionary with the image URL string and the hemisphere title to a list. This list will contain one dictionary for each hemisphere.

Part 2: MongoDB and Flask Application

Use MongoDB with Flask templating to create a new HTML page that displays all the information that was scraped from the URLs above.

Start by converting your Jupyter notebook into a Python script called scrape_mars.py by using a function called scrape. This function should execute all your scraping code from above and return one Python dictionary containing all the scraped data.

Next, create a route called /scrape that will import your scrape_mars.py script and call your scrape function.

Store the return value in Mongo as a Python dictionary.
Create a root route / that will query your Mongo database and pass the Mars data into an HTML template for displaying the data.

Create a template HTML file called index.html that will take the Mars data dictionary and display all the data in the appropriate HTML elements. Use the following as a guide for what the final product should look like, but feel free to create your own design.

