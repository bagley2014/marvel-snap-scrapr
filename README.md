![](https://github.com/bagley2014/marvel-snap-scrapr/actions/workflows/build.yml/badge.svg)

# Marvel SNAP Scrapr

Scraper for https://marvelsnapzone.com to retrieve metadata of Marvel SNAP cards.
This is a fork of [vlmaier/marvel-snap-scrapr](https://github.com/vlmaier/marvel-snap-scrapr).

## How it works

The script uses the Beautiful Soup Python library, which pulls data out of HTML or XML files.
It scrapes the website https://marvelsnapzone.com which is well-structured and provides all required metadata about Marvel SNAP cards.
Selenium web driver is required because of the dynamic loading on the website. Otherwise, the card links are not available when going for a static approach.
In the end, a dictionary of all available cards is created and saved to `data.json` alongside downloaded card thumbnails.

## How to use it

Ensure Python is installed, then in the project's root directory, run `pip install -r requirements.txt`.

The script is run like `python scrapr.py` and, unless modified, will save the files in a subdirectory of the working directory. Therefore, it's best to run the script from the directory the output files should be in (e.g. src/assets) rather than running the script from its own root directory.
