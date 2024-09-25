1. News Scraping Script:
This script scrapes news articles from specified websites (e.g., BBC, New York Times) and saves the data as a CSV file. It extracts article titles, summaries, publication dates, sources, and URLs, then stores them in a structured format for further analysis.

2. Article Categorization Script:
This script loads the previously scraped news articles, categorizes them into predefined categories (Politics, Technology, Sports, Business, Health) based on keyword matching in the article summaries, and saves the categorized articles into a new CSV file.

3. FastAPI Application:
This FastAPI application serves the categorized news articles via multiple endpoints:
GET /articles: Fetches all articles with optional filters for date range and category.
GET /articles/{id}: Retrieves a specific article by its ID.
GET /search: Allows searching for articles by keywords in their title or summary. The application reads articles from the news_articles_categorized.csv file and provides a RESTful API for accessing and filtering the data.
