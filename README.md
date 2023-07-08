![](https://github.com/bagley2014/marvel-snap-scrapr/actions/workflows/build.yml/badge.svg)

# Marvel SNAP Scrapr

Scraper for https://marvelsnapzone.com to retrieve metadata of Marvel SNAP cards.

## How it works

The script uses the Beautiful Soup Python library, which pulls data out of HTML or XML files.
It scrapes the website https://marvelsnapzone.com which is well-structured and provides all required metadata about Marvel SNAP cards.
Selenium web driver is required because of the dynamic loading on the website. Otherwise, the card links are not available when going for a static approach.
In the end, a list of dictionaries is created for all available cards and the card thumbnails are downloaded.

## How to use it

Ensure Python is installed, then in the project's root directory, run `pip install -r requirements.txt` followed by `python scrapr.py`
