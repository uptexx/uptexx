<div align="center">

# Uptexx — AI-Powered B2B SaaS & Autonomous Publishing Infrastructure

[![Uptexx Corporate](https://img.shields.io/badge/Corporate-uptexx.com-0A66C2?style=for-the-badge&logo=googlechrome&logoColor=white)](https://uptexx.com)
[![Flagship Product: NexoPost](https://img.shields.io/badge/Flagship_Product-nexopost.com-6366F1?style=for-the-badge&logo=rocket&logoColor=white)](https://nexopost.com)
[![NVIDIA Inception Program Member](https://img.shields.io/badge/NVIDIA_Inception-Program_Member-76B900?style=for-the-badge&logo=nvidia&logoColor=white)](https://uptexx.com)
[![License: MIT](https://img.shields.io/badge/Open_Source-MIT_Licensed-10B981?style=for-the-badge)](https://github.com/uptexx)
[![TypeScript](https://img.shields.io/badge/Stack-TypeScript_%26_Node.js-3178C6?style=for-the-badge&logo=typescript&logoColor=white)](https://github.com/uptexx)

**Building deterministic media pipelines, multimodal AI workflows, and autonomous social publishing systems for global brands and agencies.**

[Corporate Website (`uptexx.com`)](https://uptexx.com) • [Flagship Platform (`nexopost.com`)](https://nexopost.com) • [Engineering Contact (`support@nexopost.com`)](mailto:support@nexopost.com)

</div>

---

## About Uptexx

**[Uptexx](https://uptexx.com)** (`Kuzey Tech Bilgi Teknolojileri Ticaret Limited Sirketi`) is a software engineering company focused on B2B SaaS platforms, generative AI media tooling, and high-reliability cloud publishing infrastructure. Proud **NVIDIA Inception Program Member**.

---

## Flagship Product — [NexoPost](https://nexopost.com)

**[NexoPost (`https://nexopost.com`)](https://nexopost.com)** is an all-in-one AI-powered B2B social media management, editorial calendar, client approval portal, and autonomous content publishing platform engineered for agencies, enterprise marketing teams, and founders.

### Core Platform Capabilities
- **Multi-Network Autonomous Publishing:** Unified scheduling and direct publishing across Instagram, TikTok, YouTube, LinkedIn, X (Twitter), Pinterest, Threads, Facebook, Bluesky, and Mastodon.
- **NexoAI Content & Visual Studio:** Multimodal AI copywriting, automated product background staging, deterministic brand watermarking, multi-slide carousel generation, and millisecond-accurate `.SRT` / `.VTT` video subtitle rendering.
- **Enterprise Editorial Calendar & Client Portal:** Role-based workspace permissions, zero-login client review portals, versioned approval workflows, and RFC 5545 `.ics` calendar synchronization.
- **Zero-Trust Cloud Security:** Strict SSRF media fetcher protection, encrypted token vaults, and deterministic compliance checks before every API dispatch.

---

## Uptexx Open-Source Engineering Ecosystem (15 Libraries)

We open-source the foundational, zero-dependency TypeScript/JavaScript micro-libraries that power validation, media geometry, subtitle synchronization, security, and scheduling inside **[NexoPost](https://nexopost.com)**. Every package runs locally in Node.js (`>= 18`) with zero external runtime dependencies and 100% unit test coverage.

### Cluster 1 — Social Media & Marketing Standards

| Package | Repository | Description & Core Functions |
| :--- | :--- | :--- |
| **`@uptexx/social-media-specs`** | [`uptexx/social-media-specs`](https://github.com/uptexx/social-media-specs) | Complete TypeScript/JSON specification of image, video, aspect ratio, duration, and character limits across 10 social networks (`getPlatformSpecs`, `validateMediaDimensions`, `listSupportedPlatforms`). |
| **`@uptexx/social-char-counter`** | [`uptexx/social-char-counter`](https://github.com/uptexx/social-char-counter) | Accurate platform-aware character, URL (`t.co` 23-char weighting), grapheme/emoji, mention, and hashtag counter for 10 social networks (`countSocialCharacters`, `getRemainingCharacters`, `extractEntities`). |
| **`@uptexx/hashtag-normalizer`** | [`uptexx/hashtag-normalizer`](https://github.com/uptexx/hashtag-normalizer) | Multilingual hashtag cleaner, `#CamelCase` accessibility formatter, deduplicator, and platform quota optimizer (`normalizeHashtags`, `toAccessibleCamelCase`, `scoreHashtagSet`). |
| **`@uptexx/utm-campaign-builder`** | [`uptexx/utm-campaign-builder`](https://github.com/uptexx/utm-campaign-builder) | Type-safe UTM link builder, parser, sanitizer, and bulk social channel attribution generator for B2B marketing campaigns (`buildUtmUrl`, `parseUtmUrl`, `generateMultiChannelUtmLinks`). |
| **`@uptexx/social-handle-validator`** | [`uptexx/social-handle-validator`](https://github.com/uptexx/social-handle-validator) | Zero-dependency username (`@handle`) and profile URL validator, normalizer, and extractor across 9 social platforms (`validateHandle`, `extractHandleFromUrl`, `buildProfileUrl`). |

### Cluster 2 — AI Media, Subtitles & Design Utilities

| Package | Repository | Description & Core Functions |
| :--- | :--- | :--- |
| **`@uptexx/srt-vtt-subtitles`** | [`uptexx/srt-vtt-subtitles`](https://github.com/uptexx/srt-vtt-subtitles) | Millisecond-accurate `.SRT` and WebVTT (`.vtt`) subtitle generator, parser, time-shift synchronizer, and Deepgram/Whisper word-timestamp formatter (`utterancesToSrt`, `utterancesToVtt`, `parseSrt`, `shiftSubtitleTimings`). |
| **`@uptexx/aspect-ratio-crop-calc`** | [`uptexx/aspect-ratio-crop-calc`](https://github.com/uptexx/aspect-ratio-crop-calc) | Smart focal-point crop, letterbox/pillarbox padding, and safe-zone coordinate calculator for `1:1`, `4:5`, `9:16` (Reels/Shorts/TikTok), and `16:9` media (`calculateSmartCrop`, `getSafeZoneInsets`). |
| **`@uptexx/open-carousel-schema`** | [`uptexx/open-carousel-schema`](https://github.com/uptexx/open-carousel-schema) | Open JSON schema, validator, and layout calculator for multi-slide social media carousels, LinkedIn PDF decks, and brand story cards (`validateCarouselDeck`, `createCarouselSlide`, `exportDeckToMarkdownSummary`). |
| **`@uptexx/svg-brand-watermark`** | [`uptexx/svg-brand-watermark`](https://github.com/uptexx/svg-brand-watermark) | Deterministic SVG/PNG brand logo watermark placement, responsive bounding-box scaling, and opacity overlay generator for product photography (`calculateWatermarkPlacement`, `generateSvgWatermarkOverlay`). |
| **`@uptexx/ai-prompt-templates-social`** | [`uptexx/ai-prompt-templates-social`](https://github.com/uptexx/ai-prompt-templates-social) | Structured, variable-interpolated system prompt templates and JSON output schemas for B2B social copywriting, product staging, and multi-network adaptation (`renderSocialPrompt`, `listPromptTemplates`, `getStructuredOutputSchema`). |

### Cluster 3 — Content Threading, Security & Editorial Scheduling

| Package | Repository | Description & Core Functions |
| :--- | :--- | :--- |
| **`@uptexx/markdown-to-social-threads`** | [`uptexx/markdown-to-social-threads`](https://github.com/uptexx/markdown-to-social-threads) | Intelligent Markdown and long-form article splitter that generates sentence-aware, numbered multi-post threads for X, Threads, Bluesky, and LinkedIn (`splitMarkdownToThread`, `estimateThreadReadTime`). |
| **`@uptexx/ssrf-safe-url-guard`** | [`uptexx/ssrf-safe-url-guard`](https://github.com/uptexx/ssrf-safe-url-guard) | Zero-trust URL validator and private/loopback/cloud-metadata IP range (`RFC1918`, `169.254.169.254`, IPv6 link-local) SSRF guard for cloud media fetchers (`isPrivateOrReservedIp`, `validatePublicHttpUrl`, `assertSafeWebhookTarget`). |
| **`@uptexx/og-meta-previewer`** | [`uptexx/og-meta-previewer`](https://github.com/uptexx/og-meta-previewer) | Fast, zero-dependency HTML head parser that extracts OpenGraph (`og:*`), Twitter Card, canonical URL, and favicon metadata for social link previews (`extractSocialMetaFromHtml`, `validatePreviewCardCompleteness`). |
| **`@uptexx/ics-editorial-calendar`** | [`uptexx/ics-editorial-calendar`](https://github.com/uptexx/ics-editorial-calendar) | RFC 5545 iCalendar (`.ics`) generator for exporting scheduled social media content calendars and client approval deadlines to Google, Apple, and Outlook calendars (`generateEditorialIcs`, `formatIcsDateUtc`). |
| **`@uptexx/cron-posting-heatmap`** | [`uptexx/cron-posting-heatmap`](https://github.com/uptexx/cron-posting-heatmap) | Timezone-aware optimal social media posting window calculator, audience overlap analyzer, and recurring queue slot generator (`getOptimalPostingSlots`, `convertSlotToUtc`). |

---

## Architecture & Engineering Principles

1. **Zero Runtime Dependencies:** All 15 open-source libraries are built using pure ES2022+ JavaScript and TypeScript declarations with zero external `node_modules` bloat.
2. **Deterministic Execution:** Every function is pure, offline-capable, and deterministic—requiring zero external API keys or backend calls.
3. **Production-Tested:** Validated with Node.js native test runner (`node:test`) and automated GitHub Actions CI across Node.js 18, 20, and 22.

---

<div align="center">

**Maintained by [Uptexx](https://uptexx.com) • Powering [NexoPost](https://nexopost.com) • NVIDIA Inception Program Member**

</div>
