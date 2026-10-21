# Reference notes: Rank Math post SEO and search-engine guidance

This file records the rationale behind the operational rules in `SKILL.md`. Re-check official documentation when Rank Math or Google changes a product or guideline.

## The important distinctions

### Rank Math's Focus Keyword is an editor-side analysis aid
Rank Math says focus keywords are used to analyze how a post is optimized within the plugin; they are not communicated to Google. Use the field to guide the page's subject and audit, not as a direct Google signal.

Source: https://rankmath.com/kb/general-tab/

### SEO score and Content AI score are different
Rank Math describes the SEO score as checks for basics such as SEO metadata, focus-keyword placement, links, and readability. Content AI provides content recommendations based on the target keyword and available search-result data. Passing these tests is not a guarantee of ranking.

Source: https://rankmath.com/kb/seo-score-vs-content-ai-score/

### 600 words is a Rank Math default check, not a Google minimum
Rank Math says its generic content-length test commonly recommends at least 600 words. Google explicitly says content length alone does not matter for ranking and there is no magical minimum or maximum word count. Use the amount of copy the search intent requires; do not pad content.

Sources:
- https://rankmath.com/kb/ideal-blog-post-length/
- https://developers.google.com/search/docs/fundamentals/seo-starter-guide

### Keyword density is not a hard target
Rank Math documents 1–1.5% as its general recommendation while also saying there is no perfect density and overuse should be avoided. Treat the percentage as a plugin-oriented diagnostic only, and favor natural language, close variants, and complete answers.

Source: https://rankmath.com/kb/seo-score-vs-content-ai-score/

### Rank Math's title checks are editorial heuristics
Rank Math checks SEO-title readability, including keyword placement near the beginning, sentiment words, power words, and numbers. For this workflow, the default is to deliberately address the sentiment-word and number checks in the SEO Title using a relevant positive or negative sentiment word recognized by Rank Math and a meaningful number supported by the article. These are plugin checks, not universal Google ranking factors. Never invent counts, dates, statistics, urgency, or exaggerated promises just to pass a test. If no truthful title can reasonably satisfy a check, mark it for review. Google recommends descriptive, concise titles and warns against keyword stuffing and boilerplate titles.

Sources:
- https://rankmath.com/kb/seo-score-vs-content-ai-score/
- https://developers.google.com/search/docs/appearance/title-link

### Meta descriptions can influence snippets but do not control them completely
Google may use a meta description as the search snippet, but may instead generate a snippet from page content. Descriptions should be concise, unique, useful, and specific to the page. `%excerpt%` is sensible only if the WordPress excerpt has been deliberately written for this role.

Sources:
- https://rankmath.com/kb/variables-in-seo-title-description/
- https://developers.google.com/search/docs/fundamentals/seo-starter-guide

### External followed links should not be forced
Rank Math includes tests for linking to external resources and for at least one followed external link. This is a plugin test, not a reason to create irrelevant links or misuse link attributes. Google recommends `sponsored` or `nofollow` for paid links, and `ugc` or `nofollow` for user-generated links; use `nofollow` for links the site does not trust, rather than blanket-marking all editorial links.

Sources:
- https://rankmath.com/kb/seo-score-vs-content-ai-score/
- https://developers.google.com/search/docs/crawling-indexing/links-crawlable

### Image alt text describes the image, not just the keyword
Rank Math may test whether the primary focus keyword appears in an image's alt attribute. Google's guidance is to write descriptive alt text that explains the image and its relationship to the page. Add a keyword only if it accurately describes the visual; do not use identical keyword-only alt text across images.

Sources:
- https://rankmath.com/kb/how-to-show-images-in-search-results/
- https://developers.google.com/search/docs/fundamentals/seo-starter-guide

### A table of contents and additional media are conditional UX decisions
Rank Math checks for a TOC and media. Use a TOC when it helps navigation, especially for long content with several meaningful headings. For WordPress/Elementor posts, the TOC should be generated automatically from the actual H1/H2/H3 heading blocks by the site's TOC block or widget; do not hand-write a duplicate TOC list in the article body. If the editor or widget is unavailable, provide an implementation note and do not claim the TOC has been inserted. Add images/videos when they explain something; do not create unnecessary elements only to pass tests.

Sources:
- https://rankmath.com/kb/table-of-contents/
- https://rankmath.com/kb/seo-score-vs-content-ai-score/

## Community perspective (anecdotal, not authoritative)

A discussion in r/SEO about whether a Rank Math score must be satisfied includes several users noting that keyword checks can miss natural variations and that the score should be treated as a reference rather than followed blindly. This aligns with the official guidance above, but Reddit comments represent individual experiences, not empirical proof or official policy.

Source: https://www.reddit.com/r/SEO/comments/wft6zi/is_it_necessary_to_follow_the_rank_math_seo_score/

## Skill format

This package follows the Agent Skills convention: a folder named to match the `name` field, containing `SKILL.md` with YAML frontmatter (`name` and `description`) followed by actionable instructions. A focused references directory contains supporting research notes.

Source: https://agentskills.io/specification


### Default language for publishable blog content

Unless the user explicitly requests a different language, draft publishable blog content and its SEO fields in English, including titles, headings, body text, meta descriptions, slugs, focus-keyword fields, excerpts, FAQs, image alt text, captions, and link anchor text. Keep operational notes outside the article separate; do not mix another language into the publishable content by default.
