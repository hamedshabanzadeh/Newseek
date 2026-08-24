# Product

<!-- impeccable:product-schema 1 -->

## Platform

web

## Stack

Static HTML/CSS/JavaScript with no server or build step. Runs entirely in the browser using localStorage, Clipboard API, Service Worker, and PWA manifests.

## Users

Primary: Persian-speaking individuals researching current news on topics of personal or professional interest, who want to find the latest, most relevant, and reliable sources without manually searching multiple outlets.

Workflows: Users enter one or more topics (in Persian or English), set a time window and result limit, generate a structured news-search prompt, and open it in their preferred AI model to execute the search and receive curated results.

## Product Purpose

Newseek transforms a simple list of user topics into a structured, multi-stage news research prompt that works across multiple AI models. It eliminates manual prompt engineering by encoding a professional Discovery → Validation → Scoring → Deduplication → Final Selection → Enrichment workflow into a single reusable prompt.

Success means users can reliably find the latest, most important news on their topics without learning prompt engineering, without locking into a single search engine or AI provider, and without storing their interests on a server.

## Positioning

Newseek combines three distinct claims that competitors do not credibly copy together:

1. **Client-side + model-agnostic:** No server dependency, no stored user data, works seamlessly across ChatGPT, Claude, Gemini, Perplexity, and Grok with a single prompt.
2. **Structured workflow quality:** The generated prompt prioritizes primary/credible sources, validates freshness and novelty, scores on relevance/importance/impact/credibility, and removes duplicates and irrelevant content.
3. **Persian-first lightweight design:** Optimized for Persian users and RTL layout, clean and minimal interface, fast performance, and installable as a PWA without compromising simplicity or privacy.

## Operating Context

**Environment:** Web browser on mobile, tablet, or desktop; optionally installed as a PWA for app-like experience and offline support.

**Workflow rituals:** 
- Add topics of interest
- Choose time window (e.g., last week, last month)
- Set max results per topic
- Choose output language
- Configure summary detail level
- Generate prompt
- Review and copy prompt
- Open selected AI model and paste
- Execute search in chosen model

**Integration points:** Direct links to ChatGPT, Claude, Gemini, Perplexity, and Grok; clipboard copy; browser local storage for topic/settings persistence.

**Materials:** User-entered topics (Persian or English), structured news-search prompt (Persian or target language), AI model responses (not curated by Newseek).

## Capabilities and Constraints

**Capabilities:**
- Add unlimited topics with Persian and English language support
- Configure search time window (multiple options)
- Set result count per topic
- Choose output language for prompt
- Adjust summary detail level
- Generate multi-stage research prompt (Discovery, Validation, Scoring, Deduplication, Selection, Enrichment)
- Copy generated prompt
- Direct-open ChatGPT, Claude, Gemini, Perplexity, Grok with auto-copy
- Persist topics and settings in browser
- Responsive mobile/tablet/desktop UI
- Install as PWA
- Work offline (cached version)
- Auto-detect and notify user of new version

**Technical constraints:**
- No backend, no API calls, no user database
- Runs entirely in browser
- Execution depends on user's chosen AI model
- Cannot guarantee news freshness or accuracy (delegated to AI model)
- Service Worker cache strategy limited by browser storage
- No real user authentication or cross-device sync (by design)

**Product facts:**
- One-time first-visit onboarding for mobile/tablet PWA install
- Version update mechanism via Service Worker
- Offline capability via cache, not full functionality
- No analytics or tracking
- No third-party integrations or APIs

## Brand Commitments

**Name:** Newseek (نیوزسیک in Persian)

**Visual identity:** 
- Wordmark with distinctive split-color "s" 
- Neutral palette with blue accents
- Clean, minimal interface free of clutter or dashboard styling
- No artificial visual complexity or gamification

**Voice & personality:**
- Clear, direct, simple Persian wording
- Professional yet approachable
- Focused on clarity over decoration
- Privacy-respecting (data stays in browser)

**Typography:** Vazirmatn font family (weights: 300, 400, 500, 600, 700, 800, 900)

**Language priority:** Persian-first design and copy; English option for topics and output language choice.

**Layout:** Right-to-left (RTL) primary, responsive to mobile and desktop.

## Evidence on Hand

- Live service at https://hamedshabanzadeh.github.io/Newseek/
- Incumbent implementation: index.html (full product code)
- manifest.webmanifest (PWA metadata)
- service-worker.js (caching and version management)
- Icons: newseek-icon-192.png, newseek-icon-512.png
- readme.md (project overview in Persian)
- No fabricated results, testimonials, or customer claims

## Product Principles

1. **Privacy and control first:** All processing client-side; no stored user profiles; topics and settings persist only in browser; users choose which AI model to trust.
2. **Lightweight simplicity:** No clutter, no dashboard styling, no hidden features; one clear workflow from topic to prompt to model.
3. **Structured quality over convenience:** The effort to configure the prompt once buys reliable, multi-stage news filtering across any AI model; worth the step.
4. **Model independence:** Newseek works with any capable AI model equally; users never forced to one provider; prompt remains portable and human-readable.
5. **Persian-first accessibility:** RTL-native design, Persian language priority, mobile-optimized from day one, fast performance on limited networks; not an afterthought translation.

## Accessibility & Inclusion

Required: Persian language support (not optional); RTL layout as primary reading order; responsive mobile experience (first-class, not scaled).

Assumed: Modern browser (Chrome, Safari, Firefox, Edge) with JavaScript and localStorage support; capable of clipboard API and PWA manifest.

No specific disability accommodation requirements stated; treat as needing standard web a11y (semantic HTML, keyboard navigation, color contrast, focus visible).
