---
name: tavily-web-search
description: Fetches live search results from the internet via Tavily API and returns them as text.
metadata:
  require-secret: true
  require-secret-description: "Enter your Tavily API key. Get a free one (1000 searches/month) at https://tavily.com"
---

# Web Search

This tool fetches real-time search results from the internet using the Tavily API.

## Examples

* "What is Tesla stock price today?"
* "Latest news about AI"
* "Weather in Tokyo"

## Instructions

You MUST use the `run_js` tool with the following exact parameters:

- data: A JSON string with the following fields:
  - query: String. The search query based on the user's question.
