# image_downloader

![Logo](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQ5ETagi_CWCmvYNKXy5LMVe-cRwHO_lGbi2eRuVxrrIK7f7d85XZefoqOja6BZWsD7Nvw&usqp=CAU)

This Python script is designed to download images from a list of URLs provided in an Excel file. It utilizes asynchronous programming with the aiohttp and asyncio libraries to efficiently download images concurrently. The downloaded images are saved to a specified destination folder.

## Prerequisites
Before running the script, make sure you have the following dependencies installed:
-    Python 3.7+
-    aiohttp
-    openpyxl
-    aiofiles

You can install the required Python packages using pip:

```python
pip install aiohttp openpyxl aiofiles
```



## Usage
```python
python image_downloader.py
```

1.    Prepare an Excel file with a list of URLs in the first column (Column A). Make sure that the Excel file is named "urls.xlsx" and is in the same directory as the script.

2.    Create a destination folder where the downloaded images will be saved. By default, the destination folder is named "downloaded_images," but you can change it as per your preference.

3.    Run the script using the following command:
## Script Details

-    The download_image function asynchronously downloads images from the provided URLs using the aiohttp library. It saves the images in the specified destination folder with filenames based on the URL.

-    The main function is the entry point of the script. It loads the URLs from the "urls.xlsx" file and initiates concurrent downloads using asyncio. The downloaded images are saved to the destination folder.
## Folder Structure
After running the script, your project directory should have the following structure:

- image_downloader.py
- urls.xlsx
- downloaded_images/
  - image1.jpg
  - image2.jpg
  - ...


## Note

-    If you wish to change the destination folder, simply modify the destination_folder variable in the script.

-    Ensure that the Excel file "urls.xlsx" is correctly formatted with URLs in the first column (Column A).

-    Make sure you have proper permissions to write to the destination folder.

I'm sure you can handle it; after all, you're the big boys!
