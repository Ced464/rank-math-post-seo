---
name: rank-math-post-seo
description: Research, draft, optimize, and audit WordPress blog posts for Rank Math SEO. Use when creating or revising posts, selecting a focus keyword, preparing an SEO title/meta description/slug, improving headings, images, links, readability, or checking Rank Math recommendations without sacrificing helpfulness or natural writing.
metadata:
  version: "1.0.0"
  language: "en"
---

# Rank Math SEO Post Writer

## Purpose

Create useful, well-researched, search-intent-matched WordPress posts and prepare the post-level fields used by Rank Math SEO. Optimize for readers first; use Rank Math as a diagnostic checklist, not as a ranking guarantee. Follow the rules in `references/seo-rules-and-sources.md` when a recommendation appears to conflict with user value or search-engine guidance.

## Non-negotiable principles

1. **People-first, search-intent-first.** Answer the reader's real question with accurate, specific, original information. Do not pad an article just to meet a word count.
2. **No keyword stuffing.** Use the main phrase where it naturally belongs and use relevant variants, synonyms, entities, and questions. Never make sentences awkward to force an exact match.
3. **Never fabricate.** Do not invent first-hand experience, product tests, statistics, quotes, case studies, author credentials, citations, source URLs, or features. Research factual/current claims when web access is available and cite material claims with trustworthy sources.
4. **Do not treat every Rank Math test as a Google ranking factor.** Sentiment words, power words, title numbers, an exact keyword-density target, and a required TOC/media count are plugin heuristics or editorial choices, not universal ranking requirements.
5. **Links must be editorially justified.** Do not add irrelevant external/internal links only to turn a test green. Do not make paid or affiliate links followed simply to satisfy Rank Math.
6. **Be transparent about limitations.** If the site’s URL inventory, current Rank Math score, post editor, Content AI, or WordPress access is unavailable, do not claim to have checked it. Provide suggested targets and a checklist instead.

## Inputs and defaults

Use the details the user supplies: topic/draft, intended audience, target market/language, website or brand, preferred tone, focus keyword, word range, internal pages, and source requirements.

- If a focus keyword is supplied, preserve its intended meaning and validate that it matches the post's search intent.
- If none is supplied, research/select one primary query and a small set of supporting terms; state any material assumptions. Do not stop for clarification unless an essential ambiguity makes the result unreliable.
- If no word count is supplied, choose a length that answers the query completely. For a typical informational post, use **600 words as a Rank Math-oriented baseline only**, not as a Google requirement; many topics need less or more. If the user specifically asks for 600–2,500 words, stay within that range unless doing so would make the result misleading or padded.
- Keep the article language consistent with the requested audience and site. Do not switch languages mid-article.

## Workflow

### 1. Establish search intent and research

1. Identify whether the query is informational, commercial investigation, transactional, navigational, or mixed.
2. Determine the central question the page should satisfy and what would make this page useful beyond a generic summary.
3. When browsing is available and current/external facts matter, inspect relevant search results and prioritize primary sources, official documentation, subject-matter experts, and reputable publishers. Community discussions may reveal common questions or practical issues, but treat anecdotes as opinions rather than verified facts.
4. Collect primary keyword, secondary terms, common sub-questions, key entities, and source-backed facts. Use only terms that belong naturally in the article.
5. Avoid targeting the exact same primary search intent as another page on the same site when site data is available. If it is not available, mention that keyword cannibalization has not been checked.

### 2. Plan the article

1. Produce one clear working title/H1 and an outline that satisfies the intent without repetitive sections.
2. Use a logical heading hierarchy: one main H1 in the post template; H2s for major sections; H3s for nested points. Do not select heading levels merely to change font size.
3. Put a concise, direct answer or useful framing near the beginning. Include the primary focus keyword in the opening when it reads naturally.
4. For long articles with roughly three or more meaningful sections, include a table of contents or recommend one. Do not force a TOC into a short post that does not need it.
5. Add FAQs only when they address real reader questions and contribute useful content; do not add filler questions just to target extra phrases.

### 3. Write and edit the article

- Use clear, specific prose and short paragraphs. Aim for one main idea per paragraph; avoid walls of text. As a practical check, avoid paragraphs over roughly 120 words, since Rank Math may flag them.
- Use examples, tables, steps, definitions, comparisons, original analysis, or useful decision criteria when they genuinely help.
- Support important factual, technical, medical, legal, financial, or time-sensitive claims with reliable sources. Qualify uncertainty and make dates explicit when relevant.
- Use accurate wording and balanced explanations; don't overstate certainty or promise results.
- Do not paraphrase source material so closely that the article becomes a substitute for the source. Summarize and link/cite it.
- If the user provides an existing draft, preserve its intent and verified details. Prefer targeted revisions unless a rewrite is requested.

### 4. Prepare the Rank Math fields

Always provide the following fields in a clearly labeled block when drafting a post. Make each field copy-ready.

| Rank Math / WordPress field | Rule |
|---|---|
| **Post Title / H1** | Clear, unique, truthful, and useful. It should match the page's actual content and search intent. |
| **SEO Title** | Default site-wide template may be `%title% %sep% %sitename%`. For a specific post, supply a custom title when it better matches the query or improves clarity. Place the primary keyword near the beginning if natural; keep the wording concise and avoid repeating the same phrase. |
| **Permalink / Slug** | Provide a short, descriptive slug in lowercase with hyphens, ideally containing the primary keyword naturally. Rank Math uses 75 characters or fewer as its URL-length pass threshold; this is a plugin heuristic, not a ranking law. If the post is already published, do not change its URL casually: arrange a redirect and update internal links where necessary. |
| **Meta Description** | Prefer a manually written, unique 1–2 sentence summary that accurately describes the post and its value. Include the primary keyword naturally if useful. `%excerpt%` is acceptable only when the WordPress excerpt is deliberately written and suitable as a search snippet; do not assume an auto-generated excerpt is optimized. Search engines may generate a different snippet. |
| **Focus Keyword** | Set one primary focus keyword/phrase that best represents the page. Add secondary focus keywords only when they represent meaningful supporting queries and are supported by the content. Rank Math uses these internally for its analysis; they are not submitted to Google as a ranking instruction. |
| **WordPress Excerpt** | Optional but useful. Write a real excerpt instead of relying on an unrelated auto-excerpt, especially if `%excerpt%` is used in the meta description. |

When the site has a global snippet template, do not overwrite it unnecessarily. A template such as ` %title% %sep% %sitename% ` is a useful default, but a unique title may be better for an individual post. The final title displayed by Google is not guaranteed to exactly match the configured SEO title.

### 5. Apply the on-page keyword checks

Use this as a prioritized checklist, not a command to insert exact-match keywords everywhere:

- [ ] One relevant primary focus keyword is set in Rank Math.
- [ ] The primary phrase appears in the SEO title when it can be done naturally.
- [ ] The primary phrase appears in the meta description when it fits naturally.
- [ ] The slug is short, readable, and includes the phrase or its core wording when appropriate.
- [ ] The phrase or a natural close variant appears near the start of the article.
- [ ] The phrase/variants appear in the body where relevant.
- [ ] At least one relevant H2/H3 includes the phrase or a close variant if it fits the outline.
- [ ] At least one relevant image has descriptive alt text; include the keyword only if it accurately describes that image.
- [ ] Keyword usage sounds natural and does not become repetitive or awkward.

**Keyword density:** Rank Math's own documentation describes 1–1.5% as its general recommendation, but there is no universally correct density. Treat that range as a rough diagnostic, not a quota. If the exact phrase is repeated unnaturally, stop adding it. Avoid a density target overriding semantic variants, clarity, or reader experience.

### 6. Links

**Internal links**
- Link to relevant existing articles, category pages, guides, or other pages on the same site when they help readers continue their journey.
- Use descriptive anchor text that explains the destination; avoid generic anchors such as “click here” where a descriptive phrase works better.
- If site URLs are not provided or accessible, output **internal-link opportunities** as suggested target topics/anchor text. Do not invent URLs or claim the links are live.

**External links**
- Cite or link to reputable sources when they substantiate claims, help readers, or provide further reading. Prefer original/official sources where possible.
- Normal editorial links to trustworthy sources can generally remain followed. Use `rel="sponsored"` or `nofollow` for paid links as appropriate, and `ugc`/`nofollow` for untrusted user-generated links. Never manipulate link attributes solely to satisfy a plugin test.
- A Rank Math test may ask for a followed external link. Do not create an irrelevant link or convert a sponsored/affiliate link to followed for the sake of a green indicator.

### 7. Images and media

- Recommend images, diagrams, screenshots, or videos when they add explanatory value. Do not invent an image asset or claim one has been added when only text has been produced.
- For every proposed image, supply: placement/section, what it should show, and concise descriptive alt text. Mark image-generation or sourcing needs clearly.
- Alt text should describe the meaningful visual content and its context. Do not use the same exact keyword alt text for every image. Purely decorative images may use empty alt text in implementation.
- Use original/high-quality media when possible and place it near related text. Consider licensing, privacy, and attribution.
- Rank Math may reward media quantity (its documentation describes four images/videos for the full media test in some configurations), but **do not force four media items into every post**. The appropriate number depends on topic, layout, and reader needs.

### 8. Title readability: apply selectively

Rank Math may flag the absence of a sentiment word, power word, or number. Resolve a flag only when the addition is accurate and useful:

- **Keyword near the beginning:** preferred if natural; do not make the title ungrammatical.
- **Sentiment word:** use a positive/negative sentiment only where it conveys the actual article stance or outcome. Avoid fake urgency, fear, and exaggerated promises.
- **Power word:** use a concrete descriptor (for example, “practical”, “complete”, “essential”) only when the article supports it; avoid hype.
- **Number:** use numbers for genuinely numbered guides, comparisons, or data—not as decoration. Never invent a count or list structure solely to pass the test.

The title must remain accurate, distinctive, and concise. Google may truncate a long title and may generate a different title link from other page signals.

### 9. Readability and Content AI

- Use a TOC for long, section-heavy posts when it helps navigation.
- Keep paragraphs focused and easy to scan. Use lists and tables when they clarify, not as formatting filler.
- Include helpful media where it adds value; the text must remain useful without decorative additions.
- Content AI is optional. When available, use its keyword, outline, heading, link, and media suggestions as research prompts. Accept only suggestions that fit user intent and the verified facts. Review generated changes before applying them; do not claim that Content AI was used unless it actually was.
- Rank Math's SEO score and Content AI score measure different things. Neither guarantees indexing, rankings, or traffic.

### 10. Final audit before delivery

Check the article in this order:

**Critical**
- Does it answer the actual query?
- Are facts, dates, names, claims, links, and quotations verified or properly qualified?
- Is the content original/useful, with no fabricated experience or filler?
- Are SEO title, meta description, slug, and focus keyword supplied?
- Is the title a fair description of the page?

**Important**
- Keyword placement is natural in the title, opening, body, and a heading where relevant.
- Headings are logically nested; paragraphs are scannable.
- Internal links and citations are relevant and real, or are explicitly marked as suggestions.
- Image recommendations include accurate alt text, not keyword stuffing.
- The meta description is unique and not simply an unreviewed auto-excerpt.

**Optional Rank Math enhancements**
- Rough 1–1.5% keyword-density check if helpful, never a quota.
- Short URL, TOC for longer posts, useful media, relevant external followed link where appropriate.
- Sentiment word, power word, or title number only if the title benefits from it.
- Content AI feedback only when available and relevant.

Do not delay an otherwise excellent article to chase 100/100. Report which warnings were intentionally not followed and why, if any remain.

## Output contract

For a new post, return these sections in this order:

1. **SEO brief** — search intent, audience assumption, primary focus keyword, supporting terms, and any research caveat.
2. **Rank Math fields** — Post Title/H1, SEO Title, Slug, Meta Description, Focus Keyword, and optional Excerpt. Copy-ready; no extra commentary inside the fields.
3. **Article draft** — complete article with H2/H3 structure, cited sources as appropriate, and a TOC when useful.
4. **Media plan** — each recommended image/video, placement, and alt text. If none is useful, explain briefly.
5. **Link plan** — internal-link targets/anchors and external sources; clearly separate real verified URLs from suggested site pages.
6. **Rank Math audit** — a compact checklist with statuses `Pass`, `Review`, or `Not applicable`. Do not claim a live plugin score unless the actual editor or score was inspected.
7. **Sources** — trusted source links used for research, where applicable.

For a post audit/revision rather than a new draft, focus on the supplied content and list specific fixes first. Preserve working elements and do not rewrite the full post unless requested.
