# How the AUTX AI Visibility Check works

This document is a copy of [autx.ai/how-it-works](https://autx.ai/how-it-works/) as of November 11, 2026. The page on autx.ai is the current version.

## What we ask, which models we ask, and what the grade means

We ask AI models the questions your customers ask and read every answer. This page explains what we count, which models we ask and what the grade means.

## Three results, counted apart

A mention alone can flatter you, because a place in a list of rivals is not a recommendation.

- **Named.** The answer names your business, and something in it ties the name to you.
- **Recommended.** The answer tells the customer to go to you. This result sends people your way, and it is rarer.
- **Cited your website.** Your website shows up in the answer or its sources.

Every count comes with the number of answers behind it, for example recommended in 2 of 13 answers and named in 5 of 13. The gap between named and recommended tends to be the finding.

## The grade

Your AI visibility grade: a letter from A to F and a score out of 100. Like a credit score, it sums up a lot of detail in one number. It is a snapshot of the answers on the day we ask. The score weighs the three results from the questions that do not name you: named 50%, recommended 35% and cited your website 15%. We work out each model's share of its answers, average the models from one company so each company counts once, then average the companies. We ask Gemini 3.5 Flash-Lite without web search, so the grade leaves it out, but the report still shows its answers and counts.

A is 80 or more, B is 60 or more, C is 40 or more, D is 20 or more, and F is below 20. When you give no website, the grade uses the other two results, named and recommended. A report gets no grade when it is incomplete, or when a model with web search answered none of the questions in your set that do not name you. If we cannot complete a full report within 24 hours, we refund your order in full. The free check has no grade, because answers from one model are too few to grade.

## Your strengths

You can list up to three things you want to be known for, such as outdoor seating or vegan pastries. For each one we ask a question that does not name you, such as "Which coffee shop in Austin, TX is best for outdoor seating?" We count all three results by the same rules we use for the other questions. Google says the top restaurant details people ask AI Mode about in follow-up questions include outdoor seating, vegan or vegetarian options, live music and whether dogs are welcome. ([Google, How people are using AI Mode in the U.S.](https://services.google.com/fh/files/blogs/ai_mode_us_insights.pdf), page 24.) We do not test Google AI Mode itself.

Your strengths are your own picks, so their answers get their own section and stay out of the grade and the headline figures. The sites they cite count toward the sites to pursue.

## Where the answers come from

Models with web search build their answers from the pages they find, so the businesses those pages name tend to show up in the answers. Those pages are often guides, review sites and lists, not a business's own website. The report names the sites the models cited for your type of business and your city, so you know where to get listed and reviewed. The fix kit covers your own website.

## If your name is shared, the numbers lie

We learned this on ourselves. An early run counted our company, AUTX, as visible in a third of answers. The answers described a defunct stock ticker, an autotransformer and a fiber that share the name. Our real visibility was zero.

So we ask each model what your name means, and count a mention only when something in the answer ties the name to your business. Name collisions get their own line and stay out of your numbers.

## The questions

Each type of business has its own set of questions. They are the questions a customer asks close to choosing a business, with your type of business and your city filled in. Most do not name you, and a few ask about you by name. For a coffee shop in Austin, TX, three of them are:

- What is the best coffee shop in Austin, TX?
- Which coffee shop in Austin, TX would you recommend?
- What coffee shop in Austin, TX should I try this weekend?

Your results show the exact question behind each answer.

## How we read an answer

Software reads every answer and applies the same rules to every business. A name counts only when the answer ties it to you. A recommendation means the answer tells the customer to go to you. A citation means your website is in the answer or its sources. Other things that share your name stay out of your numbers.

Software can misread an answer. If a number in your report looks wrong, email sales@autx.ai with your order reference, and we will explain it.

## What the report does not promise

No ranking change by any date. Answers vary between runs. The report states what the models said and what their sources support, and running the check again later is how you see movement. Anyone who promises a ranking is guessing.

## Models

- **Free check:** GPT-6 Luna (Azure) with web search on. The first three questions of your set, one question for each strength you list, and the name check.
- **Full report:** Claude Sonnet 5.5, GPT-6.1 Sol (Azure), GPT-6 Luna (Azure), Grok 4.7 (Azure), Muse Spark 1.3 (Azure), DeepSeek V4 Pro (Azure), Gemini 3.5 Flash-Lite and Perplexity Sonar, with web search on for every model except Gemini 3.5 Flash-Lite. Every question in your set, one question for each strength you list, and the name check. Each model answers each question once.
- **Without web search:** Gemini 3.5 Flash-Lite answers from what it learned in training, so it gives no sources and shows your website only if it learned the address.

We ask each model through its developer API, with web search on for every model except Google's Gemini. The ChatGPT, Claude, Gemini, Grok, Meta AI, DeepSeek and Perplexity apps can answer differently, and AUTX does not measure any app.

## Noise

Models answer the same question differently from run to run. One run is a sample, not a census, so read a difference of one or two answers between two runs as noise. We make no ranking promise. The score can move a few points between runs, so a grade near the edge of a band can change by a letter.
