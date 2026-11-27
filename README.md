<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/header-dark.svg">
  <img alt="Mayank: AI agents, MCP servers and Hindi-first retrieval. Builder of Ur Next Door, Bangalore." src="assets/header-light.svg" width="100%">
</picture>

<p align="center">
  <a href="https://urnextdoor.com">urnextdoor.com</a> ·
  <a href="https://www.linkedin.com/in/mayank-urnextdoor">LinkedIn</a> ·
  <a href="https://x.com/MayankQnAPe">X</a>
</p>

I build the plumbing that makes LLMs useful in production: servers that give agents tools safely, retrieval that works for Indian users in Hindi, English and the Hinglish in between, and checks that keep AI output honest. By day I'm building [Ur Next Door](https://urnextdoor.com), a community platform for Indian neighbourhoods, cities and interest groups.

## Open source

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

- **Numbers come from runs.** Every figure on this page (test counts, eval scores, demo output) is copied from a real run, not estimated.
- **Secure by default.** Hashed tokens with scopes, least-privilege CI permissions, untrusted input treated as untrusted.
- **India is not an edge case.** Devanagari, Hinglish and Windows terminals get tested, not assumed.
- **Small enough to read.** mcp-kit's core is under 1,000 lines. If you can't read it in one sitting, it's too big.

## Stack

<p>
  <img alt="TypeScript, Python, Node.js, PHP, MySQL, FastAPI, Docker, Linux, GitHub Actions" src="https://skillicons.dev/icons?i=ts,py,nodejs,php,mysql,fastapi,docker,linux,githubactions&perline=9" height="40">
</p>

Plus the Claude API, Model Context Protocol, and hybrid BM25 + dense retrieval.

## Try one in a minute

```bash
pip install git+https://github.com/mayank-urnextdoor/slop-score@v0.1.0
slop-score README.md
```
