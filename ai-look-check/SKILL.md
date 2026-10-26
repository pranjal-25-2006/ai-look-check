---
name: ai-look-check
description: Check whether a website or landing page looks AI-made, give it an AI-look score out of 100 with every giveaway listed, then fix them. Use when someone says "does my site look AI-made", "make this look less AI", "audit my landing page design", "my vibe-coded site looks generic", "fix the design", or shares HTML, a URL, a screenshot or a repo of a site built with Claude, Lovable, Bolt, v0 or Cursor.
---

# AI-look check

Two jobs, always in this order: **Check** (score + list of giveaways), then **Fix** (only after showing the check).
Never invent facts about the business while fixing. Missing real content becomes a `[placeholder]` the owner fills in.

## 1. Check

Read the page (HTML/CSS, a screenshot, or the live URL). For each giveaway below, mark it **present** or **not present** and
note where (selector, section or line). Score = 100 minus the points of every giveaway present (minimum 0).

| # | Giveaway | Points |
|---|---|---|
| 1 | Purple / blue / pink gradient hero or gradient text headline | 10 |
| 2 | Hype copy: "unlock", "elevate", "seamless", "revolutionize", "supercharge", "in today's fast-paced world", "next level" | 10 |
| 3 | Numbers nobody can check: "10,000+ happy customers", "99% satisfaction", "trusted by thousands", with no source | 10 |
| 4 | Three (or six) identical feature cards: icon + bold title + one vague sentence | 8 |
| 5 | Emoji used as icons or bullets (🚀 ✨ 💡 ⚡ ✅) | 6 |
| 6 | Fake or placeholder testimonials ("Sarah J., CEO", lorem ipsum, stock avatars with no real names) | 8 |
| 7 | Everything centred, every section the same width and rhythm | 6 |
| 8 | One font at a few sizes, no real type scale (h1 barely bigger than body, or 5+ random sizes) | 6 |
| 9 | Glass cards, glows, blur and big shadows on everything | 6 |
| 10 | Random spacing (padding and gaps not on one scale) | 5 |
| 11 | More than one accent colour fighting for attention | 5 |
| 12 | Generic CTA repeated: "Get Started", "Learn More", "Join now" with no specific outcome | 5 |
| 13 | Headline that could fit any business ("Your partner for success") | 7 |
| 14 | No real photo of the actual product, place or people | 5 |
| 15 | Dead footer: links to "#", "Careers", "Blog" pages that don't exist | 3 |

Report like this:

```
AI-look score: 23/100  (100 = looks hand-made)
Giveaways found (11):
- [#1, 10 pts] hero has a purple-to-blue gradient (section.hero)
- ...
Top 3 fixes that move the score most: ...
```

## 2. Fix

Fix every giveaway present, biggest points first. Keep the owner's real content, structure and brand colour if they have one.

- **Colour:** one neutral background, one ink colour, ONE accent used for the main button and maybe one highlight. No gradients unless it's the brand.
- **Type:** two fonts at most (a display face for headings, a readable text face). A clear scale, e.g. 56 / 32 / 20 / 16 px. Tighter letter-spacing on big headings.
- **Spacing:** one scale (4, 8, 16, 24, 32, 48, 64, 96). Use it for every gap and padding.
- **Layout:** break the symmetry. Left-aligned hero with text one side and the real photo the other, a list instead of three cards, one section that is visually different.
- **Copy:** say what the business actually does, for whom, where, and the price or next step. Replace hype words with plain, specific ones. Swap unverifiable numbers for real ones the owner gives you, or remove them.
- **Proof:** real reviews with real names and the place they came from (Google, Zomato...), or a `[paste 2 real reviews here]` placeholder. Never write fake ones.
- **Icons:** drop emoji. Use a real photo, a simple line icon set, or nothing.
- **CTA:** one specific action ("Order a cake for Saturday", "Book a 15-minute call"), repeated at most twice.
- **Footer:** only links that work: address, hours, phone/WhatsApp, map, Instagram.

Then run the Check again on the result and show **before score -> after score** and what's still left.

## Rules
- Don't redesign the brand from scratch; remove the generic AI layer.
- Don't add stock photos pretending to be the business. Ask for a real photo or leave a clearly marked placeholder.
- Accessibility stays: text contrast at least 4.5:1, buttons at least 44 px tall, real alt text.
