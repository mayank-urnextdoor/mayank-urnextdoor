<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/header-dark.svg">
  <img alt="Mayank: AI agents, MCP servers and Hindi-first retrieval. Builder of Ur Next Door, Bangalore." src="assets/header-light.svg" width="100%">
</picture>

<p align="center">
  <a href="https://urnextdoor.com">urnextdoor.com</a> ·
  <a href="https://www.linkedin.com/in/mayank-urnextdoor">LinkedIn</a> ·
  <a href="https://x.com/MayankQnAPe">X</a>
</p>

I build the plumbing that makes LLMs useful in production. That means servers that hand agents tools without handing them the keys, and retrieval that understands how India actually types, Hinglish included. By day I'm building [Ur Next Door](https://urnextdoor.com), a community platform for Indian neighbourhoods and interest groups.

## Open source

<a href="https://github.com/mayank-urnextdoor/karya-ai"><picture><source media="(prefers-color-scheme: dark)" srcset="assets/card-karya-ai-dark.svg"><img alt="karya-ai: AI agents that run customer messaging for Indian small businesses and ask the owner before anything risky" src="assets/card-karya-ai-light.svg" width="98.5%"></picture></a>

<p>
  <a href="https://github.com/mayank-urnextdoor/mcp-kit"><picture><source media="(prefers-color-scheme: dark)" srcset="assets/card-mcp-kit-dark.svg"><img alt="mcp-kit: production starter kit for MCP servers" src="assets/card-mcp-kit-light.svg" width="49%"></picture></a>
  <a href="https://github.com/mayank-urnextdoor/bharat-rag"><picture><source media="(prefers-color-scheme: dark)" srcset="assets/card-bharat-rag-dark.svg"><img alt="bharat-rag: Hindi, English and Hinglish Q&A over Indian public documents" src="assets/card-bharat-rag-light.svg" width="49%"></picture></a>
</p>
<p>
  <a href="https://github.com/mayank-urnextdoor/ai-pr-reviewer"><picture><source media="(prefers-color-scheme: dark)" srcset="assets/card-ai-pr-reviewer-dark.svg"><img alt="ai-pr-reviewer: GitHub Action that reviews pull requests with Claude" src="assets/card-ai-pr-reviewer-light.svg" width="49%"></picture></a>
  <a href="https://github.com/mayank-urnextdoor/slop-score"><picture><source media="(prefers-color-scheme: dark)" srcset="assets/card-slop-score-dark.svg"><img alt="slop-score: explainable linter for AI-sounding prose" src="assets/card-slop-score-light.svg" width="49%"></picture></a>
</p>

## See it run

A Hinglish question finds the right scheme in both English and Hindi documents:

<img alt="bharat-rag answering a Hinglish question with sources from English and Hindi documents" src="assets/demo-bharat-rag.svg" width="640">

A launch post full of stock phrases scores 96 out of 100, with every hit explained:

<img alt="slop-score report on an AI-styled launch post" src="assets/demo-slop-score.svg" width="640">

## How I build

Every number on this page comes from a real run: the test counts, the eval score, the terminal output above. Nothing is estimated.

Security is the default, not a feature. Tokens are stored hashed and carry scopes; CI jobs get the least permission they need.

India is not an edge case. Devanagari text and Hinglish queries get tested on Windows terminals too, because that's where a lot of Indian developers work.

Small beats clever. mcp-kit's core is under 1,000 lines, and you can read it in one sitting.

## Stack

<p>
  <img alt="TypeScript, Python, Node.js, PHP, MySQL, FastAPI, Docker, Linux, GitHub Actions" src="https://skillicons.dev/icons?i=ts,py,nodejs,php,mysql,fastapi,docker,linux,githubactions&perline=9" height="40">
</p>

Plus the Claude API and Model Context Protocol on the AI side.

## Try one in a minute

```bash
pip install git+https://github.com/mayank-urnextdoor/slop-score@v0.1.0
slop-score README.md
```
