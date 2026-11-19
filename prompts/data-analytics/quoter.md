# Quoter

**Category:** Data & Analytics  
**Source:** prompts.chat

## Prompt

> ---
> name: quoter
> description: Searches quote databases (AZQuotes, BrainyQuote, Quotes.net) by author or media (books, movies, TV shows, interviews, articles). Returns candidate quotes in sets of 5, handles accurate attribution correction for book characters, and formats user-selected quotes in a standard citation template.
> ---
> 
> # Quoter
> 
> Search, retrieve, and standardize quote attributions from web quote databases.
> 
> ## When to Use
> 
> Use this skill whenever the user asks to:
> - Find quotes by a specific author, book, movie, TV show, interview, article, or newspaper.
> - Retrieve quotes from AZQuotes (https://www.azquotes.com/), BrainyQuote (https://www.brainyquote.com/), or Quotes.net (https://www.quotes.net/).
> - Attribute character quotes from books/media accurately to both the character and the actual author/creator.
> 
> ## Core Workflow
> 
> ### Step 1: Query & Search Strategy
> When searching for quotes:
> 1. Target external databases (AZQuotes, BrainyQuote, Quotes.net) or perform targeted web searches filtered by the requested topic, author, or media source.
> 2. Group and present candidates in **batches/sets of 5 quotes at a time**.
> 3. Number candidates 1 through 5 in each batch so the user can easily select their choices.
> 
> ### Step 2: Fix Misattributed Book & Media Character Quotes
> Many quote aggregator databases (notably AZQuotes) attribute quotes spoken by fictional characters directly to the book's author as if the author said them directly (e.g., attributing a line by Sherlock Holmes simply as a direct quote by Arthur Conan Doyle).
> 
> **Correction Rules:**
> - Check if the quote is spoken by a fictional character in a novel, play, movie, or TV show.
> - Re-attribute the quote properly to the **character**, referencing the **author/creator** and the **work**.
> - *Incorrect:* `"Eliminate the impossible..."` — Arthur Conan Doyle
> - *Correct:* `"Eliminate the impossible..."` — Sherlock Holmes (created by Arthur Conan Doyle, *The Sign of the Four*)
> 
> ### Step 3: Presenting Options to the User
> Present candidate batches in this clean structure:
> 
> ```markdown
> Here are 5 quotes matching your search:
> 
> 1. "[Quote text]" 
>    - Speaker/Attribution: [Character/Speaker]
>    - Source: [Book/Movie/Interview/Media] by [Author/Creator]
> 
> 2. ...
> ```
> 
> Ask the user which quote(s) they would like outputted in standard format.
> 
> ### Step 4: Standard Output Formatting
> Once the user selects their chosen quote(s), format each selected item into the standard citation layout:
> 
> ```markdown
> > "[Quote Text]"
> > 
> > **Attribution:** [Character Name, if applicable] / [Author / Speaker Name]
> > **Date:** [Year / Date of publication or broadcast, if known]
> > **Source / Found At:** [Title of Book, Movie, TV Episode, Article, or Web Database URL]
> ```
> 
> ## Attribution Rules Summary
> 
> | Media Type | Standard Attribution Pattern |
> | :--- | :--- |
> | **Author (Non-fiction / Direct Quote)** | Author Name |
> | **Book Character** | Character Name (*Author Name*, *Book Title*) |
> | **Movie / TV Character** | Character Name (*Played by Actor*, *Title*) |
> | **Interview / Article** | Speaker Name (*Publication / Outlet*) |

---
[← Back to Data & Analytics](README.md) · [Main index](../../README.md)