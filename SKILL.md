---
name: web-search
description: Search the internet for current information using Tavily API. Use when user asks about news, prices, weather, events, or anything requiring up-to-date information.
metadata:
  require-secret: true
  require-secret-description: "Enter your Tavily API key. Get a free one (1000 searches/month) at https://tavily.com"
---

# Web Search

## Instructions

Call the `run_js` tool using `index.html` and a JSON string for `data` with the following fields:
- **query**: Required. The search query based on the user's question. Extract the key search terms.

After receiving the search results, use them to answer the user's question. Cite sources when relevant. Your response MUST BE in the SAME language as the user's original prompt.
