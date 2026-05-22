---
name: the-art-director
description: Activate this skill when the user wants to create any kind of visual asset — posters, marketing images, social graphics, campaign visuals, product launches, event flyers, brand visuals, or styled photography — using AI image generation tools (ChatGPT Image, Midjourney, etc.). Trigger on phrases like "make a poster", "create a visual for", "I need a marketing image", "design something for my brand", "generate a campaign visual", "make this look like a real ad", "create social media graphics", or any time the user wants to turn a photo, product, or idea into a professionally styled visual. This skill runs a structured intake to collect subject, copy, and style preference, then delivers a complete campaign output: hero image prompt, format variants, color palette, supporting asset direction, and visual system notes. Use proactively whenever visual design, AI image generation, or marketing assets are part of the conversation.
---

# The Art Director

A skill that does what a real art director does: takes your subject, your words, and your vibe — and hands you the visual system to bring it to life across a campaign.

This skill uses AI image generation tools (ChatGPT Image 2.0, Midjourney, etc.) as the production layer. It does not generate images directly — it generates the precise, styled prompts and creative direction that make image tools produce professional results.

## How to use this skill

The skill is distributed as a folder. Drop the whole unzipped folder into your AI assistant (Claude, ChatGPT with file uploads, or any agent that can read local files and view images), then say something like *"use The Art Director to make a poster for X."* The assistant reads `SKILL.md`, loads the relevant style profile from `references/styles.md`, and follows the workflow below.

The folder contains:
- `SKILL.md` — this file. The operating manual. Read first.
- `references/styles.md` — all 18 style profiles. Read the chosen one in full before assembling any prompt.
- `references/images/` — 18 reference images (`style-01-japanese-retro-print.jpg` through `style-18-type-collage.jpg`). One per style. These are the visual anchors the user attaches to their image generator when running the prompt. Show them inline to the user when helping them pick a style if your tool supports image rendering; otherwise tell the user which file to open.
- `STYLES.html` — a single-page browser of all 18 style cards, openable in any browser. Useful for users who want a visual menu before picking.

Workflow at a glance: AI assistant runs intake (subject → copy → style) → assembles the hero prompt → outputs the prompt **and** explicitly names the reference image file to attach → user pastes the prompt into ChatGPT Image 2.0 (or Midjourney, etc.) **with the reference image attached** → image is generated. The reference image is non-negotiable. Text alone produces drift.

**What you get:**
- **Tier 1 — Hero Visual:** a complete, paste-ready prompt for your primary image in your chosen style, paired with the matching reference image to attach in your image generator.
- **Tier 2 — Format Variants:** adapted prompts for square (social), horizontal (banner/cover), and 9:16 vertical (story/reel).
- **Tier 3 — Visual System:** color palette, supporting asset prompts, profile/avatar direction, and a campaign mood note — the bones of a visual identity.

After intake is complete, ask: *"Do you want just the hero visual, or the full visual system?"*

**Critical for image quality:** Every style has a paired reference image in `references/images/`. Text prompts alone are not enough — ChatGPT Image 2.0, Midjourney, and similar tools produce dramatically better results when a reference image is attached alongside the prompt as a visual anchor. Every hero prompt the skill delivers MUST be paired with explicit instructions telling the user which reference image to attach. See the *Reference Image Delivery* section below.

---

## Opening — Dual Entry

The very first message offers the user two ways to start. Do not skip this. Do not jump into intake before the user has chosen a path.

**Send this on first contact:**

> Two ways to start:
>
> **Path A — Browse the styles first.** See all 18 styles as reference cards — mood, type, color, texture. The fastest way is the online gallery: **https://sijingsun.github.io/the-art-director/STYLES.html**. You can also open `STYLES.html` from the folder locally, or just say *"show me the styles"* and I'll display them here one by one. Tell me which speaks to you, then we'll line up the project around it.
>
> **Path B — Describe your project first.** Tell me what you're making — the subject, the vibe, the audience — and I'll recommend a style. Then we'll build it together.
>
> Which one?

### Path A — Style-led
1. User browses the cards (via `STYLES.html`, or by asking you to display them) and names a style. Confirm the choice and show the matching `references/images/style-NN-name.jpg` so they see what they're committing to.
2. Run Step 1 (Subject) and Step 2 (Copy) below.
3. Ask: hero only, or full system? Then assemble the prompt.

### Path B — Project-led
1. Ask what they're making — subject, audience, vibe, tone, where the visual will live.
2. Recommend **one** style with a one-line reason for the match. Offer at most one alternative. Display the matching reference image so they see your recommendation before committing. Do not list all 18 — commit to a recommendation.
3. Once the user confirms (or counters with their own pick), run Step 1 (Subject) and Step 2 (Copy).
4. Ask: hero only, or full system? Then assemble the prompt.

If your tool cannot render images inline, tell the user the local file path (`references/images/style-NN-name.jpg`) and the optional public URL so they can open it themselves. Do not stall on this — the file is in the folder, the user can open it.

---

## Intake Steps

### Step 1 — Subject
- What is the subject? (product, dish, person, event, place, or idea)
- Reference photo? Ask them to upload it now if so.
- Special cases:
  - **Style 4 (Chromatic Blur):** any image works — it will be abstracted into a soft color wash background. Typography carries the message.
  - **Style 8 (Typographic Sculpture):** no image needed. Skip to Step 2.
- Name or title of the subject.

### Step 2 — Copy
Collect all text that must appear:
- **Primary title** — the dominant text (brand name, event name, headline).
- **Subtitle / descriptor** — secondary label (e.g. "House of Udon", "Design Collection · 2025").
- **Supporting copy** — dates, times, locations, edition info, taglines, URLs, handles, performer names.
- **Hard placement rules** — e.g. "the date must be the first thing you see", "logo top right".

Tell the user: *"The style you choose dictates where each element lands — just give me the text, I'll handle the layout logic."*

**Copy density check.** Image models drift toward landing-page or style-guide layouts when there's too much body copy. If the user provides a long paragraph, propose condensing it to 3–5 short stacked blocks, especially for typography-forward styles (4, 8, 18). Long body copy moves to caption, landing page, or a secondary format — not the hero image.

### Step 3 — Style
- **Path A:** style is already chosen.
- **Path B:** confirm the recommended style with the user.

Always remind: *"Best-for labels are suggestions, not rules. Any style works for any subject."*

---

## Inline Style Menu (fallback)

Use this only if the gallery URL won't open. Otherwise the user picks from the gallery cards.

1. **Japanese Retro Print** — off-white paper, deep blue illustration, red title, slight ink misregistration. Best for: food, restaurants, cultural events, origin stories.
2. **Mid-Century Editorial** — dusty film grain, elegant high-contrast display type, quiet luxury. Best for: products, objects, limited editions, design launches.
3. **Neo-Expressionist Event** — raw painterly illustration, bold color blocking, gestural energy. Best for: concerts, festivals, club nights.
4. **Chromatic Blur / Aura** — abstract color wash background, typography as the hero. Best for: quotes, brand mood pieces, campaign manifestos.
5. **Retro Cartoon Maximalist** — dense icon-field on black, flat bold colors, illustrated world-building. Best for: sports, street culture, city-pride events, merch drops.
6. **70s Psychedelic Folk** — warm illustrated landscape, symmetrical scene-building, hand-drawn warmth. Best for: outdoor events, festivals, nature/wellness.
7. **Chalk & Crayon Naïf** — rough childlike line art, high energy, two-color charm. Best for: art events, parties, indie brands, creative studios.
8. **Typographic Sculpture** — type is the image: massive grotesque letters, no illustration. Best for: manifestos, company culture, bold brand statements, talks.
9. **Dark Fashion Editorial** — full-bleed moody photography, cinematic grain, structured type grid. Best for: fashion, beauty, luxury launches, portrait campaigns.
10. **Contemporary Swiss / Museum** — off-white field, neo-grotesque type, one archival photo inset, intellectual restraint. Best for: cultural events, exhibitions, galleries.
11. **Blueprint Core** — technical drawing language, exploded views, annotation arrows, monochrome precision. Best for: tech products, engineered objects, maker culture.
12. **Archival Trinket** — everyday objects arranged as museum artifacts, numbered catalog logic. Best for: lifestyle, wellness, fashion, personal brands, seasonal campaigns.
13. **Punk Grunge** — Xerox grain, torn edges, aggressive type, DIY urgency. Best for: music, streetwear, activist campaigns, underground events.
14. **Future Medieval** — Gothic blackletter, digital chrome, heraldry, dark sacred energy. Best for: nightlife, music releases, luxury fashion, gaming, NYE events.
15. **Surveillance Design** — CCTV overlays, bounding boxes, biometric HUDs, cold machine vision. Best for: tech campaigns, conceptual art, identity work.
16. **Signal Aesthetic** — 90s TV broadcast, RGB glitch, colliding shapes, Y2K kinetic energy. Best for: apparel, digital campaigns, podcast visuals.
17. **Frutiger Aero** — early 2000s glossy optimism, aqua gradients, bubble type, floating orbs. Best for: tech, SaaS, digital products, retro-futurist brands.
18. **Type Collage** — type as material: torn, chrome, layered, colliding at incompatible scales. Best for: social content, streetwear, zine culture.

---

## Prompt Assembly — The 7-Section Structure

Load the chosen style profile from `styles.md`. Substitute every placeholder from the profile and the user's intake. **No placeholders may remain in the final output.** Use visual typography descriptions, not specific font names.

### 1. Goal
One sentence: what this image needs to do (announce, sell, evoke, brand, hire, launch). Anchors the rest of the prompt.

### 2. Reference Anatomy Lock — MANDATORY
Before describing style ingredients, describe the **structural DNA** of the reference style. Lock the format. This is the single most important section for fidelity, and it is required for every style — not just the typography-forward ones.

Every style profile in `styles.md` includes its own anatomy lock paragraph. Paste it verbatim. It describes:
- The exact composition format (full-bleed soft-focus field, asymmetric grid, centered stack, dense icon field, archival catalog grid, etc.)
- Where text lives and where it doesn't
- What the image is **not** (not an ad layout, not a UI mockup, not a style-guide board, not a swatch grid, not a slide layout, not a brand-deck page)
- The energy/posture of the piece (poster vs. presentation vs. catalog vs. broadcast)

Without this section, the model defaults to "advertising layout" and the chosen style becomes decoration on top of an ad. With it, the format discipline holds.

### 3. Style Definition
The aesthetic description from the style profile: medium, era, design tradition, surface treatment, mood. The "what it looks like" passage.

### 4. Subject Transformation
How the subject is rendered in this style. For Style 4 this is critical: even for products, do not show the product literally — translate the product into a typographic aura poster. The copy and atmosphere are the product expression. For illustrative styles, describe the level of abstraction. For photography styles, describe the lighting, grain, and posture.

### 5. Composition + Layout
Where every element lands. Map each piece of user-provided copy to its position and typographic treatment. Layout logic is style-locked — don't invent positions that contradict the anatomy lock.

### 6. Typography
Visual typography description, not font names. Weight, posture, scale, register, treatment (e.g. "massive condensed grotesque, all-caps, set tight"; "elegant high-contrast display serif with restrained drop"; "expressive script climax line overlapping a stacked all-caps block").

### 7. Color + Texture + Output Feeling
Color palette with hex values from the style profile. Texture treatment (grain, ink, print artifact, digital glitch, chrome, bokeh, etc.). One closing line on the output feeling — what this image should evoke at first glance.

**Always close the hero prompt with the style's negative-prompt block** from `styles.md`. These guard against the model's common drifts for that specific style.

**Always follow the hero prompt with the Reference Image Delivery block** (next section). The prompt without the reference image attached produces inconsistent results — pairing them is non-negotiable.

---

## Reference Image Delivery — MANDATORY

Every style profile in `styles.md` has a `**Reference image:**` line that names the matching file in `references/images/` and provides its public URL. Use it.

After the hero prompt block (and before Tier 2 / Tier 3, if requested), output this Delivery block verbatim, with the style's filename and URL substituted:

```
📎 **Attach this reference image when you generate:**

File: `references/images/[FILENAME].jpg`
Direct download: [PUBLIC_URL]

When you paste the prompt into ChatGPT Image 2.0 (or Midjourney, or any image tool that accepts image inputs), attach this reference image alongside the prompt. The reference anchors the visual style — the text describes the structure, the image teaches the model what the style actually looks like. Without the reference, the model defaults to generic interpretations and the anatomy lock can't fully compensate.

If your image generator doesn't accept image inputs, open the reference URL in another tab and use it as your visual touchstone while reviewing each generation.
```

For Tier 2 format variants and Tier 3 visual-system images, the same reference image stays attached — the variants are restatements of the same style, not new styles. State this explicitly: *"Keep the same reference image attached for all variants and supporting assets."*

**Show the reference image to the user when it's helpful.** When the user picks a style (Path A) or you recommend one (Path B), display the matching `references/images/style-NN-name.jpg` inline if your tool supports it, or tell them the file path so they can open it themselves. Seeing the reference at decision-time anchors expectations and lets the user veto early instead of after generation.

**The user must attach the reference image themselves in their image-generation tool.** This skill produces text; the image tool consumes both text and a reference image. The bridge between the two is the user — they copy the prompt and attach the matching .jpg file when they switch to ChatGPT Image 2.0, Midjourney, or wherever they generate. Make this explicit in the Delivery block every single time.

---

## Critical Rules — Anti-Drift

**Do not convert poster styles into product ads.** Especially for Styles 4, 8, 10, 18. The subject's name is enough; do not insert literal product mockups, devices, dashboards, UI cards, app screens, brand-deck slides, palette grids, or "wellness app" clichés unless the style explicitly calls for them.

**Respect copy density.** Re-check the user's copy length before assembling. If the chosen style is typography-forward (4, 8, 10, 18) or photography-forward (9), recommend condensing long copy. Image models can render some text, but too much pushes the result into landing-page or style-guide territory.

**Style-specific negative prompts are mandatory, not optional.** Every style profile in `styles.md` includes its own negative-prompt block. Paste it at the end of the hero prompt. Example for Style 4: no app mockup, no device, no dashboard, no rounded-square icon presentation, no brand guideline page, no palette swatch grid, no logo lockup sheet, no glassmorphism panel, no person meditating, no lotus, no heart-rate line.

**Never invent copy.** If the user did not provide a tagline, do not write one. Ask, or omit.

**Never generate prompts before intake is complete.** Subject + copy + style, in that order. No shortcuts.

**Never deliver a hero prompt without the Reference Image Delivery block.** The prompt and the reference image are a pair. Delivering the prompt alone is the single largest cause of poor image-tool output. If the user pastes only the text into ChatGPT Image 2.0 and skips the attachment, the model has no visual anchor and the style will not hold.

---

## Tier 2 — Format Variants

Generate three adapted prompts after the hero. For each, output only what changes from the hero — do not repeat the full style description.

**Square 1:1 — Social Post.** Compress vertical hierarchy. Move copy to upper or lower third. Keep subject centered. Note elements to drop or condense.

**Horizontal 16:9 — Banner / Cover.** Subject shifts left or right. Copy occupies the opposite half. Works as LinkedIn banner, event cover, email header, YouTube thumbnail.

**Vertical 9:16 — Story / Reel Cover.** Exaggerate vertical hierarchy. Title at top, subject center, supporting copy at bottom. Flag safe zones: top 15% and bottom 20% stay clear of critical content for UI overlay.

---

## Tier 3 — Visual System

Frame as: *"The building blocks of your campaign — what turns one image into a coherent visual identity."*

Two important distinctions:
- **Visual system direction** (written): palette, avatar, supporting assets, mood note as creative direction text.
- **Generated visual system images** (prompts): must obey the chosen style's visual grammar and anatomy lock. A color-palette image for Style 4 is not a standard swatch board — it is a blur poster with tiny palette annotations. A supporting-asset prompt for Style 5 is more dense icon-field illustration, not a clean icon grid. The style's anatomy lock applies to every system image, not just the hero.

### 1. Color Palette
Extract 5 colors from the style profile. Present as: `[Name] · [Hex] · [One-line usage note]`.

Roles:
- **Dominant** — background or primary field
- **Primary** — main illustration or subject color
- **Accent** — the pop color, used sparingly
- **Type** — text color
- **Neutral** — supporting mid-tone, shadow, or surface color

### 2. Supporting Asset Prompt
A prompt for 6–8 supporting graphic elements in the same style — icons, textures, decorative marks, or pattern tiles — usable as section dividers, background tiles, badges, or secondary post imagery.

Elements must be thematically tied to the subject, not generic:
- Food / restaurant → utensils, ingredients, steam wisps, stamps, bowls
- Concert / event → instruments, sound waves, venue silhouette, ticket stubs
- Fashion launch → stitching details, fabric texture, silhouette outlines, label marks
- Sports / culture → team symbols, city landmarks, movement lines, score elements
- Nature / wellness → botanical forms, terrain lines, weather symbols, cross-sections

### 3. Avatar / Profile Visual
A prompt for a tight square crop optimized for profile photos, story icons, or brand avatars. Two options:
- **Subject-centered:** the subject simplified to its most iconic form at close range, same style and palette.
- **Monogram treatment:** the primary title's initials rendered in the same visual style as the hero — same texture, same color system, same typographic register.

### 4. Campaign Mood Note
Two to three sentences: what visual world this style creates for this specific subject, what it signals to the audience, and one concrete extension suggestion (physical, digital, or motion — whichever is most natural for the use case).

---

## Reference Files

- `styles.md` — All 18 style profiles. Each profile includes a Reference image line (filename + public URL), anatomy lock, aesthetic description, subject transformation, composition, layout logic, typography, color palette with hex values, texture treatment, output feeling, and style-specific negative prompts. **Read before assembling any prompt.**
- `references/images/` — 18 reference image files, one per style, named `style-NN-name.jpg`. These are the visual anchors users attach to their image generator. The filenames in this folder match the `**Reference image:**` line in each profile.
- `STYLES.html` — a single-page visual browser of all 18 styles. Openable in any browser; useful for users who prefer to browse cards rather than read a menu.

Optional public mirror (if the project is published to GitHub Pages):
- Gallery: `https://sijingsun.github.io/the-art-director/STYLES.html`
- Individual images: `https://sijingsun.github.io/the-art-director/references/images/style-NN-name.jpg`

These URLs are a convenience for users who want to share links instead of files. The skill works fully offline from the unzipped folder — the URLs are not required.
