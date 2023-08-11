# Real Estate Agent Web Scraper

This Python project demonstrates web scraping skills using BeautifulSoup and requests to extract real estate agent information from Zillow's professional directory.

## Project Highlights

- Utilizes Python for web scraping tasks.
- Employs the BeautifulSoup library to parse HTML content.
- Makes HTTP requests using the requests library.
- Randomizes user agents for variety and introduces delays to simulate human browsing behavior.
- Extracts agent names, phone numbers, and corresponding states from specified URLs.
- Stores scraped data in a pandas DataFrame.
- Exports the DataFrame to a CSV file for further analysis.

## Code Sample

```python
# ... (code to import libraries and define base_urls and user_agents)

for base_url in base_urls:
    # ... (loop to iterate through pages and extract agent data)

df = pd.DataFrame(agent_data)
df.to_csv('agents.csv', index=False)
```

## How to Use

1. Clone the repository.
2. Ensure you have the required dependencies installed (`requests`, `beautifulsoup4`, `pandas`).
3. Customize the `base_urls` list with the URLs you want to scrape.
4. Run the script to extract agent data and save it to a CSV file.
