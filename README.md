# Power LLM with Web Search

This project enables **Large Language Models (LLMs)** to operate on the latest information available on the internet. By combining web search capabilities with LLMs, it retrieves up-to-date data from web sources and generates insightful summaries. The project uses **Ollama's Llama 3.1** model to analyze and summarize content scraped from publicly available websites, making it ideal for applications that require real-time information processing.

## Features

- **Latest Information Access**: Enable LLMs to operate on the latest information available on the internet by performing live web searches.
- Perform web searches using public search engines (Google, Bing) or internal corporate search APIs.
- Retrieve and scrape content from the top 6 URLs in the search results using **BeautifulSoup**.
- Generate insightful summaries from the scraped content using **Ollama's Llama 3.1** model.

## Requirements

- Python 3.6+
- Libraries:
  - `requests`
  - `BeautifulSoup4`
  - `json`
  - `langchain_community`
  - `langchain_core`
  - `ollama`

Install the required packages with:

```bash
pip install requests beautifulsoup4 langchain_community langchain_core ollama
```

## How to Run

1. **Run the Search**: The project contains a sample API result simulating a web search for "Amey Ghate." You can modify the search query to suit your needs.

2. **Scrape Web Content**: The results of the web search are limited to the first 6 URLs. These URLs are scraped using the `requests` and `BeautifulSoup` libraries to extract their textual content.

3. **Summarization**: The scraped content is passed to **Ollama**'s **Llama 3.1** model, which generates a concise summary of the retrieved data.

## Sample Output

Given the sample web search, **Llama 3.1** will produce a summary that captures the central theme of the documents.


## Usage Notes

- Customize the web search query by changing the JSON result in the notebook or making live API calls.
- Adapt the model by adjusting the prompt or switching to different versions of the **Llama** model based on your needs.


## Future Enhancements

- Integrate real-time web search API calls for dynamic content retrieval.
- Improve error handling for non-HTML content such as PDFs.
- Expand support for additional search engines and customizable query parameters.



