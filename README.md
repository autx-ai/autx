# AUTX

AUTX makes AI products and services. Website: [autx.ai](https://autx.ai).

Here, AUTX means AUTX DAO LLC, the Wyoming company at autx.ai. It is not related to other products, stock tickers or parts that share the name.

## AUTX AI Visibility Check

AI assistants can only recommend businesses they can read about. The AUTX AI Visibility Check asks AI models the questions customers ask before they choose a business. It reports whether the answers name the business, recommend it and cite its website, and which other sites the models cite.

- **Free check.** Three customer questions and one for each strength the owner lists (up to three, such as outdoor seating), put to one OpenAI model with web search on, plus a name check. About a minute, with no signup and no email. [Check a business at autx.ai](https://autx.ai/).
- **AUTX AI Visibility Report, $49, paid once.** Every question in the set for the business type, put to eight AI models from OpenAI, Anthropic, Google, Meta, xAI, DeepSeek and Perplexity. The PDF opens with a letter grade from A to F and a score out of 100 when enough answers come back to grade it. It shows how often each model named the business, recommended it and cited its website, how often the competitors the owner lists came up, and which sites the models cited most. It also has a name check and a fix kit of draft files for the business's website.
- **Sample report.** A real report for a coffee shop in Austin, TX, with the shop's name hidden: [autx.ai/sample-report](https://autx.ai/sample-report/).
- **AUTX's own grade.** AUTX ran the full report on itself on November 9, 2026, and published the result, grade included: [autx.ai/our-grade](https://autx.ai/our-grade/). It will run the report again every month.
- **Study: Who does AI pick?** AUTX asked eight AI models questions such as "What is the best coffee shop in Chicago?" for six kinds of local business in five US cities on November 1, 2026. The study shows which businesses the models named, how often they agreed and which sites they cited, with the data: [autx.ai/studies/who-does-ai-pick](https://autx.ai/studies/who-does-ai-pick/).
- **Questions and answers.** What the free check and the report cover, which AI models each one asks, refunds, privacy and how AI assistants pick businesses: [autx.ai/faq](https://autx.ai/faq/).

### What the check counts

- **Three results, counted apart.** Named the business, recommended it and cited its website. Each count comes with the number of answers behind it, for example recommended in 2 of 13 answers and named in 5 of 13.
- **A grade from A to F.** The score out of 100 weighs the three results from the questions that do not name the business: named 50%, recommended 35% and cited its website 15%. A is 80 or more, B is 60 or more, C is 40 or more, D is 20 or more, and F is below 20.
- **Eight models.** Seven answer with web search on: Claude Sonnet 5.5, GPT-6.1 Sol, GPT-6 Luna, Grok 4.7, Muse Spark 1.3, DeepSeek V4 Pro and Perplexity Sonar. Gemini 3.5 Flash-Lite answers without web search, from what it learned in training, so the grade leaves it out.
- **Developer APIs, not apps.** We ask each model through its developer API. Consumer chat apps can answer differently, and AUTX does not measure them.
- **Names have to match the business.** A mention counts only when something in the answer ties the name to the business. Name collisions stay out of the numbers. We learned this on ourselves: an early run counted AUTX as visible in a third of answers, and those answers described other things named AUTX.
- **No ranking promise.** Answers change from run to run, so a report is a sample. Its score can move a few points between runs, and a grade near the edge of a band can change by a letter.

More on what we ask, which models we ask and what the grade means: [docs/how-the-check-works.md](docs/how-the-check-works.md), or [autx.ai/how-it-works](https://autx.ai/how-it-works/).

## Documents

| Document | What it covers |
|---|---|
| [How the check works](docs/how-the-check-works.md) | What we ask, which models we ask and what the grade means |
| [Changelog](CHANGELOG.md) | What changed for customers, by date |

## For developers

AUTX built and ran a production x402 payment gateway, and offers x402 integration and audit services: [autx.ai/x402](https://autx.ai/x402/).

## History

Before the check, AUTX built a marketplace for AI agents. AUTX froze the marketplace in July 2026 and shut it down in August 2026. The public repositories [blog](https://github.com/autx-ai/blog), [agent-summarizer](https://github.com/autx-ai/agent-summarizer) and [agent-docreader](https://github.com/autx-ai/agent-docreader) come from that period.

## Contact

Email [sales@autx.ai](mailto:sales@autx.ai). AUTX on X: [@autxdotai](https://x.com/autxdotai). [About AUTX](https://autx.ai/about/).

## About this repository

AUTX keeps its product code private. This repository holds the public documents about what AUTX does and what the grade means, so that people and AI systems can read them. The [terms of service](https://autx.ai/terms/) cover how anyone may use them.
