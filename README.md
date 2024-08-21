# Remove urls k-attack from Google Search Console
This JavaScript bookmarklet is a simple yet powerful tool designed to automate the removal of URLs from Google Search Console. The script is particularly useful for tasks that require batch processing of multiple URLs, saving you time and effort by handling the entire process automatically.


## Features

- **URL Verification:** The script verifies if the URL is already listed in Google Search Console before attempting to remove it.
- **Automated Removal:** It handles the removal of the URLs entered by the user, waiting the necessary time between operations.
- **Error Handling:** If the message "Duplicate request" appears, the script automatically clicks "Close" and proceeds to the next URL.
- **Completion Notification:** After the process is complete, the script displays an `alert` informing the user that all URLs have been removed.
- **Daily Limit:** Please note that the Google Search Console API enforces a limit of 1,000 URL removal requests per day.

## How to Use

1. **Create a Bookmarklet:**
   - In your browser, create a new bookmark.
   - In the URL field, paste the code below.

2. **Run the Bookmarklet:**
   - Go to the Google Search Console page where you want to remove URLs.
   - Click the bookmarklet you saved.
   - Enter the URLs you want to remove, one per line.

  ```javascript
