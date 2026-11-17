# Visual fidelity

Overall match: **7/100** — fonts, type sizes, spacing and each section measured in a browser on both sites, and how alike the pages look as pictures, each counted from what two unrelated pages score (0) to identical (100); the weaker of the two counts double, and so do the weakest page and device. How it's scored: docs/qa/import-fidelity.md.

**Next step:** The automatic move is rough (7/100): the words and pictures came across, but most of the design didn't. That's normal for custom-built sites. Claude can make it match closely: in Claude with the OpenSpace connector, use the finish-a-move prompt (or Studio's "Finish it with Claude"). It compares the old and new pages side by side and rebuilds what didn't come across, keeping every word and picture editable.

Scored two ways, side by side: **7/100 corrected**, 6/100 by the strict v3 scorer. The corrected score reads three things the strict one gets wrong (navigation in a header themed "brand", off-screen slides counted as columns, a picture-only band on a phone); the pages below list where it did.

Before auto-tuning: 6/100. What it changed:

- section padding 50px
- section padding on phones 46px
- /challenges: 1 section(s) at the narrow width, as on the original
- text on light sections #000000, as on the original (13 of 13 sections)
- heading on light sections #000000, as on the original (13 of 13 sections)
- text on light-accent sections #000000, as on the original (2 of 2 sections)
- /: "AWAKEN THE CURRENTS OF CREATION" set at the h2 size, as on the original
- /bloom-retreat-may-2024: "You're Invited" set at the display size, as on the original
- /contact-me: "Get in touch" set at the display size, as on the original
- /copy-of-bloom-retreat-may-2024: "You're Invited" set at the display size, as on the original
- /: section 3 881px tall, as on the original
- /bloom-retreat-may-2024: section 1 711px tall, as on the original
- /bloom-retreat-may-2024: section 7 609px tall, as on the original
- /bloom-retreat-may-2024: section 15 1172px tall, as on the original
- /copy-of-bloom-retreat-may-2024: section 1 711px tall, as on the original
- /copy-of-bloom-retreat-may-2024: section 7 609px tall, as on the original
- /copy-of-bloom-retreat-may-2024: section 15 1159px tall, as on the original
- /bloom-retreat-may-2024: section 1 "Bloom" recreated as a custom component
- /bloom-retreat-may-2024: section 2 "You're Invited" recreated as a custom component
- /bloom-retreat-may-2024: section 3 "If you feel called to :" recreated as a custom component
- /bloom-retreat-may-2024: section 7 recreated as a custom component
- /bloom-retreat-may-2024: section 9 recreated as a custom component
- /bloom-retreat-may-2024: section 10 recreated as a custom component
- /bloom-retreat-may-2024: section 15 "Frequently Asked Questions" recreated as a custom component
- /contact-me: "Get in touch" set at the h3 size, as on the original

Without custom components: 7/100; with the sections recreated as components: 7/100.

## / at 1440px — 11/100

Checks passed: 61% · screenshots 46% alike (two unrelated pages compare at about 55%).

Original: https://www.courtneyacamo.com/  
Imported: / (local preview)

| Check | Original | Imported | |
|---|---|---|---|
| Heading font | forum | Forum | same |
| Heading 1 size | 80px | 80px | same |
| Heading 2 size | 80px | 80px | same |
| Heading 3 size | 109px | 109px | same |
| Body font | avenir-lt-w01_35-light1475496 | Jost (close stand-in) | close (85%) |
| Body text size | 20px | 20px | same |
| Label font | forum | Forum | same |
| Navigation size | 20px | 20px | same |
| Navigation letter spacing and case | 0em, none | 0em, none | same |
| Content width | 354px | 1280px | **differs** |
| Section padding | 11px | 49px | **differs** |

| # | Section | Match | Differences |
|---|---|---|---|
| 1 | AWAKEN THE CURRENTS OF CREATION | 67 | Image placement: left, 50% wide → right, 56% wide; Image crop: 1.06:1 → 0.75:1; Height: 679px → 1230px |
| 2 | Courtney’s intuitively guided approach to mentorship weaves modern therapy with ancient wisdom tradi | 40 | Heading: forum 23px → Forum 80px; Height: 200px → 1068px |
| 3 | Hi, it’s nice to meet you. | 17 | Heading: forum 64px → Forum 109px; Text: avenir-lt-w01_35-light1475496 20px → Jost 20px; Text color: #000000 → #f8f1ed; Columns: 3 → 2; Image placement: right, 48% wide → center, 100% wide; Image crop: 0.99:1 → 0.66:1; Height: 881px → 2168px |
| 4 | Lets work | 67 | Text: avenir-lt-w01_35-light1475496 22px → Jost 20px; Image placement: left, 32% wide → left, 57% wide; Image crop: 0.85:1 → 1.5:1; Height: 1609px → 2310px |
| 5 | Client Love | 56 | Text: avenir-lt-w01_35-light1475496 20px → Jost 20px; Columns: 2 → 1; Image placement: right, 34% wide → center, 89% wide; Image crop: 1.33:1 → 1:1; Height: 747px → 3373px |

What would close the gap:

- Site Styles → choices.typography.body = { family: "avenir-lt-w01_35-light1475496" } (Google Fonts), or upload it in Site Styles → Your fonts.
- choices.layout.contentWidth = 354
- choices.layout.sectionPadding = 11
- Adjust the stack column spans (image column) or the image's side.
- Use the original's image proportions (the block's aspect ratio).
- Lay the text out in columns (a stack layout with more columns, or the text block's Columns style).

## / at 1132px — 11/100 (strict v3: 8/100)

Corrected scoring on this page:

- Section 1: columns counted on screen only (2 → 1 counted as 1 → 1; what's off screen or inside one slideshow or map isn't a column).
- Section 2: columns counted on screen only (2 → 1 counted as 1 → 1; what's off screen or inside one slideshow or map isn't a column).
- Section 3: columns counted on screen only (2 → 1 counted as 1 → 1; what's off screen or inside one slideshow or map isn't a column).
- Section 4: columns counted on screen only (2 → 2 counted as 1 → 2; what's off screen or inside one slideshow or map isn't a column).
- Section 5: columns counted on screen only (2 → 1 counted as 1 → 1; what's off screen or inside one slideshow or map isn't a column).

Checks passed: 61% · screenshots 45% alike (two unrelated pages compare at about 55%).

Original: https://www.courtneyacamo.com/  
Imported: / (local preview)

| Check | Original | Imported | |
|---|---|---|---|
| Heading font | forum | Forum | same |
| Heading 1 size | 80px | 80px | same |
| Heading 2 size | 80px | 80px | same |
| Heading 3 size | 109px | 109px | same |
| Body font | avenir-lt-w01_35-light1475496 | Jost (close stand-in) | close (85%) |
| Body text size | 20px | 20px | same |
| Navigation: present | forum 20px | not found | **differs** |
| Content width | 506px | 342px | **differs** |
| Section padding | 11px | 39px | **differs** |

| # | Section | Match | Differences |
|---|---|---|---|
| 1 | AWAKEN THE CURRENTS OF CREATION | 78 | Image placement: left, 50% wide → center, 87% wide; Height: 679px → 1620px |
| 2 | Courtney’s intuitively guided approach to mentorship weaves modern therapy with ancient wisdom tradi | 40 | Heading: forum 23px → Forum 80px; Height: 200px → 1980px |
| 3 | Hi, it’s nice to meet you. | 37 | Heading: forum 64px → Forum 109px; Text: avenir-lt-w01_35-light1475496 20px → Jost 20px; Text color: #000000 → #f8f1ed; Image placement: right, 70% wide → center, 100% wide; Image crop: 0.99:1 → 0.18:1; Height: 881px → 2130px |
| 4 | Lets work | 47 | Text: avenir-lt-w01_35-light1475496 22px → Jost 20px; Columns: 1 → 2; Image placement: left, 47% wide → center, 87% wide; Image crop: 0.85:1 → 1.5:1; Height: 1609px → 2489px |
| 5 | Client Love | 72 | Text: avenir-lt-w01_35-light1475496 20px → Jost 20px; Image placement: right, 49% wide → center, 87% wide; Image crop: 1.33:1 → 1:1; Height: 747px → 1728px |

What would close the gap:

- Site Styles → choices.typography.body = { family: "avenir-lt-w01_35-light1475496" } (Google Fonts), or upload it in Site Styles → Your fonts.
- choices.layout.contentWidth = 506
- choices.layout.sectionPadding = 11
- Adjust the stack column spans (image column) or the image's side.
- Use the original's image proportions (the block's aspect ratio).
- Fewer columns: merge them into one stack column.

## /bloom-retreat-may-2024 at 1440px — 15/100

Checks passed: 71% · screenshots 53% alike (two unrelated pages compare at about 55%).

Original: https://www.courtneyacamo.com/bloom-retreat-may-2024  
Imported: /bloom-retreat-may-2024 (local preview)

| Check | Original | Imported | |
|---|---|---|---|
| Heading 1: present | forum 176px | not found | **differs** |
| Heading font | forum | Forum | same |
| Heading 2 size | 56px | 80px | **differs** |
| Heading 3 size | 18px | 52px | **differs** |
| Body font | avenir-lt-w01_35-light1475496 | Jost (close stand-in) | close (85%) |
| Body text size | 20px | 20px | same |
| Lead text size | 25px | 46px | **differs** |
| Label font | forum | Forum | same |
| Navigation size | 20px | 20px | same |
| Navigation letter spacing and case | 0em, none | 0em, none | same |
| Section padding | 8.5px | 25px | **differs** |

| # | Section | Match | Differences |
|---|---|---|---|
| 1 | Bloom | 70 | Heading: forum 176px → Jost 176px |
| 2 | You're Invited | 77 | Heading: forum 118px → Jost 118px; Text: avenir-lt-w01_35-light1475496 24px → Jost 24px; Height: 316px → 550px |
| 3 | If you feel called to : | 85 | Heading: forum 52px → Jost 52px; Text: avenir-lt-w01_35-light1475496 20px → Jost 20px |
| 4 | (no heading) | 100 | — |
| 5 | (no heading) | 78 | Text: avenir-lt-w01_35-light1475496 18px → Jost 20px; Height: 299px → 510px |
| 6 | Join the Journey | 89 | Text: avenir-lt-w01_35-light1475496 20px → Jost 20px; Image placement: left, 28% wide → right, 27% wide |
| 7 | (no heading) | 59 | Text: avenir-lt-w01_35-light1475496 20px → Jost 20px; Text color: #000000 → #19100c; Image placement: left, 33% wide → center, 100% wide; Image crop: 1:1 → 2.36:1 |
| 8 | WHERE YOU'LL be STAYING | 39 | Heading: forum 64px → Forum 80px; Text: avenir-lt-w01_35-light1475496 20px → Jost 20px; Columns: 5 → 1; Image placement: left, 42% wide → center, 89% wide; Image crop: 1.81:1 → 0.86:1; Height: 1616px → 11962px |
| 9 | (no heading) | 25 | Text: forum 36px → Jost 36px; Text color: #000000 → #19100c; Columns: 3 → 2 |
| 10 | (no heading) | 97 | Text: avenir-lt-w01_35-light1475496 46px → Jost 46px |
| 11 | (no heading) | 100 | — |
| 12 | (no heading) | 75 | Text: avenir-lt-w01_35-light1475496 30px → Jost 20px |
| 13 | (no heading) | 78 | Text: avenir-lt-w01_35-light1475496 22px → Jost 20px; Text color: #000000 → #f8f1ed |
| 14 | About me | 81 | Heading: forum 56px → Forum 80px; Text: avenir-lt-w01_35-light1475496 20px → Jost 20px |
| 15 | Frequently Asked Questions | 44 | Heading: forum 50px → Jost 50px; Text: avenir-lt-w01_35-light1475496 18px → Jost 10px; Text color: #ffffff → #19100c |

What would close the gap:

- choices.typography.scale.h2.size = 56
- choices.typography.scale.h3.size = 18
- Site Styles → choices.typography.body = { family: "avenir-lt-w01_35-light1475496" } (Google Fonts), or upload it in Site Styles → Your fonts.
- choices.typography.scale.lead.size = 25
- choices.layout.sectionPadding = 9
- Adjust the stack column spans (image column) or the image's side.
- Use the original's image proportions (the block's aspect ratio).
- Lay the text out in columns (a stack layout with more columns, or the text block's Columns style).

## /bloom-retreat-may-2024 at 1132px — 10/100 (strict v3: 4/100)

Corrected scoring on this page:

- Section 1: columns counted on screen only (2 → 1 counted as 1 → 1; what's off screen or inside one slideshow or map isn't a column).
- Section 2: columns counted on screen only (2 → 1 counted as 1 → 1; what's off screen or inside one slideshow or map isn't a column).
- Section 3: columns counted on screen only (2 → 1 counted as 1 → 1; what's off screen or inside one slideshow or map isn't a column).
- Section 5: columns counted on screen only (2 → 1 counted as 1 → 1; what's off screen or inside one slideshow or map isn't a column).
- Section 6: columns counted on screen only (3 → 1 counted as 1 → 1; what's off screen or inside one slideshow or map isn't a column).
- Section 7: columns counted on screen only (3 → 1 counted as 1 → 1; what's off screen or inside one slideshow or map isn't a column).
- Section 8: columns counted on screen only (5 → 1 counted as 1 → 1; what's off screen or inside one slideshow or map isn't a column).
- Section 9: columns counted on screen only (3 → 1 counted as 1 → 1; what's off screen or inside one slideshow or map isn't a column).
- Section 10: columns counted on screen only (3 → 1 counted as 1 → 1; what's off screen or inside one slideshow or map isn't a column).
- Section 13: columns counted on screen only (2 → 1 counted as 1 → 1; what's off screen or inside one slideshow or map isn't a column).
- Section 14: columns counted on screen only (2 → 1 counted as 1 → 1; what's off screen or inside one slideshow or map isn't a column).
- Section 15: columns counted on screen only (2 → 1 counted as 1 → 1; what's off screen or inside one slideshow or map isn't a column).

Checks passed: 57% · screenshots 53% alike (two unrelated pages compare at about 55%).

Original: https://www.courtneyacamo.com/bloom-retreat-may-2024  
Imported: /bloom-retreat-may-2024 (local preview)

| Check | Original | Imported | |
|---|---|---|---|
| Heading 1: present | forum 176px | not found | **differs** |
| Heading font | forum | Forum | same |
| Heading 2 size | 56px | 80px | **differs** |
| Heading 3 size | 18px | 42px | **differs** |
| Body font | avenir-lt-w01_35-light1475496 | Jost (close stand-in) | close (85%) |
| Body text size | 20px | 20px | same |
| Lead text size | 25px | 37px | **differs** |
| Navigation: present | forum 20px | not found | **differs** |
| Section padding | 8.5px | 23px | **differs** |

| # | Section | Match | Differences |
|---|---|---|---|
| 1 | Bloom | 60 | Heading: forum 176px → Jost 141px |
| 2 | You're Invited | 50 | Heading: forum 118px → Jost 94px; Text: avenir-lt-w01_35-light1475496 24px → Jost 19px; Image placement: center, 48% wide → center, 87% wide; Height: 316px → 610px |
| 3 | If you feel called to : | 42 | Heading: forum 52px → Jost 42px; Text: avenir-lt-w01_35-light1475496 20px → Jost 16px; Image placement: right, 57% wide → center, 87% wide; Image crop: 0.86:1 → 1.27:1; Height: 649px → 1172px |
| 4 | (no heading) | 100 | — |
| 5 | (no heading) | 78 | Text: avenir-lt-w01_35-light1475496 18px → Jost 20px; Height: 299px → 738px |
| 6 | Join the Journey | 72 | Text: avenir-lt-w01_35-light1475496 20px → Jost 20px; Image placement: left, 28% wide → center, 87% wide; Image crop: 0.38:1 → 0.66:1; Height: 725px → 1542px |
| 7 | (no heading) | 25 | Text: avenir-lt-w01_35-light1475496 20px → Jost 16px; Text color: #000000 → #19100c; Image placement: left, 48% wide → center, 100% wide; Image crop: 1:1 → 0.47:1; Height: 609px → 828px |
| 8 | WHERE YOU'LL be STAYING | 56 | Heading: forum 64px → Forum 80px; Text: avenir-lt-w01_35-light1475496 20px → Jost 20px; Image placement: left, 62% wide → center, 87% wide; Image crop: 1.81:1 → 0.86:1; Height: 1616px → 4164px |
| 9 | (no heading) | 50 | Text: forum 36px → Jost 29px; Text color: #000000 → #19100c |
| 10 | (no heading) | 60 | Text: avenir-lt-w01_35-light1475496 46px → Jost 37px; Image placement: left, 47% wide → center, 87% wide; Height: 580px → 1033px |
| 11 | (no heading) | 100 | — |
| 12 | (no heading) | 75 | Text: avenir-lt-w01_35-light1475496 30px → Jost 20px |
| 13 | (no heading) | 62 | Text: avenir-lt-w01_35-light1475496 22px → Jost 20px; Text color: #000000 → #f8f1ed; Height: 269px → 443px |
| 14 | About me | 56 | Heading: forum 56px → Forum 80px; Text: avenir-lt-w01_35-light1475496 20px → Jost 20px; Image placement: right, 50% wide → center, 87% wide; Image crop: 0.66:1 → 1.02:1; Height: 744px → 1349px |
| 15 | Frequently Asked Questions | 50 | Heading: forum 50px → Jost 40px; Text: avenir-lt-w01_35-light1475496 18px → Jost 14px |

What would close the gap:

- choices.typography.scale.h2.size = 56
- choices.typography.scale.h3.size = 18
- Site Styles → choices.typography.body = { family: "avenir-lt-w01_35-light1475496" } (Google Fonts), or upload it in Site Styles → Your fonts.
- choices.typography.scale.lead.size = 25
- choices.layout.sectionPadding = 9
- Adjust the stack column spans (image column) or the image's side.
- Use the original's image proportions (the block's aspect ratio).

## /challenges at 1440px — 10/100

Checks passed: 57% · screenshots 44% alike (two unrelated pages compare at about 55%).

Original: https://www.courtneyacamo.com/challenges  
Imported: /challenges (local preview)

| Check | Original | Imported | |
|---|---|---|---|
| Heading font | forum | Forum | same |
| Heading 1 size | 32px | 80px | **differs** |
| Label font | forum | Forum | same |
| Navigation size | 20px | 20px | same |
| Navigation letter spacing and case | 0em, none | 0em, none | same |
| Content width | 958px | 960px | same |
| Section padding | 156px | 25px | **differs** |

| # | Section | Match | Differences |
|---|---|---|---|
| 1 | Sound Medicine Course | 25 | Heading: forum 32px → Forum 80px; Columns: 4 → 1; Image placement: center, 100% wide → none; Height: 1062px → 228px |

What would close the gap:

- choices.typography.scale.h1.size = 32
- choices.layout.sectionPadding = 156
- Lay the text out in columns (a stack layout with more columns, or the text block's Columns style).
- Adjust the stack column spans (image column) or the image's side.

## /challenges at 1132px — 6/100

Checks passed: 29% · screenshots 65% alike (two unrelated pages compare at about 55%).

Original: https://www.courtneyacamo.com/challenges  
Imported: /challenges (local preview)

| Check | Original | Imported | |
|---|---|---|---|
| Heading font | forum | Forum | same |
| Heading 1 size | 32px | 40.9px | **differs** |
| Navigation: present | forum 20px | not found | **differs** |
| Content width | 1110px | 342px | **differs** |
| Section padding | 156px | 23px | **differs** |

| # | Section | Match | Differences |
|---|---|---|---|
| 1 | Sound Medicine Course | 25 | Heading: forum 32px → Forum 40.9px; Columns: 3 → 1; Image placement: center, 100% wide → none; Height: 1062px → 222px |

What would close the gap:

- choices.typography.scale.h1.size = 32
- choices.layout.contentWidth = 1110
- choices.layout.sectionPadding = 156
- Lay the text out in columns (a stack layout with more columns, or the text block's Columns style).
- Adjust the stack column spans (image column) or the image's side.

## /coming-soon-02 at 1440px — 8/100

Checks passed: 52% · screenshots 38% alike (two unrelated pages compare at about 55%).

Original: https://www.courtneyacamo.com/coming-soon-02  
Imported: /coming-soon-02 (local preview)

| Check | Original | Imported | |
|---|---|---|---|
| Heading font | forum | Forum | same |
| Heading 1 size | 56px | 80px | **differs** |
| Body font | avenir-lt-w01_35-light1475496 | Jost (close stand-in) | close (85%) |
| Body text size | 16px | 20px | **differs** |
| Label font | forum | Forum | same |
| Navigation size | 20px | 20px | same |
| Navigation letter spacing and case | 0em, none | 0em, none | same |
| Section padding | 63px | 50px | same |

| # | Section | Match | Differences |
|---|---|---|---|
| 1 | Medicine of the voice song circle | 25 | Background: #ffffff → #19100c; Heading: forum 56px → Forum 80px; Text: avenir-lt-w01_35-light1475496 16px → Jost 20px; Text color: #000000 → #f8f1ed; Image placement: right, 34% wide → center, 100% wide; Image crop: 0.62:1 → 1.68:1 |

What would close the gap:

- choices.typography.scale.h1.size = 56
- Site Styles → choices.typography.body = { family: "avenir-lt-w01_35-light1475496" } (Google Fonts), or upload it in Site Styles → Your fonts.
- choices.typography.scale.body.size = 16
- Give the section its own background color (style.background = { type: "color", color: "#ffffff" }).
- Adjust the stack column spans (image column) or the image's side.
- Use the original's image proportions (the block's aspect ratio).

## /coming-soon-02 at 1132px — 1/100

Checks passed: 27% · screenshots 58% alike (two unrelated pages compare at about 55%).

Original: https://www.courtneyacamo.com/coming-soon-02  
Imported: /coming-soon-02 (local preview)

| Check | Original | Imported | |
|---|---|---|---|
| Heading font | forum | Forum | same |
| Heading 1 size | 56px | 40.9px | **differs** |
| Body font | avenir-lt-w01_35-light1475496 | Jost (close stand-in) | close (85%) |
| Body text size | 16px | 20px | **differs** |
| Navigation: present | forum 20px | not found | **differs** |
| Section padding | 63px | 46px | **differs** |

| # | Section | Match | Differences |
|---|---|---|---|
| 1 | Medicine of the voice song circle | 8 | Background: #ffffff → #19100c; Heading: forum 56px → Forum 40.9px; Text: avenir-lt-w01_35-light1475496 16px → Jost 20px; Text color: #000000 → #f8f1ed; Columns: 2 → 1; Image placement: right, 50% wide → center, 100% wide; Image crop: 0.62:1 → 0.33:1 |

What would close the gap:

- choices.typography.scale.h1.size = 56
- Site Styles → choices.typography.body = { family: "avenir-lt-w01_35-light1475496" } (Google Fonts), or upload it in Site Styles → Your fonts.
- choices.typography.scale.body.size = 16
- choices.layout.sectionPadding = 63
- Give the section its own background color (style.background = { type: "color", color: "#ffffff" }).
- Lay the text out in columns (a stack layout with more columns, or the text block's Columns style).
- Adjust the stack column spans (image column) or the image's side.
- Use the original's image proportions (the block's aspect ratio).

## /contact-me at 1440px — 23/100 (strict v3: 19/100)

Corrected scoring on this page:

- Section 1: columns counted on screen only (3 → 1 counted as 1 → 1; what's off screen or inside one slideshow or map isn't a column).

Checks passed: 94% · screenshots 46% alike (two unrelated pages compare at about 55%).

Original: https://www.courtneyacamo.com/contact-me  
Imported: /contact-me (local preview)

| Check | Original | Imported | |
|---|---|---|---|
| Heading font | forum | Forum | same |
| Heading 2 size | 106px | 109px | same |
| Label font | forum | Forum | same |
| Navigation size | 20px | 20px | same |
| Navigation letter spacing and case | 0em, none | 0em, none | same |
| Section padding | 98px | 103.5px | same |

| # | Section | Match | Differences |
|---|---|---|---|
| 1 | Get in touch | 83 | Image placement: center, 89% wide → none |

What would close the gap:

- Adjust the stack column spans (image column) or the image's side.

## /contact-me at 1132px — 34/100 (strict v3: 28/100)

Corrected scoring on this page:

- Section 1: columns counted on screen only (2 → 1 counted as 1 → 1; what's off screen or inside one slideshow or map isn't a column).

Checks passed: 77% · screenshots 65% alike (two unrelated pages compare at about 55%).

Original: https://www.courtneyacamo.com/contact-me  
Imported: /contact-me (local preview)

| Check | Original | Imported | |
|---|---|---|---|
| Heading font | forum | Forum | same |
| Heading 2 size | 106px | 109px | same |
| Navigation: present | forum 20px | not found | **differs** |
| Section padding | 98px | 76px | same |

| # | Section | Match | Differences |
|---|---|---|---|
| 1 | Get in touch | 67 | Image placement: center, 100% wide → none; Height: 740px → 1048px |

What would close the gap:

- Adjust the stack column spans (image column) or the image's side.

## /copy-of-bloom-retreat-may-2024 at 1440px — 12/100

Checks passed: 63% · screenshots 54% alike (two unrelated pages compare at about 55%).

Original: https://www.courtneyacamo.com/copy-of-bloom-retreat-may-2024  
Imported: /copy-of-bloom-retreat-may-2024 (local preview)

| Check | Original | Imported | |
|---|---|---|---|
| Heading font | forum | Forum | same |
| Heading 1 size | 176px | 80px | **differs** |
| Heading 2 size | 64px | 80px | **differs** |
| Body font | avenir-lt-w01_35-light1475496 | Jost (close stand-in) | close (85%) |
| Body text size | 20px | 20px | same |
| Label font | forum | Forum | same |
| Navigation size | 20px | 20px | same |
| Navigation letter spacing and case | 0em, none | 0em, none | same |
| Section padding | 8.5px | 25px | **differs** |

| # | Section | Match | Differences |
|---|---|---|---|
| 1 | Bloom | 60 | Heading: forum 176px → Forum 80px |
| 2 | You're Invited | 42 | Text: avenir-lt-w01_35-light1475496 24px → Jost 20px; Columns: 2 → 1; Image placement: center, 33% wide → center, 89% wide; Image crop: 4.9:1 → 2.4:1; Height: 316px → 946px |
| 3 | If you feel called to : | 64 | Heading: forum 52px → Forum 80px; Text: avenir-lt-w01_35-light1475496 20px → Jost 20px; Image crop: 1.27:1 → 0.75:1; Height: 649px → 1253px |
| 4 | (no heading) | 100 | — |
| 5 | (no heading) | 78 | Text: avenir-lt-w01_35-light1475496 18px → Jost 20px; Height: 299px → 510px |
| 6 | Join the Journey | 89 | Text: avenir-lt-w01_35-light1475496 20px → Jost 20px; Image placement: left, 28% wide → right, 27% wide |
| 7 | (no heading) | 34 | Text: avenir-lt-w01_35-light1475496 20px → Jost 20px; Text color: #000000 → #f8f1ed; Columns: 3 → 2; Image placement: left, 33% wide → center, 100% wide; Height: 609px → 1611px |
| 8 | WHERE YOU'LL be STAYING | 39 | Heading: forum 64px → Forum 80px; Text: avenir-lt-w01_35-light1475496 20px → Jost 20px; Columns: 5 → 1; Image placement: left, 42% wide → center, 89% wide; Image crop: 1.81:1 → 0.86:1; Height: 1616px → 11962px |
| 9 | (no heading) | 17 | Text: forum 36px → Jost 20px; Text color: #000000 → #f8f1ed; Columns: 3 → 2 |
| 10 | (no heading) | 40 | Text: avenir-lt-w01_35-light1475496 46px → Jost 20px; Columns: 3 → 1; Image placement: center, 32% wide → center, 89% wide; Height: 580px → 1861px |
| 11 | (no heading) | 100 | — |
| 12 | (no heading) | 75 | Text: avenir-lt-w01_35-light1475496 30px → Jost 20px |
| 13 | (no heading) | 78 | Text: avenir-lt-w01_35-light1475496 22px → Jost 20px; Text color: #000000 → #f8f1ed |
| 14 | About me | 81 | Heading: forum 56px → Forum 80px; Text: avenir-lt-w01_35-light1475496 20px → Jost 20px |
| 15 | (no heading) | 100 | — |

What would close the gap:

- choices.typography.scale.h1.size = 176
- choices.typography.scale.h2.size = 64
- Site Styles → choices.typography.body = { family: "avenir-lt-w01_35-light1475496" } (Google Fonts), or upload it in Site Styles → Your fonts.
- choices.layout.sectionPadding = 9
- Lay the text out in columns (a stack layout with more columns, or the text block's Columns style).
- Adjust the stack column spans (image column) or the image's side.
- Use the original's image proportions (the block's aspect ratio).

## /copy-of-bloom-retreat-may-2024 at 1132px — 11/100 (strict v3: 5/100)

Corrected scoring on this page:

- Section 1: columns counted on screen only (2 → 1 counted as 1 → 1; what's off screen or inside one slideshow or map isn't a column).
- Section 2: columns counted on screen only (2 → 1 counted as 1 → 1; what's off screen or inside one slideshow or map isn't a column).
- Section 3: columns counted on screen only (2 → 1 counted as 1 → 1; what's off screen or inside one slideshow or map isn't a column).
- Section 5: columns counted on screen only (2 → 1 counted as 1 → 1; what's off screen or inside one slideshow or map isn't a column).
- Section 6: columns counted on screen only (3 → 1 counted as 1 → 1; what's off screen or inside one slideshow or map isn't a column).
- Section 7: columns counted on screen only (3 → 1 counted as 1 → 1; what's off screen or inside one slideshow or map isn't a column).
- Section 8: columns counted on screen only (5 → 1 counted as 1 → 1; what's off screen or inside one slideshow or map isn't a column).
- Section 9: columns counted on screen only (3 → 1 counted as 1 → 1; what's off screen or inside one slideshow or map isn't a column).
- Section 10: columns counted on screen only (3 → 1 counted as 1 → 1; what's off screen or inside one slideshow or map isn't a column).
- Section 13: columns counted on screen only (2 → 1 counted as 1 → 1; what's off screen or inside one slideshow or map isn't a column).
- Section 14: columns counted on screen only (2 → 1 counted as 1 → 1; what's off screen or inside one slideshow or map isn't a column).

Checks passed: 62% · screenshots 53% alike (two unrelated pages compare at about 55%).

Original: https://www.courtneyacamo.com/copy-of-bloom-retreat-may-2024  
Imported: /copy-of-bloom-retreat-may-2024 (local preview)

| Check | Original | Imported | |
|---|---|---|---|
| Heading font | forum | Forum | same |
| Heading 1 size | 176px | 40.9px | **differs** |
| Heading 2 size | 64px | 80px | **differs** |
| Body font | avenir-lt-w01_35-light1475496 | Jost (close stand-in) | close (85%) |
| Body text size | 20px | 20px | same |
| Navigation: present | forum 20px | not found | **differs** |
| Section padding | 8.5px | 23px | **differs** |

| # | Section | Match | Differences |
|---|---|---|---|
| 1 | Bloom | 60 | Heading: forum 176px → Forum 40.9px |
| 2 | You're Invited | 42 | Heading: forum 118px → Forum 54.6px; Text: avenir-lt-w01_35-light1475496 24px → Jost 20px; Image placement: center, 48% wide → center, 87% wide; Image crop: 4.9:1 → 2.4:1; Height: 316px → 520px |
| 3 | If you feel called to : | 64 | Heading: forum 52px → Forum 80px; Text: avenir-lt-w01_35-light1475496 20px → Jost 20px; Image placement: right, 57% wide → center, 87% wide; Height: 649px → 1980px |
| 4 | (no heading) | 100 | — |
| 5 | (no heading) | 78 | Text: avenir-lt-w01_35-light1475496 18px → Jost 20px; Height: 299px → 738px |
| 6 | Join the Journey | 72 | Text: avenir-lt-w01_35-light1475496 20px → Jost 20px; Image placement: left, 28% wide → center, 87% wide; Image crop: 0.38:1 → 0.66:1; Height: 725px → 1542px |
| 7 | (no heading) | 46 | Text: avenir-lt-w01_35-light1475496 20px → Jost 20px; Text color: #000000 → #f8f1ed; Image placement: left, 48% wide → center, 100% wide; Image crop: 1:1 → 0.45:1; Height: 609px → 864px |
| 8 | WHERE YOU'LL be STAYING | 56 | Heading: forum 64px → Forum 80px; Text: avenir-lt-w01_35-light1475496 20px → Jost 20px; Image placement: left, 62% wide → center, 87% wide; Image crop: 1.81:1 → 0.86:1; Height: 1616px → 4164px |
| 9 | (no heading) | 50 | Text: forum 36px → Jost 20px; Text color: #000000 → #f8f1ed |
| 10 | (no heading) | 60 | Text: avenir-lt-w01_35-light1475496 46px → Jost 20px; Image placement: left, 47% wide → center, 87% wide; Height: 580px → 905px |
| 11 | (no heading) | 100 | — |
| 12 | (no heading) | 75 | Text: avenir-lt-w01_35-light1475496 30px → Jost 20px |
| 13 | (no heading) | 62 | Text: avenir-lt-w01_35-light1475496 22px → Jost 20px; Text color: #000000 → #f8f1ed; Height: 269px → 443px |
| 14 | About me | 56 | Heading: forum 56px → Forum 80px; Text: avenir-lt-w01_35-light1475496 20px → Jost 20px; Image placement: right, 50% wide → center, 87% wide; Image crop: 0.66:1 → 1.02:1; Height: 744px → 1349px |
| 15 | (no heading) | 100 | — |

What would close the gap:

- choices.typography.scale.h1.size = 176
- choices.typography.scale.h2.size = 64
- Site Styles → choices.typography.body = { family: "avenir-lt-w01_35-light1475496" } (Google Fonts), or upload it in Site Styles → Your fonts.
- choices.layout.sectionPadding = 9
- Adjust the stack column spans (image column) or the image's side.
- Use the original's image proportions (the block's aspect ratio).

