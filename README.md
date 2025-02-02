# Image Downloader from URL

## Description
This script allows users to download all images from a provided URL and save them to a folder of their choice. It uses Python's `requests` and `BeautifulSoup` libraries to fetch the content of the URL, parse the HTML, and extract the image URLs. The images are then downloaded and saved in the specified folder.

## Features
- Download all images from a given URL.
- Supports multiple image source attributes (`src`, `data-src`, `data-srcset`, `data-fallback-src`).
- Automatically creates a folder to store the downloaded images.
- Provides a count of how many images were downloaded.

## Requirements
- Python 3.x
- `requests` library
- `BeautifulSoup` from `bs4` library

## Installation

To install the required libraries, run the following commands in your terminal:

```bash
pip install requests
pip install beautifulsoup4
