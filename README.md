# web_scraping_discogs

README

####### Cloning repository #########
use the following command to clone repositor with both the discogs and price_discogs submodules included:

git clone --recurse-submodules https://github.com/boubinmj/web_scraping_discogs

####### Discogs Submodule ##########

The discogs submodule is used to scrape Wikipedia.org for the Billboard 200 data related to the top rated album of each week
To scrape the data, run the following command in the discogs/discogs/ directory:

scrapy crawl discogs_spider

The data scraped using this command will store data from all pages chosen into the discogs.csv file

There is prescraped data included in this project.  This data is stored in the data/ directory.
Preset visualizations have been created to provide insight into this data.  To view the premade visualziation,
run the visualization.py file.

####### price_discogs Submodule #####

The price_discogs module scrapes data directly from the discogs marketplace.  To scrape new data, 
run the following command with scrapy:

scrapy crawl price_discogs_spider

The data scraped will be stored in the discogs.csv file.

This submodule also has a data/ directory containing pre-scraped data, and users can run the 
visualization.py file to view visualizations for the prescraped data.
