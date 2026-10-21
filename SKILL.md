---
name: rank-math-post-seo
description: Research, draft, optimize, and audit WordPress blog posts for Rank Math SEO. Use when creating or revising posts, selecting a focus keyword, preparing an SEO title/meta description/slug, improving headings, images, links, readability, or checking Rank Math recommendations without sacrificing helpfulness or natural writing.
metadata:
  version: "1.2.0"
  language: "en"
---

# Rank Math SEO Post Writer

## Purpose

Create useful, well-researched, search-intent-matched WordPress posts and prepare the post-level fields used by Rank Math SEO. Optimize for readers first; use Rank Math as a diagnostic checklist, not as a ranking guarantee. **This SKILL.md is the complete, self-contained instruction file and must not require any separate local reference file to operate.** The SEO decision rules and official documentation links included below provide the context needed when plugin recommendations conflict with reader value or search-engine guidance.

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
- **Default language: English.** Unless the user explicitly requests another language, write all publishable blog content entirely in English, including the post title, H1/H2/H3 headings, article body, SEO title, meta description, slug, focus keyword, excerpt, FAQ, image alt text, captions, and link anchor text.
- Keep the article language consistent throughout. Do not mix Chinese or other languages into publishable content unless explicitly requested. Operational explanations outside the article may use the user's preferred language.

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
4. For long articles with roughly three or more meaningful sections, recommend an automatically generated Table of Contents when it improves navigation. **Do not hand-write a TOC list inside the article draft.** Structure the actual content with correctly nested H1/H2/H3 headings so a WordPress/Elementor TOC block or widget can generate the entries from those headings. If the component has not been inserted or inspected, provide a separate implementation note and do not claim the TOC is live.
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
| **SEO Title** | Default site-wide template may be `%title% %sep% %sitename%`. For a specific post, supply a custom title when it better matches the query or improves clarity. Place the primary keyword near the beginning if natural; keep the wording concise and avoid repeating the same phrase. By default, deliberately optimize the SEO Title for Rank Math's sentiment-word and number checks: include a relevant positive or negative sentiment word recognized by Rank Math and a meaningful number when this can be done accurately and naturally. Keep the title concise and aligned with actual article content. Never invent counts, statistics, dates, urgency, or exaggerated claims merely to make a test pass; if a truthful title cannot reasonably satisfy a check, mark it `Review` and explain why. |
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

### 8. Title readability: default checks for SEO Title

By default, build the SEO Title so it addresses Rank Math's sentiment-word and number checks while staying truthful, relevant, and readable. These are plugin readability checks, not universal Google ranking factors.

- **Sentiment word:** Include a positive or negative sentiment word that Rank Math recognizes and that genuinely fits the article's content. Consult the current official Rank Math guidance or editor feedback when unsure; do not assume any adjective will pass.
- **Number:** Include a meaningful number that is supported by the article, such as the actual count of methods, steps, mistakes, comparisons, or a relevant verified year. If the title promises a specific count, the body must contain that number of substantive items.
- **Primary keyword:** Place it near the beginning when natural, without making the title awkward or repetitive.
- **Accuracy:** Avoid fake urgency, fear, exaggerated promises, arbitrary numbers, or unsupported statistics.
- **Post Title/H1:** It may match the SEO Title when that reads well. Do not distort the reader-facing H1 just to force a plugin indicator; prioritize the actual Rank Math SEO Title check and keep both titles consistent with the page.
- **Verification:** Before delivery, state which sentiment word and number were used in the SEO Title. If the actual Rank Math editor is unavailable, report a content-level assessment rather than claiming the live test passed. If a truthful title cannot reasonably satisfy a check, mark it `Review` and explain why.

The SEO Title must remain accurate, distinctive, and concise. Google may truncate it or generate a different title link from other page signals.

### 9. Readability and Content AI

- Use an automatically generated TOC for long, section-heavy posts when it helps navigation. Generate entries from the actual WordPress/Elementor H1/H2/H3 heading blocks or configured TOC widget; do not include a hand-written duplicate list of headings in the article draft. If no site editor is available, provide a separate implementation note instead of claiming the widget has been added.
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
- Is the SEO Title assessed for a Rank Math-recognized sentiment word and a meaningful number? Record the word and number; do not claim a live pass unless the editor was inspected.
- Is the title a fair description of the page?
- Is all publishable article content and publishable SEO metadata in English by default, unless the user explicitly requested another language?
- For long, section-heavy articles, is the TOC intended to be generated automatically from actual headings rather than manually typed into the article?

**Important**
- Keyword placement is natural in the title, opening, body, and a heading where relevant.
- Headings are logically nested; paragraphs are scannable.
- Internal links and citations are relevant and real, or are explicitly marked as suggestions.
- Image recommendations include accurate alt text, not keyword stuffing.
- The meta description is unique and not simply an unreviewed auto-excerpt.

**Optional Rank Math enhancements**
- Rough 1–1.5% keyword-density check if helpful, never a quota.
- Short URL, TOC for longer posts, useful media, relevant external followed link where appropriate.
- Apply the default sentiment-word and meaningful-number checks for the SEO Title as described in Section 8. Use power words selectively, only when they are accurate and improve clarity.
- Content AI feedback only when available and relevant.

Do not delay an otherwise excellent article to chase 100/100. Report which warnings were intentionally not followed and why, if any remain.

## Self-contained SEO principles and official source notes

The rules in this section are part of this file's operational instructions. They are included here so the Skill remains usable when only this SKILL.md is installed or supplied.

### Focus Keyword and scoring

- Rank Math's Focus Keyword is an editor-side analysis aid. Rank Math uses it to analyze the post; it is not sent to Google as a ranking instruction. Use it to keep the article focused, not as a claimed direct ranking signal.
- Rank Math's SEO score and Content AI score are different. The SEO score checks on-page basics such as metadata, keyword placement, links, and readability. Content AI provides suggestions based on the target keyword and available search-result data. Neither score guarantees indexing, rankings, or traffic.
- Official sources: [Rank Math General Tab](https://rankmath.com/kb/general-tab/) and [Rank Math SEO Score vs. Content AI Score](https://rankmath.com/kb/seo-score-vs-content-ai-score/).

### Content length and keyword density

- Rank Math's generic content-length test commonly uses 600 words as a baseline. This is a plugin check, not a Google minimum. Google states that content length alone does not determine ranking and there is no universal ideal word count. Write as much as the search intent requires; do not pad.
- Rank Math documents 1–1.5% as a general keyword-density recommendation, but there is no universally correct density. Treat it only as a rough diagnostic and never as a quota. Prefer natural variants, clarity, and complete answers over repetition.
- Official sources: [Rank Math's Ideal Blog Post Length](https://rankmath.com/kb/ideal-blog-post-length/), [Google SEO Starter Guide](https://developers.google.com/search/docs/fundamentals/seo-starter-guide), and [Rank Math SEO Score vs. Content AI Score](https://rankmath.com/kb/seo-score-vs-content-ai-score/).

### SEO titles and search snippets

- The default SEO Title workflow deliberately checks for a Rank Math-recognized sentiment word and a meaningful number, while keeping the title truthful, readable, concise, and aligned with the actual article. These are plugin readability checks, not universal Google ranking factors.
- Never invent a count, statistic, year, urgency, benefit, or claim just to make a title test pass. When a number describes a count, the article must contain that number of substantive items. If no truthful title can reasonably satisfy a check, mark it Review and explain why.
- Google may truncate a title or generate a different title link from page signals. A manually written SEO title is not a guarantee that Google will show exactly that wording.
- Official sources: [Rank Math SEO Score vs. Content AI Score](https://rankmath.com/kb/seo-score-vs-content-ai-score/) and [Google's Title Links Guidance](https://developers.google.com/search/docs/appearance/title-link).

### Meta descriptions and excerpts

- Write a unique, accurate, useful meta description specific to the page. Include the primary keyword naturally when appropriate.
- Search engines may use the meta description as a search snippet or generate a snippet from page content. The description does not fully control what appears in search results.
- Use the `%excerpt%` variable only when the WordPress excerpt has deliberately been written and is suitable for the snippet; do not assume an auto-generated excerpt is optimized.
- Official sources: [Rank Math Title and Description Variables](https://rankmath.com/kb/variables-in-seo-title-description/) and [Google SEO Starter Guide](https://developers.google.com/search/docs/fundamentals/seo-starter-guide).

### Links, image alt text, and TOC

- Add external links when they substantiate a claim or help the reader. Do not force an irrelevant followed external link solely to pass a plugin test. Use `rel="sponsored"` or `nofollow` for paid links as appropriate, and `ugc`/`nofollow` for untrusted user-generated content. Do not blanket-mark all normal editorial links as nofollow.
- Image alt text must describe the meaningful visual content and its relationship to the page. Include a keyword only when it accurately describes the image; do not repeat the same keyword-only alt text across multiple images. Decorative images may use empty alt text when implemented as decorative.
- A Table of Contents is a conditional usability feature. When useful, generate it from actual WordPress/Elementor H1/H2/H3 heading blocks using the site's TOC block or widget. Never hand-write a duplicate heading list in the article body. If the widget/editor is unavailable, provide an implementation note and do not claim it has been inserted.
- Add images or videos when they genuinely explain the subject; do not force media counts to satisfy a plugin test.
- Official sources: [Rank Math Link and SEO Score Guidance](https://rankmath.com/kb/seo-score-vs-content-ai-score/), [Google Crawlable Links Guidance](https://developers.google.com/search/docs/crawling-indexing/links-crawlable), [Rank Math Image Search Guidance](https://rankmath.com/kb/how-to-show-images-in-search-results/), [Rank Math Table of Contents](https://rankmath.com/kb/table-of-contents/), and [Google SEO Starter Guide](https://developers.google.com/search/docs/fundamentals/seo-starter-guide).

### Interpreting plugin checks

- Resolve Rank Math warnings when doing so improves clarity, relevance, usability, or metadata quality.
- When a check is a heuristic and a change would introduce filler, keyword stuffing, an inaccurate title, irrelevant links, or unnecessary media, preserve the better editorial choice and mark the warning Review with a short reason.
- Do not chase 100/100 as a substitute for accuracy, usefulness, or search performance. Community discussions can offer anecdotal context but do not override official documentation.

## Output contract

For a new post, return these sections in this order:

1. **SEO brief** — search intent, audience assumption, primary focus keyword, supporting terms, and any research caveat.
2. **Rank Math fields** — Post Title/H1, SEO Title, Slug, Meta Description, Focus Keyword, and optional Excerpt. Copy-ready; no extra commentary inside the fields.
3. **Article draft** — complete article with properly nested H1/H2/H3 headings and cited sources as appropriate. Do not include a manually written TOC list in the article body; when a TOC is useful, add a separate implementation note for automatic generation from the actual headings.
4. **Media plan** — each recommended image/video, placement, and alt text. If none is useful, explain briefly.
5. **Link plan** — internal-link targets/anchors and external sources; clearly separate real verified URLs from suggested site pages.
6. **Rank Math audit** — a compact checklist with statuses `Pass`, `Review`, or `Not applicable`. Include the SEO Title's proposed sentiment word and meaningful number, the default English-language check, and the automatic-TOC implementation status where relevant. Do not claim a live plugin score or a live TOC insertion unless the actual editor/site was inspected.
7. **Sources** — trusted source links used for research, where applicable.

For a post audit/revision rather than a new draft, focus on the supplied content and list specific fixes first. Preserve working elements and do not rewrite the full post unless requested.
