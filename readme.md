# Search_With_AI: Advanced AI-Powered Web Search Tools

This repository contains two powerful AI-enhanced search tools designed for deep web analysis and news aggregation. 
These tools combine web scraping, search engine querying, and AI-powered analysis to provide comprehensive and intelligent search results.
 

## Tools

### 1. deep_search-ai

An advanced web search and analysis tool that leverages multiple search engines and AI to provide in-depth information on given topics.

#### Features:
- Multi-engine search (Google, Bing, and other API-based search engines)
- Web scraping of search results
- AI-powered analysis and summarization of scraped content
- Customizable search parameters
- Support for knowledge panel information extraction
- Utilizes public APIs for enhanced search capabilities

for more scripts using GPT for translation and subtitle check here: [Subtitle Management Tools section in the main README](https://github.com/YanivHaliwa/Linux-Stuff/tree/master?tab=readme-ov-file#subtitle-management-tools).


#### Usage:
```
./deep_search-ai [query] [options]
```

Options:
- `-a`, `--ai`: Perform AI analysis on the results
- `-r`, `--results`: Display only search results without AI analysis


### 2. news_search-ai

An AI-enhanced news aggregation and summarization tool.

#### Features:
- Focuses on recent news articles
- Uses Google News search
- Extracts content from news articles
- AI-powered summarization and analysis
- Generates HTML output for easy reading

#### Usage:
```
./news_search-ai [query]
```

## API Usage Strategy

This tool employs a unique strategy to maximize the use of free API tiers:

1. **Multiple API Services**: It uses both SerpAPI and multiple endpoints from RapidAPI for search queries.
2. **Intelligent Switching**: The script attempts to use different API endpoints when rate limits are reached on one.
3. **Fallback Mechanism**: If one API fails or reaches its limit, the script automatically tries the next available API.

## Important Notes

- These tools require an active internet connection and API access.
- The scripts use multiple free-tier API services to extend usage limits. Be aware of and respect the terms of service for each API.
- While the tool is designed to work within free tier limits, monitor your usage to avoid unexpected charges.
- The AI analysis features use OpenAI's GPT models, which may incur costs depending on your OpenAI plan.
- Performance may vary based on API availability and rate limits.


## Requirements

- Python 3
- OpenAI API key
- SerpAPI key (free tier)
- RapidAPI key (free tier)
- Various Python libraries (see `requirements.txt`)

## Installation

1. Clone the repository
2. Install required Python packages:
   ```
   pip install -r requirements.txt
   ```
3. Set up the necessary API keys as environment variables:
   ```
   export OPENAI_API_KEY='your_openai_api_key_here'
   export SERPAPI_API_KEY='your_serpapi_key_here'
   export RAPIDAPI_KEY='your_rapidapi_key_here'
   ```

## Ethical Use

These tools are powerful and should be used responsibly. Ensure you have the right to scrape or analyze any website or data source you target. Always respect copyright and terms of service of the websites and APIs you interact with.

## Disclaimer

The developers of these tools are not responsible for any misuse or for any damages that may result from the use of these tools. Use at your own risk and discretion.
 