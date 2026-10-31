# AUTX

AUTX makes AI products and services. Website: [autx.ai](https://autx.ai).

Here, AUTX means AUTX DAO LLC, the Wyoming company at autx.ai. It is not related to other products, stock tickers or parts that share the name.

## AUTX AI Visibility Check

More customers ask AI assistants where to eat, shop, train or book. Those assistants can only recommend businesses they can read about. The AUTX AI Visibility Check shows a business what AI models say about it today, and where to put content about what it does best.

- **Free check.** Three questions a business's customers ask, put to one OpenAI model with web search on, plus a name check. About a minute, with no signup and no email. [Check a business at autx.ai](https://autx.ai/).
- **AUTX AI Visibility Report, $49, one time.** Every question in the business's question set, put to six AI models from OpenAI, Anthropic, Google, xAI and Perplexity. The PDF shows how often each model names, recommends and links the business, how often the competitors the owner lists come up, and which sites the models cite. It also includes a name check and a fix kit of draft files for the business's website.
- **Sample report.** A real report for an Austin coffee shop, with its name, website and address hidden: [autx.ai/sample-report](https://autx.ai/sample-report/).

### How it measures

- **Three results, counted apart.** Named, recommended and linked. Each count comes with the number of answers behind it, for example recommended in 2 of 13 answers and named in 5 of 13.
- **Six models.** GPT-6.1 Sol and GPT-6 Luna on Azure OpenAI, Grok 4.7 on Azure AI Foundry, Claude and Perplexity Sonar answer with web search on. Gemini 3.8 Flash answers without web search, from what it learned in training.
- **Developer APIs, not apps.** We ask each model through its developer API. The ChatGPT, Claude, Gemini, Grok and Perplexity apps can answer differently, and AUTX does not measure any app.
- **Names have to match the business.** A mention counts only when something in the answer ties the name to the business. Name collisions stay out of the numbers. We learned this on ourselves: an early run counted AUTX as visible in a third of answers, and those answers described other things named AUTX.
- **No ranking promise.** Answers change from run to run, so a report is a sample. Its score can move a few points between runs, and a grade near the edge of a band can change by a letter.

The full method, with every question and every counting rule: [docs/how-the-check-works.md](docs/how-the-check-works.md), or [autx.ai/how-it-works](https://autx.ai/how-it-works/).

## Documents

| Document | What it covers |
|---|---|
| [How the check works](docs/how-the-check-works.md) | The questions, the models and how we count every answer |
| [Independent review, 30 October 2026](docs/review-2026-10-30.md) | What an outside review found, and what we fixed |
| [Report design](docs/report-design.md) | The planned two-part report: an owner summary, then actions backed by evidence |
| [Roadmap](docs/roadmap.md) | What is live and what comes next |
| [Changelog](CHANGELOG.md) | What shipped, by date |

## For developers

AUTX built and ran a production x402 payment gateway, and offers x402 integration and audit services: [autx.ai/x402](https://autx.ai/x402/).

## History

AUTX first built a marketplace for AI agents. AUTX froze the marketplace in July 2026 and shut it down in August 2026. The public repositories [blog](https://github.com/autx-ai/blog), [agent-summarizer](https://github.com/autx-ai/agent-summarizer) and [agent-docreader](https://github.com/autx-ai/agent-docreader) come from that period.

## Contact

[sales@autx.ai](mailto:sales@autx.ai) · X: [@autxdotai](https://x.com/autxdotai) · [About AUTX](https://autx.ai/about/)

## About this repository

AUTX keeps its product code private. This repository holds the public documents about what AUTX does and how it measures, so that people and AI systems can read them.
