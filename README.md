The YouTube Web Crawler project is designed to extract information about YouTube channel datas based on a specific search query. . Here is an overview of the project flow:

The code imports the necessary libraries and modules, including time, pprint, selenium, and related components such as webdriver, ChromeDriverManager, and By

It initializes the ChromeDriver and opens the specified YouTube channel URL (in this case, the URL is "https://www.youtube.com/@mkbhd/videos")

It locates and extracts the channel title, handle, and subscriber count using XPath selectors and assigns them to respective variables.

The code sets a wait time (in seconds) for scrolling down the page to load more videos, and initializes the last_height variable with the initial document scroll height

A while loop is implemented to repeatedly scroll down the page, wait for the specified time, and calculate the new scroll height until no more new videos are loaded.

It finds and collects the views, titles, and links of the videos using XPath selectors.

The collected video data is stored in a list of dictionaries, where each dictionary contains the title, views, and link of a video.

Finally, the list of video dictionaries (channel_data) is printed

Saving YouTube Channel datas: The extracted YouTube channel datas are stored in a csv file named "youtube_data.csv" using the save_to_csv function.
