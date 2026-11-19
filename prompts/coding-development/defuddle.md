# defuddle

**Category:** Coding & Development  
**Source:** prompts.chat

## Prompt

> ---
> name: defuddle
> description: Extract clean Markdown from HTML pages with Defuddle CLI.
> ---
> 
> # Defuddle
> 
> Use Defuddle CLI to extract clean readable content from web pages. Prefer over WebFetch for standard web pages — it removes navigation, ads, and clutter, reducing token usage.
> 
> If not installed: `npm install -g defuddle`
> 
> ## Usage
> 
> Always use `--md` for markdown output:
> 
> ```bash
> defuddle parse <url> --md
> ```
> 
> Save to file:
> 
> ```bash
> defuddle parse <url> --md -o content.md
> ```
> 
> Extract specific metadata:
> 
> ```bash
> defuddle parse <url> -p title
> defuddle parse <url> -p description
> defuddle parse <url> -p domain
> ```
> 
> ## Output formats
> 
> | Flag | Format |
> |------|--------|
> | `--md` | Markdown (default choice) |
> | `--json` | JSON with both HTML and markdown |
> | (none) | HTML |
> | `-p <name>` | Specific metadata property |
> 
> FILE:LICENSE
> MIT License
> 
> Copyright (c) 2026 Steph Ango (@kepano)
> 
> Source: https://github.com/kepano/obsidian-skills
> 
> Permission is hereby granted, free of charge, to any person obtaining a copy
> of this software and associated documentation files (the "Software"), to deal
> in the Software without restriction, including without limitation the rights
> to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
> copies of the Software, and to permit persons to whom the Software is
> furnished to do so, subject to the following conditions:
> 
> The above copyright notice and this permission notice shall be included in all
> copies or substantial portions of the Software.
> 
> THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
> IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
> FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
> AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
> LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
> OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
> SOFTWARE.

---
[← Back to Coding & Development](README.md) · [Main index](../../README.md)