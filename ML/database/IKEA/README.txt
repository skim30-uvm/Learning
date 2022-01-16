Source : https://www.kaggle.com/ahmedkallam/ikea-sa-furniture-web-scraping
Context
This notebook is a practice of web scraping techniques. The web scraping has been applied on IKEA Saudi Arabian website for the furniture category. The scraped website link: https://www.ikea.com/sa/en/cat/furniture-fu001/

The data requested by 4/20/2020. The libraries used are BeautifulSoup and Selenium for web scraping, as well as regular Python libraries: Pandas, Numpy, and Regex for regular analysis activities. Number of rows=2962 Number of features=13

Content
item_id : item id wich can be used later to merge with other IKEA dataframes
name: the commercial name of items
category:the furniture category that the item belongs to (Sofas, beds, chairs, Trolleys,…)
Price: the current price in Saudi Riyals as it is shown in the website by 4/20/2020
old_price: the price of item in Saudi Riyals before discount
Short_description: a brief description of the item
full_Description: a very detailed description of the item. Because it is long, it is dropped from the final dataframe, but it is available in the code in case it needs to be analyzed.
designer: The name of the designer who designed the item. this is extracted from the full_description column.
size: the dimensions of the item including a lot of details.As a lot of dimensions mentioned and they vary from item to item,
the most common dimensions have been extracted which are: Height, Wideh, and Depth. This column is dropped from the final dataframe, but it is available in the code in case it is needed.
width: Width of the item in Centimeter
height: Height of the item in Centimeter
depth: Depth of the item in Centimeter
sellable_Online: if the item is available for online purchasing or in-stores only (Boolean)
other_colors: if other colors are available for the item, or just one color as displayed in the website (Boolean)
link: the web link of the item
Licences
The scraped website link: https://www.ikea.com/sa/en/cat/furniture-fu001/

Inspiration
The collected dataset can be utilized mainly towards two data science modeling:

Regression: Predict the Sales Price of new items
Classification: Predict the category of new items
Classification: Predict if an item will be discounted
