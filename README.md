# ragy-python
 A simple Python wrapper for the Ragy web seach and summarization api
 
 [Signup](https://www.ragy.ai/signup) (3.000 free credits a month) (or [Rapidapi](https://rapidapi.com/pschinkel80/api/ragy-search) )
 
 [Docs](https://www.ragy.ai/docs)
 
 [Website](https://www.ragy.ai/)

# Usage Example:
import ragy-python

api_key = "YOUR-API_KEY"
ragy = RagyWebSearch(api_key)

result = ragy.search(query="What is Rag", lang="en", country="US", limit=50)
print(result)

## Example search params:
* query: The search query string (required).
* lang: The language of the search results (optional, default: 'en').
* country: The country code for regional search results (optional, default: 'US').
* limit: Maximum number of results to return (optional, default: 50).
* timeout: Timeout for the search request in seconds (optional, default: 2).
* max_snippets_length: Max length of snippets to return (optional, default: 10000).
* add_markdown: Whether to include markdown formatted content (optional, default: 0).
* add_content_raw: Whether to include raw content in response (optional, default: 0).
* add_reader: Whether to include raw HTML reader content (optional, default: 0).
* add_html: Whether to include raw HTML in response (optional, default: 0).

