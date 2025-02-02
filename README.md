# Image Extractor from URL

This Python script downloads images from a given URL and saves them into a specified folder. It uses the `requests` and `BeautifulSoup` libraries to fetch and parse the HTML content of the webpage, and the `os` library for file system operations.

## Features

*   Prompts the user for a URL and a folder name.
*   Handles cases where the specified folder already exists.
*   Identifies image URLs from various `img` tag attributes (`data-srcset`, `data-src`, `data-fallback-src`, and `src`).
*   Downloads images in binary format (`.jpg`).
*   Handles potential UnicodeDecodeErrors during image download.
*   Provides feedback on the number of images found and downloaded.
*   Uses exception handling to gracefully manage potential errors during the process.

## Requirements

*   Python 3.x
*   `requests` library: `pip install requests`
*   `beautifulsoup4` library: `pip install beautifulsoup4`

## How to Use

1.  Save the Python code as a `.py` file (e.g., `image_downloader.py`).
2.  Open a terminal or command prompt and navigate to the directory where you saved the file.
3.  Run the script using the command: `python image_downloader.py`
4.  The script will prompt you to enter the URL of the webpage you want to download images from.
5.  Next, it will ask you to enter a name for the folder where the images will be saved.
6.  The script will then attempt to download all images found on the webpage.
7.  After the download is complete, it will display a message indicating the total number of images found and the number of images successfully downloaded.  The images will be saved in the folder you specified.

## Example

```bash
$ python image_downloader.py
Enter URL:- [https://www.example.com/images](https://www.google.com/search?q=https://www.example.com/images)
Enter Folder Name:- example_images
Total 10 Image Found!
Total 8 Images Downloaded Out of 10
