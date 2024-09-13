import requests

class RagyWebSearch:
    BASE_URL = "https://api.ragy.ai/v1/search"

    def __init__(self, api_key):
        """
        Initialize the RagyWebSearchAPI with an API key.

        :param api_key: Your API key for accessing the RAGY Web Search API
        """
        self.api_key = api_key

    def search(self, query, lang="en", country="US", limit=50, timeout=2, max_snippets_length=10000,
               add_markdown=0, add_content_raw=0, add_reader=0, add_html=0):
        """
        Perform a web search using the RAGY API.

        :param query: The search query string (required).
        :param lang: The language of the search results (optional, default: 'en').
        :param country: The country code for regional search results (optional, default: 'US').
        :param limit: Maximum number of results to return (optional, default: 50).
        :param timeout: Timeout for the search request in seconds (optional, default: 2).
        :param max_snippets_length: Max length of snippets to return (optional, default: 10000).
        :param add_markdown: Whether to include markdown formatted content (optional, default: 0).
        :param add_content_raw: Whether to include raw content in response (optional, default: 0).
        :param add_reader: Whether to include raw HTML reader content (optional, default: 0).
        :param add_html: Whether to include raw HTML in response (optional, default: 0).

        :return: JSON response containing search results.
        """
        params = {
            'api_key': self.api_key,
            'q': query,
            'lang': lang,
            'country': country,
            'limit': limit,
            'timeout': timeout,
            'max_snippets_length': max_snippets_length,
            'add_markdown': add_markdown,
            'add_content_raw': add_content_raw,
            'add_reader': add_reader,
            'add_html': add_html
        }

        try:
            response = requests.get(self.BASE_URL, params=params)
            response.raise_for_status()
            return response.json()
        except requests.exceptions.RequestException as e:
            print(f"Error: {e}")
            return None
