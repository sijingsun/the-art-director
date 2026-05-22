# The Art Director

Turn any subject — a dish, a product, an event, an idea — into a professional AI-generated visual campaign. Choose from 18 curated poster styles and get a complete paste-ready prompt for ChatGPT Image, Midjourney, or any modern image generator, plus format variants, a color palette, and supporting asset direction. No design experience needed — just tell it what you're making.

**[Browse all 18 styles in the visual gallery →](https://sijingsun.github.io/the-art-director/STYLES.html)**

---

## 18 Styles at a Glance

| # | Style | Feels like |
|---|-------|------------|
| 1 | Japanese Retro Print | Screen-printed food stall poster, 1960s Osaka |
| 2 | Mid-Century Editorial | Page from a 1972 design magazine |
| 3 | Neo-Expressionist Event | Wheat-pasted festival poster, contemporary Berlin |
| 4 | Chromatic Blur / Aura | Abstract color wash, typography as the whole message |
| 5 | Retro Cartoon Maximalist | Limited-edition sports merch drop |
| 6 | 70s Psychedelic Folk | Grateful Dead meets national park print |
| 7 | Chalk & Crayon Naïf | Art party flyer made by someone with great taste |
| 8 | Typographic Sculpture | Manifesto printed on a wall — type IS the image |
| 9 | Dark Fashion Editorial | A24 film poster meets luxury fashion campaign |
| 10 | Contemporary Swiss / Museum | Something MoMA would mail you |
| 11 | Blueprint Core | A ramen bowl deconstructed into 47 labeled parts |
| 12 | Archival Trinket | A museum specimen sheet of your most meaningful objects |
| 13 | Punk Grunge | Photocopied three times, wheat-pasted over something else |
| 14 | Future Medieval | A cathedral rebuilt inside a server room |
| 15 | Surveillance Design | CCTV still of someone who didn't know they were watched |
| 16 | Signal Aesthetic | Saturday morning TV intro, frozen mid-frame |
| 17 | Frutiger Aero | Windows XP default wallpaper as prophecy |
| 18 | Type Collage | A zine page that went to art school |

Styles 11–18 based on [Kittl's 2026 Graphic Design Trend Report](https://www.kittl.com/blogs/graphic-design-trends-2026/).

---

## What you get

For every project, the skill produces:

- **Tier 1 — Hero prompt:** A complete, paste-ready prompt for ChatGPT Image, Midjourney, or any image generator that accepts a text prompt plus a reference image.
- **Tier 2 — Format variants:** Square (1:1 social), horizontal (16:9 banner/cover), vertical (9:16 story/reel).
- **Tier 3 — Visual system:** 5-color palette, supporting asset prompts, avatar/profile crop direction, campaign mood note.

**Every hero prompt is paired with the matching reference image to attach in your image generator.** Text alone produces drift; the reference image anchors the visual style. This pairing is the single biggest reason the skill produces consistent on-style results.

---

## How it works

1. Drop the folder into your AI assistant — Claude, ChatGPT with file uploads, or any agent that can read files and view images.
2. Activate the skill (see *Quick Start* below).
3. Pick a style — browse the [online gallery](https://sijingsun.github.io/the-art-director/STYLES.html), open `STYLES.html` locally, or ask the AI to show you the styles inline.
4. Tell the AI your subject, copy, and any hard placement rules.
5. Receive the prompt plus an explicit "attach this reference image" instruction.
6. Open ChatGPT Image 2.0 (or Midjourney, or your image tool of choice). Paste the prompt, attach the named `.jpg`, generate.

---

## Quick Start

### Any AI assistant (Claude, ChatGPT, etc.)

Download or clone this repo, attach the entire folder to your AI assistant, then send this activation prompt:

```
I've attached the The Art Director skill folder.

1. Read SKILL.md end-to-end — that's your operating manual.
2. Load references/styles.md so all 18 style profiles are ready.
3. Note the 18 reference images in references/images/.
4. Your first reply should be the Dual Entry opening from SKILL.md, exactly as written.

Follow the workflow strictly: never assemble a prompt before intake (subject + copy + style) is complete, always include the Reference Image Delivery block with every hero prompt, and show me the matching reference image inline when I pick a style.
```

### Claude Code

```bash
git clone https://github.com/sijingsun/the-art-director ~/.claude/skills/the-art-director
```

Then describe what you're making — the skill triggers automatically.

---

## Files

| File / Folder | Purpose |
|---|---|
| `SKILL.md` | Operating manual — intake flow, prompt assembly, three-tier output, anti-drift rules |
| `references/styles.md` | All 18 style profiles — reference anatomy lock, typography geometry, composition, palette, texture, style-specific negative prompts |
| `references/images/` | 18 reference images (`style-NN-name.jpg`), one per style. Attach the matching `.jpg` to your image generator alongside the prompt. |
| `STYLES.html` | Single-page visual browser of all 18 styles. Openable locally; also served at the [public gallery URL](https://sijingsun.github.io/the-art-director/STYLES.html). |

---

## Why reference images matter

ChatGPT Image 2.0 and most modern image generators produce dramatically better, more consistent results when you give them a reference image alongside the text prompt. Text describes the structure; the image teaches the model what the style actually looks like.

Every hero prompt the skill produces comes with an explicit "attach this image" instruction naming the matching file in `references/images/`. Skip the attachment and the model will drift toward its own interpretation of "moody fashion editorial" or "psychedelic folk poster" — which is rarely what you want.

---

## By

Clair Sun — [clairsun.design](https://clairsun.design)
