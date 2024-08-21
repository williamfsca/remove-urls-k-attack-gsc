# Remove URLs K-Attack from Google Search Console

This JavaScript bookmarklet is a simple yet powerful tool designed to automate the removal of URLs from Google Search Console. The script is particularly useful for tasks that require batch processing of multiple URLs, saving you time and effort by handling the entire process automatically.

## Features

- **URL Verification:** The script verifies if the URL is already listed in Google Search Console before attempting to remove it.
- **Automated Removal:** It handles the removal of the URLs entered by the user, waiting the necessary time between operations.
- **Error Handling:** If the message "Duplicate request" appears, the script automatically clicks "Close" and proceeds to the next URL.
- **Completion Notification:** After the process is complete, the script displays an `alert` informing the user that all URLs have been removed.
- **Daily Limit:** Please note that the Google Search Console API enforces a limit of 1,000 URL removal requests per day.

## How to Use

1. **Navigate to the URL Removal Page in Google Search Console:**
   - Open your Google Search Console account.
   - Go to the **Removals** tool under the **Index** section.

2. **Extract URLs to Remove:**
   - From Google Search Console, you can extract all the pages you want to remove. This can be done by manually compiling a list of URLs from the **Coverage** report or other relevant tools within Google Search Console.

3. **Create a Bookmarklet:**
   - In your browser, create a new bookmark.
   - In the URL field of the bookmark, paste the code provided below.

4. **Run the Bookmarklet:**
   - Go to the **URL Removal** page in Google Search Console where you want to remove URLs.
   - Click the bookmarklet you saved.
   - Paste the URLs you want to remove into the alert box presented by the script, with each URL on a new line.

5. **Execute the Process:**
   - The script will start processing each URL, checking if it has already been removed or is pending removal. If it encounters a duplicate request, it will handle it and move on to the next URL.

## Robots.txt
To block all URLs ending with `.html` from being indexed by search engines using the `robots.txt` file, you can add the following directives:

~~~
User-agent: *
Disallow: /*.html$
~~~

## Acknowledgments

I would like to thank [seoutopico](https://gist.github.com/seoutopico) for their inspiration to this code. Their work provided valuable guidance in developing this bookmarklet.

## Important Notes

- **Make sure you are on the correct page:** The bookmarklet is designed to work specifically on the **Removals** page of Google Search Console.
- **Paste your URLs carefully:** Ensure that the URLs you paste into the prompt are correctly formatted and listed one per line. This will help the script process them efficiently.
- **Remember the daily limit:** You can submit up to 1,000 URL removal requests per day, as enforced by Google Search Console's API limits.
