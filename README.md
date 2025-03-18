# Google Search Scraper
## Categorizes Companies

### Overview
This script automates the process of searching for company categorization on Google using Selenium with Undetected ChromeDriver. It queries Google with the question "Is [Company] a [Category] company?" and retrieves a Yes/No response. The results are saved in CSV files.

## Requirements
- Python (>=3.7)
- Google Chrome
- Install dependencies:
  ```bash
  pip install undetected-chromedriver selenium
  ```
    ```bash
  pip install selenium
  ```
## Functionality
1. **Initialize Chrome Driver**: The script uses `undetected_chromedriver` to bypass bot detection.
2. **Open Google Search**: It loads `https://www.google.com`.
3. **Search Queries**:
   - Iterates over predefined companies and categories.
   - Enters "Is [Company] a [Category] company?" into Google search.
   - Extracts relevant text from search results.
   - Determines a "Yes" or "No" answer based on predefined logic.
4. **Save Results**: The collected data is stored in CSV files (`output1.csv`, `output2.csv`, etc.).
5. **Close Browser**: Once processing is complete, the browser session is terminated.

## Notes
- Avoid frequent searches to prevent blocking.
- Results depend on Google's answers.

## problems faced and fixes
- Bot Detection by google
  fix - used undetected-chromedriver
- web elements locator
- fixed location need popups
- fixed google ai overview search limits by dividing input company list into 3 parts and reruning whole code for 3 times exactly

