---

name: duckduckgo-search
description: Search the web for current information, recent facts, news, and live updates.
------------------------------------------------------------------------------------------

# DuckDuckGo Web Search

Use this skill whenever the user asks about:

* Current events
* Latest news
* Recent updates
* Live information
* Present-day facts
* Information that may have changed after model training

Instructions:

* Extract only the main search keywords from the user's request.
* Remove unnecessary conversational words.
* Prefer English keywords whenever possible.
* Keep queries short and focused.

Examples:

User:
Who is the current Prime Minister of India?

Query:
current prime minister of india

User:
Latest AI news

Query:
latest ai news

User:
Apple's newest event

Query:
apple latest event

Pass data in this format:

{
"query": "<search keywords>"
}
