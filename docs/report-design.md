> **Status: partly built (1 November 2026).** The report on sale since 1 November is built on this design, with two changes the founder chose: it opens with a letter grade, and its three measures are called "Named you", "Recommended you" and "Cited your website". Parts not built yet include a check of the business's own website, holding competitors to the same name rules as the business, separate choices for search and training crawlers, treating llms.txt as optional, and a way to ask for help with the tasks. This design came out of the [independent review](review-2026-10-30.md), and the text below is the reviewer's, kept as written. [How the check works](how-the-check-works.md) describes the method: the questions, the models and the counting rules.

# Owner summary + implementation brief: report vNext

Proposed contract, October 30, 2026. Version the format, measurement protocol, scoring rules and offer separately. Preserve the original evidence and terms for existing orders. Generate PDF and owner-facing web summary from the same structured report object; do not maintain independent calculations or an LLM-written summary that invents numbers.

## What the customer buys

A dated sample of how selected AI models answer relevant business-discovery questions, with evidence, a fair comparison where identities can be confirmed, and a prioritized action brief. This is not a live measurement of every customer conversation, a search-engine rank, a forecast of lost sales, or guaranteed improvement.

Keep the free check useful: three discovery questions to the current single model, a name/identity check, exact answer excerpts and cited pages, one plain-language takeaway and one next action. Show “1 of 3 answers named you” rather than a precision-looking grade from three trials. The paid offer adds broader comparable coverage, competitor evidence and prioritized owner/developer work. It does not merely add more unfamiliar model IDs.

## Part 1: the owner summary

Target: understandable in two minutes; PDF pages 1–2, with a mobile-readable equivalent on the existing protected order experience.

### Page 1: what it means and what to do first

1. Business name, website or explicit “no website supplied,” location/service area, business type, run date and coverage status. Let the buyer confirm identity before running. A namesake warning comes before a score.
2. A short conclusion drawn from measured facts: for example, “The models recognized your business when asked by name, but it rarely appeared in these customer-discovery answers.” Use only when both conditions are supported. Do not say “Google doesn't know you” merely because a Gemini response omitted the name.
3. Three plain-language measures: **Appeared**, **Recommended**, **Website cited**. Each shows its denominator and a concise definition. Recommendation labels remain secondary until calibrated; an explicit invitation metric is narrower than every natural recommendation.
4. Optional **sample visibility score** and competitive table only when the comparability conditions below pass. No letter grades, “top X%” claims, consumer market-share weights or monetary opportunity estimates without a relevant measured population.
5. Exactly three priorities, each with who acts, why this matters, evidence reference and effort band. Split owner tasks from developer tasks. If the data cannot support three specific priorities, show fewer plus honest verification tasks.
6. Scope line beside the result: “We tested model APIs. The ChatGPT, Gemini and other consumer apps can answer differently. This is a snapshot of these questions.” Link to the methodology; do not bury this only in an FAQ.

### Page 2: familiar products, differences and competitors

Use familiar labels while preserving actual measurement:

| Customer-facing group | What to show |
|---|---|
| OpenAI, company behind ChatGPT | OpenAI API results, web search on; group its two models under an expandable/appendix detail. Do not label the row “ChatGPT app tested.” |
| Claude / Anthropic | Claude API model results and observed search mode. |
| Grok / xAI | Grok model results via the actual provider, search mode recorded. |
| Perplexity | Perplexity API results and observed search mode. |
| Gemini / Google | Separate “without web search” panel under the current configuration. No inference about current Google Search, Maps or Gemini-app results. |

For each, show answered/planned questions, appearance/recommendation/citation counts, and one useful example. No unexplained Azure deployment strings on these pages. Exact provider, model ID, version, temperature, search tools, date, prompt pack, classifiers and coverage belong in the appendix.

Competitive table: **this business and confirmed competitors under the same questions/modes/identity rules**. A raw name token is insufficient for common names. If an identity cannot be confirmed, label it ambiguous and exclude it from ranking, with the exclusion visible. Unknown competitors can remain in “businesses mentioned” evidence without asserting that they are the requested business. Do not compare the client's confirmed recommendations against competitors' unconfirmed mentions.

## Comparable score specification

Implement only after AV-01/02 calibration and coverage work. Keep existing raw counts available with their old protocol version.

- Primary metric: **sample visibility = confirmed appearances in matched discovery responses**. Separate links and calibrated recommendations instead of blending arbitrary weights into one number.
- Compare web-search-enabled API runs together; retain current ungrounded Gemini results separately. These are configured modes, not permanent assertions about a provider's capabilities.
- First average binary appearance within each configured model over its answered, matched discovery question/sample cells. Then average model means using fixed, predeclared weights within each web-search provider group; finally average provider groups equally. For the two OpenAI models, each has half of OpenAI's weight regardless of how many answers returned. Never pool their raw answer counts or renormalize away a missing model. No claimed audience weighting.
- Proposed displayed score is 100 times that equally weighted mean, rounded to a whole number. All businesses use the identical eligible response set and identity standard. Explain the weighting in one sentence and expose counts underneath.
- Missing/blocked/error/budget-skipped answers are unavailable, not “not named,” and remain in planned coverage. Do not let failed models disappear from the protocol or a denominator shrink invisibly. Use matched answers for comparison and show removed/missing observations.
- Suppress a combined score/rank when identity is unresolved, a required provider/model is missing, or coverage falls below the disclosed threshold. Proposed prelaunch screen: at least 90% of planned discovery responses overall and at least 80% within every included model. These are product-quality rules to adopt before sales, not statistical confidence guarantees. Any result below 100% states the actual missing count and that the score describes available answers; missingness may bias it. Each compared business uses exactly the same actual response cells. Defer this optional composite if calibration or missing-data interpretation is not ready; matched counts remain useful.
- Avoid-type and branded recognition questions remain separate from discovery scoring. An avoid-question answer is not necessarily negative; use its actual content or mark it for review.
- Do not calculate statistical confidence as if related prompts, repeated models or providers were independent draws of customers. Do not present small before/after changes as proven uplift.
- Comparisons across dates require stable location, question/eligibility set, search mode, provider configuration and scoring version, plus matched actual question/model/sample cells across both runs. Recompute the comparison on that shared panel with its coverage shown, or suppress the delta. Unchanged configured prompts alone do not eliminate failed-call selection bias. Label methodology changes and provide raw evidence rather than an improvement claim.

### Paid deliverable completeness is a separate gate

Score eligibility covers the comparable discovery panel. It does not establish that every purchased test was delivered. The paid run manifest includes **all promised models**, including Gemini without search, and all promised question classes. Proposed new-version delivery gate: at least 90% of all promised responses answered, at least 80% within each promised model and within each promised question class, and no promised model or class absent. Round required counts upward; record actual coverage even when these gates pass. These are proposed service-quality rules, not statistical guarantees. A failed promised model triggers the disclosed partial-delivery/retry/refund process even if a grounded score can still be calculated. A partial report must never be relabeled complete merely by suppressing its score.

## Part 2: what the owner and developer should change

Start this part with a one-page checklist. Full generated files and raw answers go after it, not before it.

Every action object contains:

`action_id`, `priority`, `title`, `owner_role`, `evidence_refs`, `status` (observed / verify first / owner supplied / general guidance), `rationale`, `steps`, `page_or_system`, `acceptance_check`, `effort_band`, `dependencies`, `limitations`.

Priority is an explained judgment based on business relevance, evidence and implementation effort, not an invented numeric ROI. Code changes should have a diff or a concrete check; owner marketing tasks should name the actual source/venue where applicable.

Examples of appropriate distinctions:

- **Observed:** an answer describes a similarly named business. Owner verifies its submitted website/city and updates inconsistent owned profiles if found. Do not claim the business must rename itself.
- **Verify first:** a cited guide covers the category. Check the exact cited page and editorial/listing process before requesting inclusion. The guide may already include the business, be a competitor's own site, or offer no listing mechanism.
- **Observed after a site check:** a specified public page returns noindex or lacks a title. Developer reviews whether that is intentional, fixes the owned page, and verifies the response. Do not infer this defect from model absence alone.
- **General guidance:** verify current opening hours and service descriptions. Mark it as a checklist item unless owner/site evidence establishes an error.

### Two implementation lanes

**Owner:** confirm business facts; update owned business profiles/listings; publish useful firsthand information about services, prices, location and questions customers actually ask; review named cited sources for legitimate inclusion. No bulk review manipulation, fake testimonials or guaranteed placement. Existing verified information should not be rewritten just to inflate a checklist.

**Developer/hosting provider:** review access to the supplied public site; verify redirects/canonical URL and indexability; make important business/service text accessible; validate existing structured data against visible facts; update sitemap/internal links where an observed gap exists. Explain what can be done in a CMS editor versus what needs hosting access. Retest observable technical changes separately from running another AI sample.

### Bounded site evidence, not a new SEO crawler

Optional follow-on: to claim site-specific technical findings, add a small paid-only public check: supplied homepage, robots.txt, sitemap reference and up to two owner-selected service/about/contact pages. Budget at most six fetches total, bounded redirects/time/bytes, and an explicit fetch status. No logged-in access, headless browsing or whole-site crawling in v1. If this enhancement is deferred, fetches fail or the owner supplies no site, retain useful answer evidence and provide “verify with your developer” tasks instead of fabricated findings. It is not a blocker to testing the clearer report with customers.

HTTP fetcher must reject private/loopback/link-local/reserved IPs, metadata endpoints, credentials in URLs and unsafe ports; revalidate DNS/address/redirect destinations, including IPv6 and rebinding. Do not read private files or execute scraped instructions. Treat scraped content as untrusted evidence. Never describe a fetch from AUTX as proof of a particular provider bot's access, search indexing or ranking. Tests must cover these distinctions and SSRF defenses before enabling fetches.

### Generated files

- Drafts must be based on verified or owner-confirmed facts. Never invent awards, opening hours, prices, reviews, ratings or guarantees.
- Prefer a concise CMS-ready content outline, schema patch where appropriate, and merge instructions. Do not ask a novice to overwrite robots.txt or an existing SEO plugin's schema blindly.
- Keep missing-fact questions in a separate owner checklist; do not label REPLACE-filled files “ready to publish.” Preserve download attachments for developers who want them.
- Demote `llms.txt` to optional experimental material. Google Search says it does not use llms.txt; it is not a required repair for Google's generative search features. This does not establish whether another service uses it. [Google's AI optimization guidance](https://developers.google.com/search/docs/fundamentals/ai-optimization-guide)
- Distinguish search/retrieval crawler choices from training permission. Allowing training is not a prerequisite to being recommended. Use official provider references and preserve intentional restrictions. [OpenAI crawler roles](https://developers.openai.com/api/docs/bots), [Anthropic crawler roles](https://support.claude.com/en/articles/8896518-does-anthropic-crawl-data-from-the-web-and-how-can-site-owners-block-the-crawler)

## Report QA and future implementation help

Validate summary counts against retained evidence, all source/action links, PDF wrapping and accessibility, no private token leakage, no invented findings and no mixed-mode score. Render names with long/non-ASCII strings, incomplete providers, no website, ambiguous competitor, negative and positive avoid-question answers, and no useful changes. A technically sound existing website should be allowed to receive “no verified technical defect found.”

Add a private, optional “I need help implementing this” interest action on the paid report after the report itself is useful. It does not send the report to a developer or sell contact details. Measure demand first. Brokering, vendor vetting, pricing, permissioned sharing and dispute handling require a later plan; none is included in this $49 purchase.
