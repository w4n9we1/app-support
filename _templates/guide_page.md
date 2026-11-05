---
# =============================================================================
# GUIDE PAGE TEMPLATE (Jekyll collection document, markdown)
# =============================================================================
# HOW TO USE
# 1. Copy this file to /Users/ww/code/app-support/_guides/<slug>.md —
#    the file name (slug) defines the final URL https://lababacy.com/guides/<slug>/
#    (collection already configured in _config.yml: output + permalink).
# 2. Replace every {{PLACEHOLDER}}. MUST-EDIT checklist:
#    - title            <= 60 chars
#    - description      120-160 chars, direct-answer style (feeds og:description
#                       via {% seo %} in the default layout)
#    - canonical        MUST equal https://lababacy.com/guides/<slug>/ —
#                       {% seo %} also emits a canonical from the permalink;
#                       keep this field in sync, it documents the intent
#    - image            keep the site-wide default, or a guide-specific
#                       1200x630 image in /assets_og/
#    - date             publish date, ISO 8601 (e.g. 2026-11-06 09:00 +0800)
#    - {{ANSWER}}       first paragraph: 40-60 words, fully self-contained
#                       direct answer (AI-summary friendly)
#    - JSON-LD block at the bottom: datePublished/dateModified, FAQ
#       mainEntity (MUST mirror the visible FAQ exactly, 4-6 questions),
#       breadcrumb slug
#    - internal links   only real, existing pages
# 3. Facts (formats, free tier, Pro, privacy) — copy wording from
#    _data/product_facts.yml. Qualitative only: never publish specific
#    row/cell counts or a dollar price.
# 4. Only claim capabilities that are actually implemented (plan §8).
# 5. WARNING before publishing: replace EVERY {{PLACEHOLDER}}. An unreplaced
#    {{PLACEHOLDER}} is valid Liquid (an undefined variable), so Jekyll renders
#    it as an EMPTY STRING and fails silently — no build error, just missing
#    text on the live page. Self-check on the final file: grep -n "{{" must
#    return nothing, and the rendered page must have no empty headings or
#    paragraphs.
# =============================================================================
layout: default
title: "{{TITLE}}"
description: "{{DESCRIPTION}}"
canonical: "https://lababacy.com/guides/{{SLUG}}/"
image: "/assets_og/og-databaseviewer.png"
date: "{{DATE_PUBLISHED}}"
---

{{ANSWER}}

<!-- Body: 3-5 H2 sections, each opens with a short direct answer to its
     question, then expands. Question-style H2s rank well for long-tail
     queries and are easy for AI engines to lift. -->

## {{SECTION_H2_1}}

{{BODY_1}}

## {{SECTION_H2_2}}

{{BODY_2}}

## Frequently asked questions

<!-- Keep 4-6 questions; the FAQPage JSON-LD below MUST mirror these exactly. -->

<details>
<summary>{{FAQ_Q_1}}</summary>
{{FAQ_A_1}}
</details>

<details>
<summary>{{FAQ_Q_2}}</summary>
{{FAQ_A_2}}
</details>

<details>
<summary>{{FAQ_Q_3}}</summary>
{{FAQ_A_3}}
</details>

<details>
<summary>{{FAQ_Q_4}}</summary>
{{FAQ_A_4}}
</details>

## Related pages

<!-- 2-3 internal links: sibling guides and/or format pages + the product page. -->

- [{{RELATED_1_TITLE}}]({{RELATED_1_URL}})
- [{{RELATED_2_TITLE}}]({{RELATED_2_URL}})
- [Database Viewer](/databaseviewer/)

## Get the app

Free to start — Pro is a one-time purchase.

[Download on the App Store](https://apps.apple.com/app/database-viewer-sqlite-dbf/id6811615295) · [Get it on Google Play](https://play.google.com/store/apps/details?id=com.lababacy.accessviewer&referrer=utm_source%3Dwebsite%26utm_medium%3Dseo)

<!-- JSON-LD: BlogPosting + FAQPage + BreadcrumbList.
     Keep the three scripts separate. dateModified = last substantive update. -->

<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "BlogPosting",
  "headline": "{{TITLE}}",
  "description": "{{DESCRIPTION}}",
  "datePublished": "{{DATE_PUBLISHED_ISO}}",
  "dateModified": "{{DATE_MODIFIED_ISO}}",
  "author": { "@type": "Organization", "name": "Lababacy", "url": "https://lababacy.com/" },
  "publisher": { "@type": "Organization", "name": "Lababacy" },
  "mainEntityOfPage": "https://lababacy.com/guides/{{SLUG}}/",
  "image": "https://lababacy.com/assets_og/og-databaseviewer.png"
}
</script>

<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "FAQPage",
  "mainEntity": [
    { "@type": "Question", "name": "{{FAQ_Q_1}}", "acceptedAnswer": { "@type": "Answer", "text": "{{FAQ_A_1}}" } },
    { "@type": "Question", "name": "{{FAQ_Q_2}}", "acceptedAnswer": { "@type": "Answer", "text": "{{FAQ_A_2}}" } },
    { "@type": "Question", "name": "{{FAQ_Q_3}}", "acceptedAnswer": { "@type": "Answer", "text": "{{FAQ_A_3}}" } },
    { "@type": "Question", "name": "{{FAQ_Q_4}}", "acceptedAnswer": { "@type": "Answer", "text": "{{FAQ_A_4}}" } }
  ]
}
</script>

<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "BreadcrumbList",
  "itemListElement": [
    { "@type": "ListItem", "position": 1, "name": "Lababacy", "item": "https://lababacy.com/" },
    { "@type": "ListItem", "position": 2, "name": "Guides", "item": "https://lababacy.com/guides/" },
    { "@type": "ListItem", "position": 3, "name": "{{TITLE}}", "item": "https://lababacy.com/guides/{{SLUG}}/" }
  ]
}
</script>
