# How to use `template.html`

This is the same single-page showcase site you have for the 6th Asian U18 Athletics Championships, but with every project-specific value replaced by a `{{PLACEHOLDER}}`. Paste it into any AI chat (Claude, ChatGPT, etc.) along with the prompt below and your details — the AI will fill in the placeholders and give you a ready-to-deploy `index.html` for your next project.

---

## Ready-to-paste prompt

> I have an HTML template for a single-page project showcase site. Below is the template followed by my project details. Replace every `{{PLACEHOLDER}}` with the matching value from my details and return the complete, finished `index.html` file. Do not add new sections, do not invent extra colors, do not change the structure. Keep all CSS, JavaScript, and SVG icons exactly as they are. Do not use emojis anywhere.
>
> **PROJECT DETAILS**
>
> - PROJECT_NAME: …
> - PROJECT_NAME_PART_1 / HIGHLIGHT / PART_2: … / … / …  *(split for the heading accent color)*
> - PROJECT_TAGLINE: …
> - PROJECT_YEAR: …
> - PROJECT_LOCATION: …
> - PROJECT_LOCATION_AND_YEAR: e.g. "Riyadh 2026"
> - PROJECT_DURATION: e.g. "3 days"
> - PROJECT_SCOPE: e.g. "End-to-End Delivery"
> - ONE_LINE_PROJECT_SUMMARY: short meta-description sentence
> - LOGO_DATA_URI: paste a `data:image/png;base64,…` of the project logo *(or a URL)*
> - HERO_AWARD_IMAGE_URL: paste a `data:image/jpeg;base64,…` of the proof/award photo *(or a URL)*
> - HERO_AWARD_ALT_TEXT: short description of the proof image
>
> **COMPANY**
>
> - COMPANY_NAME: e.g. "Mood Event"
> - COMPANY_NAME_PART_1 / PART_2: e.g. "Mood" / "Event"  *(footer split brand)*
> - COMPANY_TAGLINE: footer tagline
> - CTA_TEXT: e.g. "Work With Us"
> - CTA_HREF: e.g. "mailto:info@moodevent.net"
>
> **OVERVIEW**
>
> - OVERVIEW_HEADING_PART_1 / HIGHLIGHT: heading and accent
> - OVERVIEW_PARAGRAPH_1
> - OVERVIEW_PARAGRAPH_2
> - OVERVIEW_ACCENT_QUOTE: the dark callout quote
>
> **STATS** (5 numbers shown in the dark band)
>
> - STAT_1_NUM, STAT_1_LABEL
> - STAT_2_NUM, STAT_2_SUFFIX *(use "+" or empty)*, STAT_2_LABEL
> - STAT_3_NUM, STAT_3_LABEL
> - STAT_4_NUM, STAT_4_LABEL
> - STAT_5_NUM, STAT_5_LABEL
>
> **OUR ROLE** (6 cards)
>
> - ROLE_HEADING_PART_1 / HIGHLIGHT / PART_2
> - ROLE_LEAD_PARAGRAPH
> - CARD_1_TITLE, CARD_1_DESCRIPTION
> - CARD_2_TITLE, CARD_2_DESCRIPTION
> - CARD_3_TITLE, CARD_3_DESCRIPTION
> - CARD_4_TITLE, CARD_4_DESCRIPTION
> - CARD_5_TITLE, CARD_5_DESCRIPTION
> - CARD_6_TITLE, CARD_6_DESCRIPTION
>
> **TIMELINE** (5 stages)
>
> - TIMELINE_HEADING_PART_1 / HIGHLIGHT
> - TIMELINE_INTRO_PARAGRAPH
> - TIMELINE_STAGE_1_TITLE / DESC
> - TIMELINE_STAGE_2_TITLE / DESC
> - TIMELINE_STAGE_3_TITLE / DESC
> - TIMELINE_STAGE_4_TITLE / DESC
> - TIMELINE_STAGE_5_TITLE / DESC
>
> **QUOTE BLOCK**
>
> - QUOTE_PART_1, QUOTE_HIGHLIGHT, QUOTE_PART_2
>
> **BRAND PALETTE** (any 4 hexes — keep the "primary dark / accent / light accent / soft background" relationship)
>
> - COLOR_PRIMARY_DARK: e.g. `#3D2755`
> - COLOR_ACCENT: e.g. `#7851A0`
> - COLOR_LIGHT_ACCENT: e.g. `#B19EC4`
> - COLOR_SOFT_BG: e.g. `#E1DBE7`
>
> **FONTS** (Google Fonts names)
>
> - HEADING_FONT: e.g. `Barlow Condensed`
> - BODY_FONT: e.g. `Barlow`
> - HEADING_FONT_GOOGLE_PARAM: e.g. `Barlow+Condensed:wght@600;700;800;900`
> - BODY_FONT_GOOGLE_PARAM: e.g. `Barlow:wght@300;400;500;600`
>
> **TEMPLATE FOLLOWS — paste it back to me filled in:**
>
> ```html
> [paste the full contents of template.html here]
> ```

---

## Notes for converting images to base64 (so they embed in the HTML)

If you want the proof photo and project logo embedded inside the HTML (so the page is one self-contained file with no broken-image risk), convert them to base64 data URIs first. The simplest way:

1. Go to https://www.base64-image.de/
2. Upload your image
3. Copy the `data:image/...` string it produces
4. Paste that into the `LOGO_DATA_URI` or `HERO_AWARD_IMAGE_URL` placeholder

Both fields also accept normal image URLs (e.g. `https://example.com/photo.jpg`) if you'd rather host the images separately.
