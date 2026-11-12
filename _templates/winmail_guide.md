---
# =============================================================================
# WINMAIL GUIDE TEMPLATE (Jekyll collection `winmail_guides`, markdown)
#
# HOW TO USE
# 1. Copy to /Users/ww/code/app-support/_winmail_guides/<slug>.md
#    URL = https://lababacy.com/winmail/guides/<slug>/
# 2. Replace every {{PLACEHOLDER}}; `grep -n "{{"` must return nothing.
# 3. Facts: _data/winmail_facts.yml + ~/code/winmail/app-truth.md §2/§4/§6/§9.
#    Free = FIRST SCREEN teaser. No dollar figures, no row counts, no Android,
#    no Mac app, no OST→PST, no "zero data collected".
# 4. First paragraph = 40–60 word self-contained answer (AI-summary friendly).
# 5. FAQ: 4–6 questions; the JSON-LD below MUST mirror them exactly.
# 6. Internal links: only existing pages; link back to the matching format hub
#    and to https://lababacy.com/winmail/.
# 7. dateModified + visible "Last updated" must match.
# =============================================================================
layout: winmail
title: "{{TITLE}}"
description: "{{DESCRIPTION_120_160_CHARS}}"
canonical: "https://lababacy.com/winmail/guides/{{SLUG}}/"
image: "/assets_og/og-winmail.png"
date: "{{DATE_PUBLISHED}}"
---

{{ANSWER_40_60_WORDS}}

## {{SECTION_H2_1}}

{{BODY_1}}

## {{SECTION_H2_2}}

{{BODY_2}}

## {{SECTION_H2_3}}

{{BODY_3}}

## Frequently asked questions

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

## Related

- [{{FORMAT_HUB_LABEL}}](https://lababacy.com/winmail/formats/{{FORMAT_SLUG}}/)
- [All formats Winmail Reader opens](https://lababacy.com/winmail/formats/)
- [Winmail Reader](https://lababacy.com/winmail/)
- [Privacy policy](https://lababacy.com/winmail/privacy/)

*Last updated: {{YYYY-MM-DD}}*

<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "BlogPosting",
  "headline": "{{TITLE}}",
  "description": "{{DESCRIPTION_120_160_CHARS}}",
  "datePublished": "{{DATE_PUBLISHED}}",
  "dateModified": "{{DATE_MODIFIED}}",
  "author": { "@type": "Organization", "name": "Lababacy" },
  "publisher": { "@type": "Organization", "name": "Lababacy" },
  "mainEntityOfPage": "https://lababacy.com/winmail/guides/{{SLUG}}/",
  "about": { "@type": "SoftwareApplication", "name": "Winmail Reader - DAT, MSG, EML", "sameAs": ["https://apps.apple.com/app/winmail-reader-dat-msg-eml/id6823454038"] }
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
    { "@type": "ListItem", "position": 1, "name": "Home", "item": "https://lababacy.com/" },
    { "@type": "ListItem", "position": 2, "name": "Winmail Reader", "item": "https://lababacy.com/winmail/" },
    { "@type": "ListItem", "position": 3, "name": "Guides", "item": "https://lababacy.com/winmail/guides/" },
    { "@type": "ListItem", "position": 4, "name": "{{TITLE}}", "item": "https://lababacy.com/winmail/guides/{{SLUG}}/" }
  ]
}
</script>
