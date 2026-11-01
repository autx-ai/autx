# How the AUTX AI Visibility Check works

This page is a copy of [autx.ai/how-it-works](https://autx.ai/how-it-works/) as of 1 November 2026 (question set version 2026-10-31). The page on autx.ai is the current version.

## What we ask, which models we ask, and how we count

We ask AI models the questions your customers ask and read every answer. This page lists every question and every rule.

## Three results, counted apart

A mention alone can flatter you, because a place in a list of rivals is not a recommendation.

- **Named.** The answer names your business, and something in it ties the name to you.
- **Recommended.** The answer tells the customer to go to you. This result sends people your way, and it is rarer.
- **Cited your website.** Your website shows up in the answer or its sources.

Every count comes with the number of answers behind it, for example recommended in 2 of 13 answers and named in 5 of 13. The gap between named and recommended tends to be the finding.

## The grade

Your AI visibility grade: a letter from A to F and a score out of 100. Like a credit score, it sums up a lot of detail in one number. It is a snapshot of the answers on the day we ask. The score weighs the three results: named 50%, recommended 35% and cited your website 15%. We work out each model's share of its answers to the questions in your set that do not name you, average the models from one company so each company counts once, then average the companies. Gemini 3.5 Flash-Lite is asked without web search, so the grade leaves it out, but the report still shows its answers and counts.

A is 80 or more, B is 60 or more, C is 40 or more, D is 20 or more, and F is below 20. When you give no website, the website result drops out, and named and recommended make up the whole score: 59 percent and 41 percent. A report gets no grade when it is incomplete, or when a model with web search answered none of the questions in your set that do not name you. The free check has no grade, because answers from one model are too few to grade.

## Your strengths

You can list up to three things you want to be known for, such as outdoor seating or vegan pastries. For each one we ask a question that does not name you, such as "Which coffee shop in Austin, TX is best for outdoor seating?" We count all three results by the same rules we use for the other questions. Google says the top restaurant details people ask AI Mode about in follow-up questions include outdoor seating, vegan or vegetarian options, live music and whether dogs are welcome. ([Google, How people are using AI Mode in the U.S.](https://services.google.com/fh/files/blogs/ai_mode_us_insights.pdf), page 24.) We do not test Google AI Mode itself.

Your strengths are your own picks, so their answers get their own section and stay out of the grade and the headline figures. The sites they cite count toward the sites to pursue.

## Where the answers come from

Models with web search build their answers from the pages they find, so the businesses those pages name tend to show up in the answers. Those pages are often guides, review sites and lists, not a business's own website. The report names the sites the models cited for your type of business and your city, so you know where to get listed and reviewed. The fix kit covers your own website.

## If your name is shared, the numbers lie

We learned this on ourselves. An early run counted our company, AUTX, as visible in a third of answers. The answers described a defunct stock ticker, an autotransformer and a fiber that share the name. Our real visibility was zero.

So we ask each model what your name means, and count a mention only when something in the answer ties the name to your business. Name collisions get their own line and stay out of your numbers.

## What the report does not promise

No ranking change by any date. Answers vary between runs. The report states what the models said and what their sources support, and running the check again later is how you see movement. Anyone who promises a ranking is guessing.

## Models

- Free check: GPT-6 Luna (Azure) with web search on. The first three questions of your set, one question for each strength you list, and the name check.
- Full report: Claude Sonnet 5.5, GPT-6.1 Sol (Azure), GPT-6 Luna (Azure), Grok 4.7 (Azure), Muse Spark 1.3 (Azure), DeepSeek V4 Pro (Azure), Gemini 3.5 Flash-Lite and Perplexity Sonar, with web search on for every model except Gemini 3.5 Flash-Lite. Every question in your set, one question for each strength you list, and the name check. Each model answers each question once.
- Without web search: Gemini 3.5 Flash-Lite answers from what it learned in training, so it gives no sources and shows your website only if it learned the address.

We ask each model through its developer API, with web search on for every model except Google's Gemini. The ChatGPT, Claude, Gemini, Grok, Meta AI, DeepSeek and Perplexity apps can answer differently, and AUTX does not measure any app.

## Question sets

Each set holds the questions a customer asks close to choosing a business. Some questions do not name you; the others do. We fill in your type of business, your city (or "your area" when you give none), your name and the strengths you list. A strength that starts with "best for" gets the "best for" form (best for remote work). Any other strength that starts with "best" or "the best" gets the "has the best" form (best espresso). Common descriptions such as dog friendly, family owned, open late or vegan get the "is" form. Every other strength gets the "best for" form. Your results show the exact question we asked. Question set version 2026-10-31.

### Shops, cafés, restaurants, salons, gyms and studios (question set `storefront`)

Questions that do not name you (15):

- What is the best {category} in {location}?
- Which {category} in {location} would you recommend?
- What {category} in {location} should I try this weekend?
- Which {category} in {location} has the best reviews?
- What is the most popular {category} in {location} right now?
- Which {category} in {location} do locals love?
- Which {category} in {location} is the best value for the money?
- Which {category} in {location} has the best atmosphere?
- What is a hidden gem {category} in {location}?
- Which {category} in {location} is worth the hype?
- Which new {category} in {location} is worth trying?
- I'm new to {location}. Which {category} should I go to?
- Which {category} in {location} has the friendliest staff?
- Which {category} in {location} should I avoid?
- What are the warning signs of a bad {category}?

Questions about you by name (5):

- Is {brand} a good {category} in {location}?
- What do people say about {brand}?
- Are there any complaints about {brand}?
- Is {brand} worth the price?
- What is {brand} known for?

One question for each strength you list, in the form that fits it:

- Which {category} in {location} is best for {strength}?
- Which {category} in {location} is {strength}?
- Which {category} in {location} has the best {strength}?

### Trades and home services (question set `local`)

Questions that do not name you (15):

- Who are the best {category} companies in {location}?
- I need {category} in {location}. Who should I call first?
- What should I look for when hiring a {category} company in {location}?
- Who are the most trusted {category} providers near {location}?
- Compare the top {category} companies in {location}.
- What does {category} typically cost in {location}?
- Which {category} companies in {location} have the best reviews?
- Who is the largest {category} provider in {location}?
- What questions should I ask a {category} contractor before signing?
- Which {category} companies in {location} offer emergency service?
- What are the red flags when choosing a {category} company?
- Who has been doing {category} in {location} the longest?
- Recommend a {category} company for a small business in {location}.
- What is the difference between the top {category} providers in {location}?
- Who should I avoid when hiring for {category} in {location}?

Questions about you by name (5):

- Is {brand} a good choice for {category} in {location}?
- What do people say about {brand}?
- Are there any complaints about {brand}?
- I got a quote from {brand}. Is that a fair price?
- Is {brand} licensed and insured?

One question for each strength you list, in the form that fits it:

- Which {category} companies in {location} are best for {strength}?
- Which {category} companies in {location} are {strength}?
- Which {category} company in {location} has the best {strength}?

### Professional services (question set `professional`)

Questions that do not name you (15):

- Who are the best {category} firms in {location}?
- How do I choose a {category} provider?
- What should {category} services cost?
- Which {category} firms work with small businesses?
- Compare the leading {category} providers in {location}.
- What credentials should a {category} provider have?
- Who is the most experienced {category} provider in {location}?
- What questions should I ask before hiring a {category} firm?
- Which {category} providers offer a free consultation?
- What are the warning signs of a bad {category} provider?
- Recommend a {category} firm for a startup.
- How long does {category} work usually take?
- Which {category} firms specialize in my industry?
- Is it better to use a large or boutique {category} firm?
- Which {category} provider gives the best value?

Questions about you by name (5):

- Is {brand} reputable?
- What do clients say about {brand}?
- Are there any complaints about {brand}?
- What does {brand} specialize in?
- Who are the alternatives to {brand}?

One question for each strength you list, in the form that fits it:

- Which {category} firms in {location} are best for {strength}?
- Which {category} firms in {location} are {strength}?
- Which {category} firm in {location} has the best {strength}?

### Online stores and brands (question set `ecommerce`)

Questions that do not name you (15):

- Where is the best place to buy {category} online?
- What are the best {category} brands?
- Which {category} brand has the best quality?
- What is the best value {category} brand?
- Compare the top {category} brands.
- Which {category} brands ship fastest?
- What are the best-reviewed {category} products this year?
- Which {category} brand has the best return policy?
- What is a good alternative to the most popular {category} brand?
- Which {category} brands are made in the United States?
- What should I look for when shopping for {category}?
- Which {category} brand is best for beginners?
- What is the most recommended {category} brand?
- Which {category} brands offer a warranty?
- Which {category} brands do experts recommend?

Questions about you by name (5):

- Is {brand} a legitimate company?
- What do reviews say about {brand}?
- Is {brand} worth the price?
- Are there any complaints about {brand}?
- Is it safe to order from {brand}?

One question for each strength you list, in the form that fits it:

- Which {category} brand is best for {strength}?
- Which {category} brands are {strength}?
- Which {category} brand has the best {strength}?

### Software and apps (question set `saas`)

Questions that do not name you (14):

- What is the best {category} tool?
- What are the top alternatives to the leading {category} software?
- Compare the best {category} tools for a small team.
- What is the cheapest good {category} tool?
- Which {category} tool is best for a solo founder?
- What {category} tool should I use if I am just starting out?
- Which {category} tools have the best free tier?
- What is the most popular {category} software right now?
- Which {category} tool integrates best with existing workflows?
- What are people switching to instead of the market leader in {category}?
- Which {category} tool has the best support?
- What should I know before buying a {category} tool?
- Which {category} tools are built for enterprise versus small business?
- What is the fastest {category} tool to set up?

Questions about you by name (6):

- Is {brand} worth it?
- What do users say about {brand}?
- What are the downsides of {brand}?
- Is {brand} better than its competitors?
- Is {brand} still actively maintained?
- How does {brand} pricing compare to alternatives?

One question for each strength you list, in the form that fits it:

- What is the best {category} tool for {strength}?
- Which {category} tools are {strength}?
- Which {category} tool has the best {strength}?

### Name check

Every run also asks:

- What is {brand}?

## How we count an answer

### Matching

We compare names after folding the text: curly and straight apostrophes count as the same, "&" counts as "and", case does not matter, and a name has to match as whole words, so "roof" does not match "roofing". Quotes keep the original text.

### Named

An answer to a question that does not name you must use your name as a name. A name that is not an everyday English word (Saatva, Casper) counts wherever it appears. A name that is an everyday word (Purple, Simple) counts when the answer uses it as a name: with its capital letter inside a sentence; in bold, as a link or alone on its line; as a label ("Purple:"); followed by a possessive, a product name or other brand names; or opening a sentence about it that also gives your city, your website or a word from your type of business outside the name's own phrase. A name of several words counts when it keeps its capital letters. For an online store or software business, the rules above are enough. A business with a city (a shop, café, salon, gym, studio, trade or professional service) also needs its city or website in the answer, or a word from your type of business in a sentence that names you. Questions about you by name and the name check already give your name, so there the answer must tie it to you instead: your website, your city, a word from your type of business in a sentence that names you, or two different words from it anywhere. When your type of business is one word, an answer about you by name may have that word anywhere, when it uses your name as a name. When every word of your name is a word from your type of business (for example, Blank Apparel selling blank apparel), only your website, or your name written closed up as in a web address, counts.

### Recommended

An answer recommends you when it tells the customer to go to you. A word such as "try", "use", "visit", "head to", "consider", "check out" or "go with" has to open a clause and come before your name in the same sentence, and "I recommend", "we suggest" and "your best bet is" count too. We reject the sentence when "instead of", "alternatives to", "rather than", "complaints about" or similar words sit between the verb and your name, or when "not", "never", "avoid" or "don't" comes right before the verb. A recommendation counts only when the same answer also names you under the rule above.

### Cited your website

An answer cites your website when your domain, or a subdomain of it, appears in the answer or in its sources. When you give no domain, we leave this result out and say so.

### Name collisions

When the model says your name points to more than one thing and the answer does not give your website, we count a collision and do not count the mention. The name check reports one of: confirmed, collision, mixed, unconfirmed, not named or no answer. When some answers count as a collision but more answers describe your business, it reads mixed, not collision.

### Headline figures

All three headline figures use only the questions that do not name you, so a question that already names you cannot raise your numbers. Questions about you by name and the name check feed the name check section. Every figure leaves out failed calls, and each count comes with the number of answers behind it. Questions that ask what to avoid or what warning signs to look for sit outside every figure, because a mention there is no win. A report quotes each answer to them that names you, in its own section. Strength questions do not name you either, but they sit outside the headline figures and the grade, in their own section.

### Sites to pursue

We list the sites cited in answers to questions that do not name you, strength questions included. We skip an answer that uses your name without tying it to you, or says the name points to more than one thing. We also list the sites cited in answers about you by name that we could tie to you. Answers to the questions about what to avoid add no sites, because a site cited there may be a complaints site. We drop your own site and its subdomains, the sites of competitors you list, and general sites such as wikipedia.org, google.com and youtube.com.

### Complete or incomplete

The free check counts as complete when at least 2 of its first three questions get an answer. Strength questions do not count toward this. A full report counts as complete when at least 60% of all its planned calls come back (a call is one question to one model). We then leave out any model that got the questions that do not name you but answered none of them. Of the calls to the other models, at least 90% must also come back, and at least 80% within each of those models and within each kind of question. A call we skip because the run hit its spending cap counts as not answered. When a model takes more than 60 seconds to answer a call, we ask it again. If a report is still incomplete, we keep the answers that came back and later ask again only the calls that got none. A model may get the questions in your set that do not name you but answer none of them. We ask it again at the next try. If it answers none again, we send the report without it and offer a refund. If we cannot complete a full report within 24 hours, we refund your order in full.

## Noise

Models answer the same question differently from run to run. One run is a sample, not a census, so read a difference of one or two answers between two runs as noise. We make no ranking promise. The score can move a few points between runs, so a grade near the edge of a band can change by a letter.
