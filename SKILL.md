---
name: web-search
description: Search the internet for current information using Tavily API. Use when user asks about news, prices, weather, events, or anything requiring up-to-date information.
metadata:
  require-secret: true
  require-secret-description: "Enter your Tavily API key. Get a free one (1000 searches/month) at https://tavily.com"
---

# Web Search

Search the live internet for up-to-date information, news, or facts.

## Examples

* "What is Tesla stock price today?"
* "Latest news about AI"
* "Weather in Tokyo"

## Instructions

You MUST use the `run_js` tool with the following exact parameters:

- data: A JSON string with the following fields:
  - query: String. The search query based on the user's question.

After receiving the search results, summarize them to answer the user's question. Always mention the source URLs in your response.
