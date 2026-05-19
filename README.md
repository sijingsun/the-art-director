# The Art Director

Turn any subject — a dish, a product, an event, an idea — into a professional AI-generated visual campaign. Choose from 18 curated poster styles, and get a complete paste-ready prompt for ChatGPT Image or Midjourney, plus format variants, a color palette, and supporting asset direction. No design experience needed — just tell it what you're making.

---

## 18 Styles at a Glance

**→ Open [STYLES.html](STYLES.html) for the visual style reference** — hover any card for best-use notes.

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

- **Tier 1 — Hero prompt:** Complete, paste-ready prompt for ChatGPT Image or Midjourney
- **Tier 2 — Format variants:** Square (social), horizontal (banner/cover), vertical (story/reel)
- **Tier 3 — Visual system:** 5-color palette, supporting asset prompts, avatar/profile crop direction, campaign mood note

---

## Files

| File | Purpose |
|------|---------|
| `SKILL.md` | Intake flow, prompt assembly logic, three-tier output system |
| `references/styles.md` | All 18 style profiles — typography geometry, composition, palette, texture |
| `gpt-system-prompt.md` | System prompt for Custom GPT setup |
| `STYLES.html` | Visual style reference — open in browser to preview all 18 styles |

---

## Usage

### Claude Code

```bash
git clone https://github.com/sijingsun/the-art-director
cp -r the-art-director ~/.claude/skills/
```

Then invoke directly:
```bash
/the-art-director
```
Or just describe what you're making — it triggers automatically.

### Custom GPT (ChatGPT)

1. Paste contents of `gpt-system-prompt.md` into the GPT Instructions field
2. Upload `SKILL.md` and `references/styles.md` as knowledge files
3. Enable DALL-E Image Generation
4. Add conversation starter chips: *"Make a poster for my restaurant"*, *"Show me the 18 styles"*, *"I have a product launch"*

### Regular ChatGPT conversation

Upload `SKILL.md`, `references/styles.md`, and `gpt-system-prompt.md`, then send:
```
Greet me as The Art Director.
```

---

## By

Clair Sun — [clairsun.design](https://clairsun.design)
