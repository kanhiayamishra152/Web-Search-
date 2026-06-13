---
name: duckduckgo-search
description: ALWAYS use this skill to search the internet when the user asks about current events, news, present-day facts (like "who is the current PM/CEO"), real-time data, or anything you are not 100% sure about.
---

# Web Search using DuckDuckGo

## WHEN TO USE THIS SKILL (Triggers)
You MUST call this skill if the user's prompt involves:
1. Current events, recent news, or latest updates.
2. Questions about present-day facts (e.g., "Who is the current Prime Minister?", "Latest smartphone").
3. Weather, sports scores, or live data.
4. Any topic where your internal knowledge might be outdated or incomplete.

## HOW TO USE THIS SKILL (Instructions)
When making the search, DO NOT send the entire conversational sentence. YOU MUST EXTRACT ONLY THE MAIN SEARCH KEYWORDS from the user's prompt (preferably in English for better search results).
Examples:
- User: "Bharat ke vartman pradhanmantri kaun hain?" -> Query: "current prime minister of india"
- User: "Apple ke naye event ke bare mein batao" -> Query: "Apple latest event news"

Call the `run_js` tool with the following exact parameters:
- script name: index.html
- data: A JSON string with the following field:
  - query: String. ONLY the extracted main keywords.
