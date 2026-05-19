# Style Library — 10 Visual Style Profiles

Each profile defines the full parameter set for the master prompt template in SKILL.md. Read the chosen profile in full before assembling any prompt.

**Critical instruction on typography:** Font names do not reliably transfer to AI image models. Always describe typography using visual geometry — stroke weight, letterform proportions, spacing behavior, and spatial relationship to the frame. The descriptions below are written for this purpose. Use them verbatim in prompts.

---

## Style Index

| # | Style Name | Mood in one word | Best for |
|---|-----------|-----------------|----------|
| 1 | Japanese Retro Print | Proud | Food, restaurants, cultural events |
| 2 | Mid-Century Editorial | Refined | Products, objects, limited editions |
| 3 | Neo-Expressionist Event | Raw | Concerts, festivals, nightlife |
| 4 | Chromatic Blur / Aura | Atmospheric | Brand mood, quotes, campaigns |
| 5 | Retro Cartoon Maximalist | Energetic | Sports, street culture, merch |
| 6 | 70s Psychedelic Folk | Warm | Outdoor events, music, nature brands |
| 7 | Chalk & Crayon Naïf | Playful | Art events, parties, indie brands |
| 8 | Typographic Sculpture | Declarative | Manifestos, brand culture, talks |
| 9 | Dark Fashion Editorial | Cinematic | Fashion, beauty, luxury launches |
| 10 | Contemporary Swiss / Museum | Intellectual | Cultural events, exhibitions, galleries |

---

## Style 1 — Japanese Retro Print

**Mood:** Proud, graphic, culturally specific. Feels handcrafted but bold.
**Best for:** Food, restaurants, cultural events, product origin stories.
**Reference:** Okiboru House of Udon poster.

### Parameters

**Aesthetic description:**
Vintage Japanese graphic poster aesthetic with a strictly limited 2–3 color palette (deep blue, warm red, off-white background). Mid-century Japanese print design — bold shapes, clean linework, slight print texture. Feels like a screen-printed food stall poster from 1960s Japan. No photography, no gradients, no realism.

**Subject treatment:**
- Convert the subject into a simplified vector-style illustration
- Reduce details to bold shapes and clean outlines only
- Apply duotone: primarily deep blue with selective red accents
- Add subtle halftone dots or grain texture to mimic screen printing
- Flat graphic shadows — no realistic lighting or drop shadows
- Stylized, not photorealistic

**Composition rules:**
- Subject centered and prominent, roughly 60% of the poster height
- Simple geometric shadow beneath (solid blue oval)
- Generous negative space around the subject
- Thin rectangular border frame in red, inset from all edges by a consistent margin

**Layout logic — where copy lands:**
- Top: Primary title — largest element on the page, warm red, all caps
- Below title: Subtitle as a narrow horizontal band flanked by short decorative rule lines on both sides (blue)
- Left side: Vertical Japanese-style characters stacked top to bottom (blue, medium weight)
- Bottom left: Secondary descriptor in small Japanese characters with romanized transliteration beneath (blue, small)
- Bottom right: Origin or establishment label e.g. "JAPAN / EST. 20XX" (red, bold)
- Optional: Small red-bordered stamp/seal in lower left with 1–2 kanji

**Typography — visual geometry specification:**
- Primary title: Letterforms with uniform stroke weight throughout — no thick-thin contrast. Characters are wide relative to their height, almost square. Stroke terminals are cut flat, not rounded. Letter-spacing is generous — roughly one stroke-width of air between each character. Height of the title block is approximately 15–18% of the total poster height. All caps. Warm red.
- Subtitle: Same uniform-stroke geometric letterforms at roughly one-third the title height. Medium tracking. Blue. Flanked by horizontal rule lines of the same stroke weight as the type.
- Vertical side text: Japanese characters stacked vertically, each occupying a square cell. Drawn with brush-like stroke variation — thicker horizontals, thinner verticals. Decorative, atmospheric.
- Bottom labels: Same geometric sans as subtitle at very small scale. Romanized text beneath Japanese characters, same width as the Japanese text above it.
- Critical: No stroke weight variation in any Latin text. No serifs. No rounded terminals. Every letterform reads as a geometric construction, not a calligraphic one.

**Color palette:**
- Dominant (background): Warm off-white / aged paper `#F5F0E8`
- Primary (illustration): Deep blue `#1A3A8F`
- Accent (title, border, stamps): Warm red `#CC2222`
- No gradients — flat solid blocks only

**Texture & finish:**
- Subtle ink bleed at all color edges — colors slightly overflow their boundaries as if absorbed into paper
- Slight misregistration (1–2px color offset) between blue and red elements, as if two passes through a press were slightly misaligned
- Paper grain texture overlay across full image — visible at normal viewing distance
- Halftone dot pattern in all shadowed or dark fill areas
- Slightly imperfect edges on large color fills — not perfectly crisp digital edges

**Output notes:**
Bold graphic simplification, strong color blocking, intentional typography. Should feel like it was pulled off a press in 1965 Osaka. The misregistration and halftone are not optional — they are what separates this from a generic flat design.

---

## Style 2 — Mid-Century Editorial

**Mood:** Refined, quietly luxurious, slightly nostalgic.
**Best for:** Products, objects, lamps, furniture, limited-edition goods, design launches.
**Reference:** Modern Light lamp editorial poster.

### Parameters

**Aesthetic description:**
Mid-century modern print aesthetic. Muted duotone palette — dusty blue or faded teal background, warm off-white typography. Subtle film grain, paper texture, and slight fading mimic aged print. Editorial and gallery-like — never commercial or loud. Feels like a page from a 1972 design magazine.

**Subject treatment:**
- Isolate the subject completely — remove all background clutter
- Preserve any warm glow, light emission, or material highlight as the focal contrast element
- Slightly desaturate the subject body while keeping warm highlights intact
- Add gentle film grain texture to the subject surface
- Place subject bottom-center, slightly overlapping into the text zone above
- Soft diffused shadow beneath to ground it — no hard drop shadows

**Composition rules:**
- Clean editorial layout, gallery-like negative space — the poster should feel mostly empty in a deliberate way
- Vertical near-symmetry, slightly offset for a human feel
- Rounded corner frame or subtle vignette at edges
- Maximum 6–7 text elements total — anything more is clutter
- Soft vignette fading toward all four corners

**Layout logic — where copy lands:**
- Top center: Very small all-caps collection label, high up, light weight — reads almost as a whisper
- Center-upper: Large display title — the biggest typographic moment, slightly overlapping with the subject below
- Left, mid-poster: A large numeral or time in display type; a 2–3 word descriptor in small type below a short horizontal rule line
- Right, mid-poster: Date or edition label in display type; a 1–2 word qualifier in small type below a short rule line
- Bottom center: Optional tagline in very small spaced caps — quiet, almost invisible
- Very bottom center: Optional small decorative symbol — 4-pointed star, cross, or dot

**Typography — visual geometry specification:**
- Primary title: High-contrast letterforms where stroke width varies dramatically — hairline thin strokes and very thick strokes within the same character. The thick strokes are approximately 8–10x the width of the thin strokes. Alternatively, flowing script letterforms with natural pen-pressure variation, where upstrokes are thin and downstrokes are thick. Either way: this type has personality and rhythm, not uniformity. The title spans approximately 70–80% of the poster width. Off-white / antique ivory color.
- Large numerals: Same high-contrast construction as the title but used for dates or times — the number forms are architectural and structural, occupying significant space.
- Small descriptor text: Extremely thin letterforms — stroke weight so light it appears almost as a line. Very generous letter-spacing, roughly 2–3 stroke-widths between characters. Small scale — roughly 4–5% of poster height.
- Tagline: Same thin letterforms at even smaller scale, tracked very wide, feels like it's barely there.
- Critical: The contrast between the heavy display title and the near-invisible small type is the entire typographic argument. Do not use a medium-weight font anywhere — everything is either very heavy or very light.

**Color palette:**
- Dominant (background): Dusty blue / faded teal / steely grey-blue `#4A6580`
- Type: Warm off-white / antique ivory `#F0EBE0`
- Subject: Natural tones, slightly desaturated, preserving inherent warmth
- No strong accent color — the subject's warmth is the only contrast

**Texture & finish:**
- Film grain across the full image — moderate, visible but not distracting
- Paper texture overlay, slightly aged
- Subtle ink bleed at text edges
- Slight text misalignment for authentic print feel
- No sharp digital edges — everything slightly softened

**Output notes:**
Preserve any subject glow as a warm focal highlight against the cool background. The visual tension between warm subject and cool field is the entire design argument.

---

## Style 3 — Neo-Expressionist Event

**Mood:** Raw, energetic, culturally alive. Feels like it was wheat-pasted on a wall in Berlin.
**Best for:** Concerts, club nights, boutique festivals, cultural events, artist showcases.
**Reference:** Cape Kablys "Prologue" festival poster.

### Parameters

**Aesthetic description:**
Contemporary European event poster aesthetic. Bold horizontal color blocking creates distinct zones (header band, illustration field, footer strip). Painterly, gestural illustration style — loose brushwork, expressive figures, almost Basquiat-influenced but constrained by a structured grid. Saturated, clashing primaries. Thick black outlines. Feels both raw and designed — intentional chaos within a system.

**Subject treatment:**
- Convert subject or figures into gestural, painterly illustration — loose brushwork, not precise vector
- Apply thick black outline strokes to all major forms — outlines should be slightly uneven in weight
- Fill with flat, saturated color fields — no blending, no gradients within shapes
- Allow forms to overlap and bleed into each other expressively
- Background of the illustration zone is a single saturated field color (e.g. dark forest green)
- Keep energy and movement — avoid static, centered poses

**Composition rules:**
- Divide the poster into three horizontal bands: title header (top ~25%), illustration field (middle ~50%), footer strip (bottom ~25%)
- Illustration bleeds to edges within its band — no padding
- Title header: solid bold color (red, orange, or primary) with title text only
- Footer: white or off-white strip containing performer/detail copy
- Strong typographic scale contrast between header title and footer details

**Layout logic — where copy lands:**
- Top band (header): Event series name small + primary event title massive (both left-aligned or centered, all caps)
- Top right corner: Date + venue logo or identifier (small, stacked)
- Middle band: Full illustration — no text intrudes except optional small location text
- Bottom band left: Headliner name(s) in bold, large
- Bottom band right: Supporting act names in condensed columns
- Very bottom: Sponsor logos + tagline in small type

**Typography — visual geometry specification:**
- Primary title (in header band): Letterforms that are extremely wide relative to their height — characters that are nearly as wide as they are tall, or even wider. Stroke weight is heavy and uniform throughout with no thick-thin variation. The negative space inside each letterform (counters) is small relative to the stroke mass. Characters sit with almost no gap between them — nearly touching or actually touching at their sides. The title fills the full width of the header band from edge to edge. All caps. The letterforms feel like they have weight and mass, like concrete blocks.
- Event series label: Same construction at roughly one-quarter the scale of the title. Light tracking.
- Performer names (footer): Same wide heavy letterforms at medium scale. Mixed sizes within the footer to indicate billing hierarchy — headliner roughly 2x the height of support acts.
- Footer details: Same sans at very small scale, regular weight.
- Critical: The header title should look like it could not fit one more letter — it consumes the entire band. No condensed fonts, no narrow letterforms. Width is the typographic personality here.

**Color palette:**
- Header band: Saturated warm color — red `#D63B1F`, orange `#E8551A`, or similar
- Illustration field: Dark saturated ground — forest green `#1A4A2E`, deep teal, or navy
- Illustration fill colors: Clashing primaries — cobalt blue, dusty pink, golden yellow, warm orange
- Footer band: White `#FFFFFF` or off-white `#F5F2EE`
- Outline: Near-black `#0A0A0A`
- No gradients — all flat, high-contrast fields

**Texture & finish:**
- Slight halftone or risograph texture across illustration — color fields are not perfectly smooth
- Subtle paper grain — light, not dominant
- Illustration brushwork should feel slightly hand-made, not vector-clean
- Text is crisp and digital — the contrast between raw illustration and clean type is intentional

**Output notes:**
The energy comes from the tension between structured layout and expressive illustration. Do not over-clean the illustration — the looseness is the point.

---

## Style 4 — Chromatic Blur / Aura

**Mood:** Atmospheric, emotional, immersive. Feels like a feeling more than a thing.
**Best for:** Brand mood pieces, campaign manifestos, quote visuals, music releases, emotional launches.
**Reference:** "Limits You" typographic aura poster.

### Parameters

**Aesthetic description:**
Contemporary digital-meets-analog aesthetic. The background is a full-bleed abstract color wash — extreme out-of-focus photography or painterly color field, completely unrecognizable as a specific image. No subject illustration. No borders. The typography floats as the only structured element, making it the entire visual argument. Feels like 2023–2025 digital art direction — emotional, abstract, typography-forward.

**Subject treatment:**
- If a reference image is uploaded: radically blur and abstract it until no recognizable forms remain — only color, light, and atmosphere survive
- If no image: generate an abstract painterly color wash using warm-to-cool gradient fields, soft blooms of color, diffused light leaks
- The background should feel like looking at light through frosted glass or a macro shot of pigment in water
- Apply subtle grain or film texture across the full background
- No sharp edges, no recognizable shapes anywhere in the background

**Composition rules:**
- Full-bleed background — no borders, no frames, no contained zones
- Typography floats freely across the color field — not anchored to a hard grid
- Intentional vertical breathing room between text blocks
- One line of copy breaks into a different typographic register (the emotional climax)
- Subtle vignette toward edges to focus attention on center

**Layout logic — where copy lands:**
- Upper third: First lines of copy — bold, all caps, centered or left-weighted, off-white
- Middle (with breathing room above and below): Second copy block — same treatment, more vertical space above it
- Lower-center: The climax line — switches to flowing script or italic letterforms, larger scale, this is the emotional peak
- Very bottom center: Optional small icon, logomark, or symbol — tiny, quiet

**Typography — visual geometry specification:**
- Primary copy lines (upper and middle): Letterforms with uniform stroke weight — no thick-thin variation. Characters are moderately wide, upright, and geometric. The stroke is heavy enough to read clearly against the blurred background without being so heavy it feels aggressive. All caps. Letter-spacing is slightly open — more air than default. Off-white or soft cream color. Semi-transparent or with very soft edges so the type feels embedded in the atmosphere rather than pasted on top.
- Climax line: Flowing, connected letterforms with dramatic stroke variation — thin hairlines where the pen lifts, thick swells where it presses. Characters connect to each other with fluid linking strokes. The overall form moves diagonally or has natural forward lean. Approximately 1.5–2x the height of the lines above it. Same off-white color. This line should feel like a sigh or an exhale after the controlled lines above.
- Critical: The shift in register between the controlled geometric lines and the flowing script climax IS the design. The contrast must be dramatic. Do not use a script font for the upper lines or a geometric font for the climax.

**Color palette:**
- Background: No fixed palette — derived from the source image or emotional brief. Typical combinations: warm terracotta + dusty blue, sage green + golden amber, deep violet + rose, cool steel + warm coral
- Typography: Off-white `#F5F2EE` or soft cream — never pure white
- No hard accent colors — the background IS the color palette

**Texture & finish:**
- Heavy grain across the full image — more grain than any other style
- Background blur should feel photographic, not digitally smooth
- Text edges slightly soft — not razor sharp
- No borders, no frames, no geometric elements of any kind

**Output notes:**
The restraint of having only typography on an abstract field is the design statement. Do not add illustration, icons, or structural elements. If it feels too empty, the answer is better copy placement — not more visual elements.

---

## Style 5 — Retro Cartoon Maximalist

**Mood:** Energetic, celebratory, city-proud. Feels like a limited-edition merch drop.
**Best for:** Sports events, street culture, city celebrations, Latin-inspired events, cultural nights, merch posters.
**Reference:** Brooklyn Nets "La Manera de Brooklyn" Noche Latina poster.

### Parameters

**Aesthetic description:**
Dense, joyful illustration maximalism. Black background. Every inch of space filled with flat illustrated icons, characters, and environmental elements. Bold primary colors with thick white outlines on every element. Chunky bubbly display type. Feels like 1970s–80s Latin American graphic design filtered through contemporary streetwear illustration. Nothing is subtle — everything is at maximum.

**Subject treatment:**
- Translate the subject into the illustrated icon language of the style — do not use the photo directly
- Create a cast of 8–12 illustrated icons/characters thematically tied to the subject: locations, objects, mascots, symbols, cultural references
- All icons: flat color fills, thick white outline strokes, bold and chunky shapes — no gradients, no shadows
- Include at least one character or mascot with personality — not just objects
- Icons scattered across the field, overlapping, at varied scales — dense but legible
- Black background bleeds to all edges — no framing or border

**Composition rules:**
- Black background field, full bleed
- Primary title at top center in massive display type
- Secondary large text at bottom center — nearly as large as the title
- Illustrated icons fill the middle field completely, around and behind any mid-poster text
- No empty space — if there's a gap, fill it with an icon
- Small logo/sponsor lockup in bottom corners

**Layout logic — where copy lands:**
- Top center: Large bubbly display title (white or primary color, with colored outline or shadow)
- Top: Subtitle or modifier in smaller display type, same family, contrasting color
- Mid-poster (floating among icons): Location name or short exclamation in bold display
- Mid-poster: Key date or number in very large bold numerals, partially behind icons
- Bottom center: Main secondary text in massive display, nearly full width
- Bottom strip: Date, event details, sponsor logos in small condensed type

**Typography — visual geometry specification:**
- Primary and secondary titles: Letterforms where the interior space of each character (the counter) is inflated — rounded, balloon-like, pushing outward. Stroke weight is heavy and consistent. Corners are rounded, not angular. The overall impression is that each letter has been inflated with air and is straining at its outline. Characters have thick white outlines that create separation from the colored background. Mixed use of white fills and solid primary color fills across different words — not uniform.
- In-poster exclamations: Same inflated rounded forms used freely for single emphasis words — different color per word if needed.
- Date/detail strip: Narrow, condensed letterforms at small scale — a deliberate contrast to the bubbly display above. Tight tracking, light to regular weight.
- Critical: The bubbly roundness of the display type must be pronounced. Generic bold fonts do not achieve this — the letterforms need visible inflation and rounded corners. Outline strokes on all display type are non-negotiable.

**Color palette:**
- Dominant (background): Pure black `#0A0A0A`
- Primary illustration colors: Flat primaries — cobalt blue, signal red, golden yellow, kelly green
- Icon outlines: White `#FFFFFF`
- Typography: White with colored outlines or shadows
- No muted colors, no pastels, no gradients within elements

**Texture & finish:**
- Minimal texture — this style is crisp and graphic
- Slight halftone or noise texture on large color fields only
- White outlines consistent weight throughout
- High contrast — black and white relationships are bold

**Output notes:**
Density and specificity are what make this style work. Generic icons feel like clip art. Every element should be legible as this subject, this place, this event.

---

## Style 6 — 70s Psychedelic Folk

**Mood:** Warm, communal, handcrafted. Feels like a poster you'd frame in a mountain cabin.
**Best for:** Outdoor music festivals, amphitheater seasons, nature brands, wellness retreats, folk or jam band events.
**Reference:** Gerald R. Ford Amphitheater 2025 Concert Season poster.

### Parameters

**Aesthetic description:**
Warm illustrated landscape poster tradition — equal parts Grateful Dead concert poster, vintage national park print, and 1970s folk album cover. Symmetrical or near-symmetrical central scene built entirely from hand-drawn illustration. Warm amber, teal, and orange palette. Organic rounded shapes throughout — no hard geometry. Decorative botanical, celestial, and natural motifs fill every corner. Friendly rounded serif display type with outline strokes.

**Subject treatment:**
- Translate the subject into a central illustrated scene — a landscape, a gathering, a moment
- Build an environmental world around it: trees, mountains, sun rays, animals, celestial elements, botanical details specific to the location or theme
- Symmetrical composition: central focal element flanked by mirrored or near-mirrored environmental framing elements
- Warm color fills throughout — no photorealism, no photography
- All illustration: flat color with bold outlines, organic rounded forms

**Composition rules:**
- Near-symmetrical: left and right sides mirror or echo each other
- Central focal illustration occupies the middle 60% of the poster
- Decorative border or natural frame built from the illustration elements (trees, mountains forming natural edges)
- Title contained within a shaped banner or pill form at the top — not floating freely
- Footer strip for detailed copy in small type on a contrasting ground

**Layout logic — where copy lands:**
- Very top: Small presenter or series label — tiny, all caps, centered
- Top, inside a banner shape: Primary title centered, 2–3 lines if needed
- Below banner: Subtitle or event descriptor in secondary display
- Mid-poster: Location name on a ribbon or arch element integrated into the illustration
- Bottom strip (contrasting ground): All supporting copy — lineup, dates, times — in small condensed type, multi-column
- Corners: Decorative botanical or celestial marks

**Typography — visual geometry specification:**
- Primary title: Slab serif letterforms — serifs that are thick rectangular slabs, approximately the same weight as the main stroke. The overall letterform weight is heavy but not extreme. Characters have a slight condensed quality — taller than wide, but not dramatically condensed. Visible outline stroke around each letterform in a contrasting color (typically darker or lighter than the fill). The outline gives the letters a slightly embossed, printed quality. Warm color fill, dark outline.
- Subtitle / descriptor: Complementary style — either italic version of the same slab serif, or a flowing script with connecting strokes between letters. Smaller scale than the title.
- Location / integrated text: Follows the shape it sits on — curved along an arch, following a ribbon. Same slab serif family.
- Details strip: Very small condensed type — narrow letterforms, tight tracking, high information density. Contrasts with the organic roundness of the display type.
- Critical: The slab serifs with outline strokes are the typographic signature. Thin modern serifs or sans-serifs destroy the period authenticity. The outline is essential — letterforms without outlines look unfinished in this style.

**Color palette:**
- Dominant (background): Warm golden amber or soft sage green
- Secondary field: Muted teal and warm orange
- Illustration fills: Warm cream, sky blue, forest green
- Text: Dark brown-black or warm cream depending on background zone
- Outline: Dark brown-black throughout
- No cold colors — everything tilts warm

**Texture & finish:**
- Hand-drawn illustration texture throughout — visible line variation, not vector-smooth
- Slight paper grain or linen texture overlay
- Color fills slightly uneven — looks screen-printed or hand-painted
- No film grain — this is illustration texture, not photography texture

**Output notes:**
The illustrated world-building is what makes this style. A generic landscape fails — it needs specific, character-filled details that belong to this event, this place.

---

## Style 7 — Chalk & Crayon Naïf

**Mood:** Playful, energetic, deliberately imperfect. Feels made by a very cool person who chose not to make it perfect.
**Best for:** Art events, gallery openings, parties, indie brands, creative studios, underground events.
**Reference:** Art Party event poster.

### Parameters

**Aesthetic description:**
Deliberately rough, childlike aesthetic — but with taste. Chunky hand-drawn display type. Single gestural line-art illustration in crayon or pastel texture. Extreme color limitation: two colors maximum on a near-white ground. Mixed typographic registers: bold chunky display for the title, casual handwritten script for secondary copy. The roughness is the design statement.

**Subject treatment:**
- Translate the subject into a single gestural line-art figure or form drawn in crayon or chunky pastel
- One continuous or near-continuous line — expressive, slightly wobbly, human
- No fill colors within the illustration — just the line itself in the accent color
- The line has visible texture: crayon wax, chalk dust, pastel grain
- Large scale — the figure occupies most of the poster height
- No background elements, no environmental context

**Composition rules:**
- Near-white or very light warm background — no border
- Title text at top, large, above or overlapping the figure
- Figure centered or slightly off-center, running from mid-poster downward
- Secondary copy floats freely around the figure — not grid-locked
- Nothing is perfectly aligned — intentional slight tilts and offsets throughout

**Layout logic — where copy lands:**
- Top: Primary title in massive chunky display, slightly uneven baseline, left or centered
- Top right or inline with title: Date in parentheses, slightly different weight
- Mid-left or mid-right (floating beside the figure): Time in large display
- Mid-right or lower-right (floating): Key detail (e.g. "free entry") in large handwritten script
- Bottom left: Address or location in very small straight type
- Bottom right: Social handle or URL in very small straight type

**Typography — visual geometry specification:**
- Primary title: Letterforms that appear hand-constructed — slightly uneven stroke widths, corners that are not perfectly square, baseline that drifts slightly across the word. The overall impression is of letters drawn quickly with a thick marker or brush. Stroke weight is heavy — approximately one-quarter to one-third of the total character height. Characters are compact, not widely spaced. The uneven quality is critical — digitally perfect letterforms destroy this aesthetic. Primary color fill (the warmer of the two palette colors).
- Date/inline modifier: Same chunky letterforms wrapped in parentheses, rendered in a slightly lighter weight or the same weight at smaller scale. Feels casual and informal, like a handwritten annotation.
- Handwritten secondary copy: Completely different register — flowing, connected, personal. Strokes that vary in width as if from natural pen pressure. Characters that connect to each other with linking strokes. Slight forward lean. The contrast between this and the chunky display title is the typographic personality of the poster.
- Small detail text (address, handle): Upright, simple, utilitarian — almost bureaucratic in its straightness relative to everything else. This creates a visual joke: the serious information is rendered in the most neutral way possible.
- Critical: The handmade quality of the display type is non-negotiable. Clean digital lettering in this style reads as Canva output. The slight irregularity of each character is what signals craft and intention.

**Color palette:**
- Dominant (background): Near-white warm paper or very pale blush
- Primary color (title + small type): Warm pink / salmon or similar warm mid-tone
- Accent color (illustration line): Deeper warm orange or burnt sienna — slightly darker than the title color
- Two colors total — strictly limited

**Texture & finish:**
- Crayon or chalk texture on the illustration line — visible wax or grain
- Slight paper grain across the background
- Edges of display type slightly rough — not perfectly digital
- No drop shadows, no gradients

**Output notes:**
The balance between rough and considered is the hardest thing to get right. Everything should look casual but nothing should look accidental. The figure needs energy and movement — a static pose kills it.

---

## Style 8 — Typographic Sculpture

**Mood:** Declarative, confident, ideological. Feels like a manifesto printed on a wall.
**Best for:** Company culture, brand values, keynote backdrops, design manifestos, conference talks, editorial campaigns.
**Reference:** GitHub "demos not memos" poster.

### Parameters

**Aesthetic description:**
The typography IS the image. No illustration, no photography, no supporting visual elements. Massive-weight grotesque type at extreme scale, lowercase, filling the poster as pure sculptural form. Type breaks columns, extends close to edges, treats letterforms as architectural mass. Small body copy floats at grid intersections as the only relief. Design argument made entirely through weight, scale contrast, and spatial tension.

**Subject treatment:**
No subject image. This style requires only text. If the user uploads an image, acknowledge it but explain it will not appear in the output — only the text they provide.

**Composition rules:**
- Dark background (near-black or very dark charcoal) — type reads as white on dark
- Primary display text fills approximately 70–80% of the poster width, stacked in 4–6 lines
- Each word or syllable break gets its own line — the line breaks are the editorial decision
- Small body copy: 2–3 instances maximum, at natural negative space intersections
- No borders, no rules, no decorative marks
- Strict invisible grid — everything aligned to baseline and column

**Layout logic — where copy lands:**
- Full poster, top to bottom: Primary message broken across 4–6 lines in massive display, left-aligned, filling the width
- Upper area, left of type: First small body quote or supporting statement (2–4 lines, small, left-aligned)
- Mid-poster, right of type: Second small body statement (2–4 lines, small, right-aligned)
- Lower area, left: Third small body statement or attribution (optional)
- No footer, no header bands — the type IS the structure

**Typography — visual geometry specification:**
- Primary display: Letterforms with extremely heavy stroke weight — the strokes are approximately 25–35% of the total character height. The interior space of each character (counter) is dramatically reduced by this stroke weight — letters like 'o', 'e', 'a' have very small holes. Characters are moderately wide, not condensed. The overall mass of each letter dominates its surrounding negative space. Lowercase only — the absence of capitals is deliberate and softens the authority slightly. Letters should feel like they have physical weight, as if cast in lead. White or very light warm white fill against dark background.
- Display size: Each character is approximately 15–25% of the poster width. A 4-letter word fills the poster from edge to near-edge.
- Small body copy: Same typeface family but at regular or light weight — the contrast in weight between display and body is the most extreme of any style in this library. Small body text is roughly 2–3% of the poster height. The weight shift from the massive display to the almost-invisible body text is the entire design.
- Critical: The line breaks in the display copy are editorial decisions. "demos / not / me / mos" creates different rhythm than "demos / not memos". These breaks must be specified deliberately based on the user's copy — do not let the AI model choose them randomly.

**Color palette:**
- Dominant (background): Very dark charcoal `#1A1A1E` or near-black `#111114`
- Primary display type: White `#FFFFFF` or very light warm white `#F5F5F0`
- Small body type: Same light white — only size distinguishes hierarchy
- Optional: Single accent word in muted color (dark red, muted gold) for emphasis — use at most once

**Texture & finish:**
- Very clean — minimal texture
- Optional very subtle noise grain at low opacity — just enough to feel printed
- Type edges: Sharp and crisp — this is the one style where precision is correct
- No paper grain, no ink bleed, no misregistration

**Output notes:**
Specify the exact line breaks for the display copy in the prompt. This is not optional — it determines the rhythm and success of the composition.

---

## Style 9 — Dark Fashion Editorial

**Mood:** Cinematic, mysterious, high-stakes. Feels like a scene from a film you want to be in.
**Best for:** Fashion launches, beauty campaigns, luxury product releases, portrait-forward campaigns, music artist profiles.
**Reference:** "The Sculpt Blazer" Larana Inc. fashion editorial poster.

### Parameters

**Aesthetic description:**
Full-bleed moody photography — deep, saturated background tones (crimson, noir black, forest, ink), heavy film grain, slight lens blur or glow at subject edges. Dramatic directional light — partial obscuring of the face or form is intentional mystery. Typography as a structured grid overlay: bold condensed block on one side, smaller metadata on the other. Feels like an A24 film poster crossed with a luxury fashion campaign.

**Subject treatment:**
- Use the subject photo with full bleed — no cropping to a contained zone
- Apply heavy film grain and a strong color grade (deep warm red, noir black, or jewel tone)
- Introduce subtle lens effects: slight bloom at light sources, gentle blur at extreme edges, slight vignette
- Allow partial obscuring (shadow crossing features, soft lens blur on one side) — creates mystery
- Do not over-retouch — texture and imperfections are authentic
- The subject should look like a film still, not a product shot

**Composition rules:**
- Full-bleed photography — color grade extends to all edges
- Typography occupies the lower 40% as a structured overlay, not a separate zone
- Left side: Primary title in large bold condensed block, 2–3 lines, left-aligned
- Right side: 2–3 metadata blocks in smaller type, right-aligned
- Small horizontal rule lines or circle marks separate metadata items
- Top: Brand name and product category — very small, flush left and right at very top edge
- Rounded corner frame on entire poster — subtle radius

**Layout logic — where copy lands:**
- Top left: Brand name — very small, light weight, all caps
- Top center: Optional small circle mark
- Top right: Product category or series — very small, light weight, all caps
- Lower left: Primary product/subject name in large bold condensed block, 2–3 lines stacked
- Lower right, stacked blocks: Product descriptor sentence, launch info with parenthetical date, attribute labels with values
- Bottom footer strip: Social handle, URL, CTA — small, evenly spaced with circle separators

**Typography — visual geometry specification:**
- Primary title (lower left): Letterforms that are significantly taller than they are wide — condensed proportion where character height is approximately 3–4x the character width. Stroke weight is heavy and uniform — no thick-thin variation. Characters sit very close together, almost touching. The overall block of text feels like a vertical architectural element anchoring the lower left corner. White fill against dark photo. 2–3 lines stacked.
- Metadata labels (lower right): Same condensed construction at very small scale — roughly 8–10% of the primary title height. All caps, tracked open. Light weight rather than heavy — the contrast with the bold title is weight-based, not size-based alone.
- Metadata values: Same small scale as labels but heavy weight — the label is light, the value is bold. Creates alternating rhythm within the metadata column.
- Descriptor sentence: Very small scale, regular or light weight — the only text that reads at a comfortable reading size. Adds warmth and approachability to the otherwise architectural layout.
- Top labels: Same family as everything else, extremely small, very light weight, tracked wide. These are barely there — functional, not decorative.
- Critical: The condensed proportion of the title block is the typographic signature. Normal-width letterforms do not create the architectural weight this style requires. The title must feel like a structural column, not a label.

**Color palette:**
- Background: Deep photographic tone — deep crimson `#4A0A0A`, noir black `#0A0A0F`, forest ink `#0A1A14`, midnight blue `#0A0A2A`
- Typography: White `#FFFFFF` throughout
- Grain and grade: Warm shift for fashion/luxury, cool shift for beauty/editorial
- No bright accent colors — the subject's own highlights are the only warm notes

**Texture & finish:**
- Heavy film grain — second most grain-forward style after Chromatic Blur
- Subtle color grade applied to full image for cohesion
- Slight vignette at all four corners
- Lens bloom at practical light sources
- Rounded corner frame — subtle radius, feels like a printed card

**Output notes:**
Ask for dramatic directional lighting and deep background tones. Flat, evenly lit photography does not work in this style.

---

## Style 10 — Contemporary Swiss / Museum

**Mood:** Intellectual, considered, quietly confident. Feels like an invitation from a place that doesn't need to impress you.
**Best for:** Art exhibitions, cultural festivals, gallery openings, design conferences, museum events.
**Reference:** Studio Air spring collection exhibition poster / Art Festival poster.

### Parameters

**Aesthetic description:**
Contemporary interpretation of Swiss International Style. Warm off-white background. Massive lowercase neo-grotesque type at the top, bleeding toward edges. One photograph inset as a contained rectangular block — treated as document, not hero image. Small justified body copy. Tiny plus marks or 4-pointed stars as the only ornamentation. Intellectual, museum-adjacent. Feels like something MoMA would mail you.

**Subject treatment:**
- Convert the subject photo into a contained rectangular inset — cropped to horizontal or square format
- Apply subtle desaturation — reduced color intensity, not full black-and-white
- Photo placed in the middle-lower zone, not full-bleed
- Treat the photo as a document or specimen — objective, not atmospheric
- Optional: subtle grain or halftone on the photo surface

**Composition rules:**
- Warm off-white background, full bleed, no border
- Primary display type at top: massive, lowercase, left-aligned, taking up 30–40% of poster height
- 2–4 small plus or 4-pointed star marks at intentional grid intersections — sparse, precise
- Body copy block: 3–5 lines, small, between title and photo
- Photo: contained rectangle, full width or slightly inset, middle-lower zone
- Footer: key details in small type, left and right aligned

**Layout logic — where copy lands:**
- Top: Primary name in massive lowercase display, 1–2 lines, left-aligned — fills the width
- Between title and photo: Body copy — descriptive sentences, small justified or left-aligned text
- Scattered (2–3 instances): Small plus marks at grid intersections
- Middle-lower: Photo inset, contained rectangle
- Bottom left: Hours, dates, or admission — bold small + regular small alternating
- Bottom right: Website or social handle — small, right-aligned
- Bottom center (optional): One small plus mark

**Typography — visual geometry specification:**
- Primary display: Letterforms with uniform stroke weight — no thick-thin variation. Characters are moderately wide, upright, and geometric. The stroke weight is heavy enough to feel substantial but not so heavy that counters collapse — the interior spaces of letters like 'o', 'e', 'a' remain open and airy. Lowercase only — the absence of capitals signals intellectual confidence, not casualness. Characters are slightly wider than a typical grotesque — between normal and extended proportion. The display type fills the width of the poster at large scale: a two-word title should span edge to edge, with each character approximately 15–20% of the poster width. Near-black fill on warm off-white background. This is the typographic signature of the style: it should feel inevitable, not decorated.
- Body copy: The same typeface family at its lightest available weight — thin strokes, open spacing, small scale (approximately 3–4% of poster height). Justified or left-aligned in a contained column. The visual impression is of a precise, considered block of information — not a paragraph of flowing prose.
- Footer details: Alternating bold and regular weight within the same small scale — "OPENING HOURS:" in bold, "10AM – 10PM" in regular. This weight alternation creates rhythm without changing size.
- Plus marks / star marks: Simple geometric forms — perfectly symmetrical, crisp, exactly the same stroke weight as the body copy. They function as grid markers, not decoration.
- Critical: The massive display type and the tiny body copy must coexist without anything in between. There is no medium-sized type in this style. The scale jump is abrupt and intentional — it creates the intellectual tension that defines the aesthetic. Any medium-scale text breaks the system.

**Color palette:**
- Dominant (background): Warm off-white `#F0EDE8` or pale parchment `#EDE8E0`
- Primary type: Near-black `#111111` — not pure black
- Plus/star marks: Same near-black
- Photo: Desaturated or subtle duotone, mid-tones
- Optional single accent: One element in muted institutional color — slate blue, moss, or warm terracotta — used for one word or one detail only

**Texture & finish:**
- Very clean — minimal texture on the layout
- Subtle paper grain at low opacity on background
- Photo may have gentle grain
- Plus marks: crisp, precise, vector-sharp
- No ink bleed, no misregistration — this style values precision

**Output notes:**
Restraint is the entire design argument. The scale contrast between massive title and tiny body copy is the primary visual tension. Do not add elements to fill space — let the space breathe. The Studio Air reference is the clearest example of this style executed correctly: two lines of massive lowercase type, a small subtitle, two plus marks, one photo, and a minimal footer. Nothing else.
