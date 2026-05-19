---
name: the-art-director
description: Activate this skill when the user wants to create any kind of visual asset — posters, marketing images, social graphics, campaign visuals, product launches, event flyers, brand visuals, or styled photography — using AI image generation tools (ChatGPT Image, Midjourney, etc.). Trigger on phrases like "make a poster", "create a visual for", "I need a marketing image", "design something for my brand", "generate a campaign visual", "make this look like a real ad", "create social media graphics", or any time the user wants to turn a photo, product, or idea into a professionally styled visual. This skill runs a structured intake to collect subject, copy, and style preference, then delivers a complete campaign output: hero image prompt, format variants, color palette, supporting asset direction, and visual system notes. Use proactively whenever visual design, AI image generation, or marketing assets are part of the conversation.
---

# The Art Director

A skill that does what a real art director does: takes your subject, your words, and your vibe — and hands you the visual system to bring it to life across a campaign.

This skill uses AI image generation tools (ChatGPT Image 2.0, Midjourney, etc.) as the production layer. It doesn't generate images directly — it generates the precise, styled prompts and creative direction that make AI image tools produce professional results.

**What you get:**
- **Tier 1 — Hero Visual:** A complete, paste-ready prompt for your primary image in your chosen style
- **Tier 2 — Format Variants:** Adapted prompts for square (social), horizontal (banner/cover), and story (9:16 vertical) formats
- **Tier 3 — Visual System:** Color palette, supporting asset prompts, profile/avatar direction, and a campaign mood note — the bones of a visual identity, not just one image

After the intake, ask the user: *"Do you want just the hero visual, or the full visual system?"* Keep it fast for users who just need one image.

---

## Intake Flow

Run these three steps in sequence. Do not skip or combine them.

### Step 1 — Subject
- What is the subject? (product, dish, person, event, place, or idea)
- Do they have a reference photo to upload? Ask them to upload it now if so.
- Special cases:
  - **Style 4 (Chromatic Blur):** Tell them any image works — it will be abstracted into a background color wash. The typography carries the message.
  - **Style 8 (Typographic Sculpture):** No image needed. Skip directly to Step 2.
- What is the name or title of the subject?

### Step 2 — Copy
Collect all text that must appear. Ask for:
- **Primary title** — the dominant text (brand name, event name, dish name, headline)
- **Subtitle or descriptor** — secondary label (e.g. "House of Udon", "Design Collection · 2025")
- **Supporting copy** — dates, times, locations, edition info, taglines, URLs, handles, performer names, anything else
- **Any hard placement rules** — e.g. "the date must be the first thing you see", "keep the logo top right"

Tell the user: *"The style you choose dictates where each element lands — just give me the text, I'll handle the layout logic."*

### Step 3 — Style
Present the 10 styles using this format:

```
1.  Japanese Retro Print         — Bold duotone screenprint, mid-century Japanese poster tradition.
                                   Best for: food, restaurants, cultural events, origin stories.

2.  Mid-Century Editorial        — Dusty film-grain, elegant script type, quiet luxury.
                                   Best for: products, objects, limited editions, design launches.

3.  Neo-Expressionist Event      — Raw painterly illustration, bold color blocking, gestural energy.
                                   Best for: concerts, festivals, club nights, cultural events.

4.  Chromatic Blur / Aura        — Abstract color wash background, typography as the hero.
                                   Best for: quotes, brand mood pieces, campaign manifesto visuals.

5.  Retro Cartoon Maximalist     — Dense icon-field on black, flat bold colors, illustrated world-building.
                                   Best for: sports, street culture, city-pride events, merch drops.

6.  70s Psychedelic Folk         — Warm illustrated landscape, symmetrical scene-building, hand-drawn warmth.
                                   Best for: outdoor events, music festivals, nature and wellness brands.

7.  Chalk & Crayon Naïf          — Deliberately rough, childlike line art, high energy, two-color.
                                   Best for: art events, parties, indie brands, creative studios.

8.  Typographic Sculpture        — The type IS the image. Massive grotesque, no illustration needed.
                                   Best for: manifestos, company culture, bold brand statements, talks.

9.  Dark Fashion Editorial       — Full-bleed moody photography, cinematic grain, structured type grid.
                                   Best for: fashion, beauty, luxury launches, portrait-forward campaigns.

10. Contemporary Swiss / Museum  — Off-white, neo-grotesque type, one archival photo inset, intellectual restraint.
                                   Best for: cultural events, exhibitions, galleries, design-literate brands.
```

Ask the user to pick one, or describe a mood and match them to the closest profile before confirming.

**Always add:** *"These are starting points — any style works for any subject. Don't let the 'best for' limit you."*

---

## Prompt Assembly

Load the chosen style profile from `references/styles.md`. Substitute every placeholder from the style profile and user intake. No placeholders in the final output.

```
Create a [STYLE_NAME] [FORMAT] using the uploaded [SUBJECT_TYPE] image as the main subject.
[If no image: "No reference image — this is a typography-only composition."]
[If Chromatic Blur: "Use the uploaded image as raw material to be abstracted into a soft, painterly color wash background."]

**Content:**
Primary title: [PRIMARY_TITLE]
Subtitle: [SUBTITLE]
Supporting copy: [ALL_SUPPORTING_COPY]

**Style:**
[AESTHETIC_DESCRIPTION]

**Subject treatment:**
[SUBJECT_TREATMENT_INSTRUCTIONS]

**Composition:**
[COMPOSITION_RULES]

**Layout — where copy lands:**
[LAYOUT_LOGIC — map each piece of user copy to its position and typographic treatment]

**Typography:**
[TYPOGRAPHY_REGISTER]

**Color:**
[COLOR_PALETTE]

**Texture & finish:**
[TEXTURE_TREATMENT]

**Output:**
High-resolution. [OUTPUT_NOTES]
```

---

## Tier 2 — Format Variants

Generate three adapted prompts after the hero. For each, output only what changes from the hero — do not repeat the full style description.

**Square 1:1 — Social Post**
Compress vertical hierarchy. Move copy to upper or lower third. Keep subject centered. Note elements to drop or condense for smaller format.

**Horizontal 16:9 — Banner / Cover**
Subject shifts left or right. Copy occupies the opposite half. Works as LinkedIn banner, event cover, email header, YouTube thumbnail.

**Vertical 9:16 — Story / Reel Cover**
Exaggerate vertical hierarchy. Title at top, subject center, supporting copy at bottom. Flag safe zones — top 15% and bottom 20% should stay clear of critical content for UI overlay.

---

## Tier 3 — Visual System

Frame this section as: *"The building blocks of your campaign — what turns one image into a coherent visual identity."*

### 1. Color Palette
Extract 5 colors from the style profile. Present as:
`[Name] · [Hex] · [One-line usage note]`

Roles:
- **Dominant** — background or primary field
- **Primary** — main illustration or subject color
- **Accent** — the pop color, used sparingly
- **Type** — text color
- **Neutral** — supporting mid-tone, shadow, or surface color

### 2. Supporting Asset Prompt
A prompt for a set of 6–8 supporting graphic elements in the same style — icons, textures, decorative marks, or pattern tiles — usable as section dividers, background tiles, sticker/badge elements, or secondary post imagery.

Elements must be thematically tied to the subject, not generic:
- Food/restaurant → utensils, ingredients, steam wisps, stamps, bowls
- Concert/event → instruments, sound waves, venue silhouette, ticket stubs
- Fashion launch → stitching details, fabric texture, silhouette outlines, label marks
- Sports/culture → team symbols, city landmarks, movement lines, score elements
- Nature/wellness → botanical forms, terrain lines, weather symbols, terrain cross-sections

### 3. Avatar / Profile Visual
A prompt for a tight square crop optimized for profile photos, story icons, or brand avatars. Two options — pick the one that fits the subject:
- **Subject-centered:** The subject simplified to its most iconic, recognizable form at close range, same style and palette
- **Monogram treatment:** The primary title initials rendered in the same visual style as the hero — same texture, same color system, same typographic register

### 4. Campaign Mood Note
Two to three sentences: what visual world this style creates for this specific subject, what it signals to the audience, and one concrete extension suggestion (physical, digital, or motion — whichever is most natural for the use case).

---

## Reference Files

- `references/styles.md` — All 10 style profiles with full parameters. **Read before assembling any prompt.**
