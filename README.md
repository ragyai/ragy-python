# ragy-python
 Python Wrapper for the Ragy web seach and summarization api
 
 [Signup](https://www.ragy.ai/signup) (3.000 free credits a month)
 
 [Docs](https://www.ragy.ai/docs)
 
 [Website](https://www.ragy.ai/)

# Usage Example:
    api_key = "YOUR-API_KEY"
    ragy = RagyWebSearchAPI(api_key)

    # Perform a search
    result = ragy.search(query="What is Rag", lang="en", country="US", limit=50)
    print(result)

