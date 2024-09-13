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

