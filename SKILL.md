---
name: stamp-memory
description: Generate original small folk-print stamps from any theme, phrase, object, memory, or supplied photograph. Always use this skill when the user asks for 印章、图章、藏书票、橡皮章、手刻章、民艺小印、stamp illustration, ex libris, bookplate, or wants a photo turned into a stamp. Preserve this skill's warm paper, restrained charcoal/cobalt/vermilion/moss palette, large negative space, naive carved linework, compact human typography, and intimate keepsake tone without copying any reference image. Return both a production-ready image prompt and a generated raster image unless the user explicitly requests prompt-only.
---

# Stamp Memory

Turn any subject or supplied photograph into one original small printed emblem built from:

> warm paper + one symbolic subject + hand-cut line and mass + a restrained ink + quiet space

The result should feel found in a personal archive, bookplate drawer, market print stall, or handmade correspondence. It is a memory mark, not a corporate logo and not a reconstruction of a historical seal.

## Default Deliverable

Always create:

1. one generated raster image;
2. the exact production-ready image prompt used;
3. a short recipe naming the ink, stamp shape, carving treatment, text treatment, and originality changes.

Save generated files under `/Users/yanliu/Desktop/Claude skills/stamp-memory/` when file output is available. Return prompt-only only when the user explicitly asks for it or no image-generation tool is available.

Default to **one isolated stamp**, not a sheet, collection, mockup, or repeated pattern. Generate a stamp sheet only when the user explicitly requests multiple stamps.

## Read The Input

Extract these decisions without asking follow-up questions when the user's intent is usable:

- **Subject:** the one person, animal, plant, object, place, gesture, or memory that must remain recognizable.
- **Meaning:** the feeling or idea the mark should retain: belonging, luck, travel, growth, friendship, solitude, celebration, remembrance, or an equivalent implied by the user.
- **Signature detail:** the one feature that makes this subject distinct: a profile, hairstyle, glasses, leaf silhouette, handle, posture, window, pet markings, or object contour.
- **Source mode:** language-only concept, supplied photograph, or supplied artwork used as content reference.
- **Words:** exact user-supplied wording, or no wording. Never invent a brand, institution, date, location, or attribution.
- **Ratio:** use the requested ratio; otherwise use `1:1` for a single stamp and `3:4` for a stamp sheet.

For a broad theme, reduce it to one concrete emblem. “A summer of freedom” might become one open window with a drifting leaf; do not illustrate an entire summer scene.

When the user supplies only a photograph, infer the subject and signature detail from the image and proceed. Ask a question only when multiple subjects make the intended focal subject genuinely ambiguous.

## Visual DNA

### 1. Paper And Ink

Use a flat, front-facing paper field. Paper is the dominant color and must remain visibly unprinted.

- **Warm archive paper:** soft ivory `#F4EFE5`, chalk white `#FAF8F2`, or pale oat `#EDE5D6`.
- **Charcoal:** `#24231F` for bookish, figurative, nocturnal, or archival subjects.
- **Cobalt:** `#214F9B` for water, travel, sky, freshness, ceramics, or playful abstraction.
- **Vermilion:** `#C83A2B` for warmth, celebration, fruit, affection, or seal-like emphasis.
- **Moss:** `#65704A` for plants, food, gardens, domestic objects, or quiet natural themes.
- **Rare pale accent:** faded sky `#86AFCE` or leaf green `#4F8A62`, used only when a second color carries meaning.

Choose exactly one dominant ink. A second ink may occupy at most 8% of the printed marks. Never use more than two inks in one stamp.

Do not cover the canvas with a color wash. Do not use gradients, neon, metallic gold, candy pastels, glossy black, or full-color imagery. The limited ink logic makes the mark feel physically printed rather than digitally styled.

### 2. Negative Space And Scale

- Keep 65%-85% of the full canvas as empty paper around a single stamp.
- Let the stamp occupy 18%-34% of the canvas area by default.
- Use one broad connected quiet field, not evenly distributed gaps.
- Place the stamp at or near center for an iconic specimen, or offset it by 4%-10% for a more personal archival rhythm.
- Never add a card, frame, tabletop, hand holding the stamp, cast shadow, wax seal, rubber handle, or product mockup.
- Inside the stamp, keep 30%-55% as paper-colored negative shape so the subject remains legible when reduced.

The surrounding silence is part of the design. Enlarging the mark to fill the page destroys its collected, keepsake quality.

### 3. Shape Language

Choose one container from the subject's silhouette:

- **No border:** use for a naturally complete silhouette such as a flower, bird, vessel, hand, or bicycle.
- **Imperfect circle or oval:** use for faces, celestial subjects, fruit, animals, and soft organic motifs.
- **Soft rectangle:** use for architecture, books, portraits, objects with a vertical axis, or a short text block.
- **Irregular tablet:** use for memories, fossils, landscapes, abstract ideas, or subjects that benefit from an excavated character.
- **Tiny modular tile:** use only for a series or when the user explicitly asks for a stamp set.

Borders must be hand-cut, slightly uneven, and secondary to the subject. Avoid scalloped postage edges unless postal exchange is part of the theme. Avoid conventional Chinese seal-script borders unless the user explicitly requests that tradition.

Build the interior from one dominant motif and at most two supporting marks. Supporting marks may be a star, dot, wave, leaf, seed, ray, short line, or tiny label. Do not decorate every empty area.

### 4. Carved Drawing

Make the image printable as a small relief stamp:

- combine blunt monoline cuts with 1-4 solid ink masses;
- preserve a recognizable silhouette at thumbnail size;
- simplify anatomy and perspective into contour, cutout, and overlap;
- use 2-6 internal detail zones, never continuous realistic shading;
- include slight pressure variation, broken edges, ink skips, doubled corners, and uneven fill;
- let some lines terminate early or overshoot slightly;
- keep the imperfection controlled: the subject must remain clear.

Prefer carving decisions over drawing detail. Merge nearby shadows, open narrow gaps, thicken fragile lines, and remove details that would clog when printed at 25-45 mm.

Never use polished vector geometry, uniform icon strokes, clip-art symmetry, photorealism, pencil shading, watercolor, airbrush, 3D embossing, or generic cute mascot styling.

### 5. Typography

Text is optional and subordinate. A strong stamp may contain no text.

When text is supplied:

- preserve the exact wording and language;
- use 1-6 words, or initials plus one short word;
- use compact hand-carved capitals, narrow old-style serif, naive handwritten block letters, or restrained bookplate small caps;
- integrate text into the border, a narrow top/bottom band, or one side of the subject;
- allow uneven baseline, imperfect spacing, and slight size variation while keeping critical words readable;
- keep text under 22% of the stamp's printed area.

For Chinese, use plain hand-cut print forms with open counters and varied pressure. Do not default to seal script, pseudo-calligraphy, or decorative ancient characters. For Latin text, avoid luxury tracking, ornate scripts, blackletter, and modern geometric branding.

If no words are supplied, do not invent a title inside the image. The recipe note may name the concept outside the artwork.

### 6. Communication Tone

Communicate like a private bookplate, travel mark, garden note, family keepsake, or small gift between people:

- intimate, observant, plainspoken, and lightly poetic;
- symbolic rather than explanatory;
- warm without becoming sentimental;
- curious without becoming whimsical branding.

Avoid advertising language, slogans, calls to action, trend jargon, mystic claims, faux-historical authority, and fake institutional identity.

## Subject Decision Flow

Choose the visual reduction in this order:

1. **Does the subject have a distinctive silhouette?**
   - Yes: preserve that silhouette and use no border or a loose oval.
2. **Is identity carried by a face or portrait?**
   - Yes: preserve profile/frontality, hair mass, eyewear, and one expression cue; use an oval or soft rectangle.
3. **Is it a place or scene?**
   - Yes: retain one landmark contour plus one environmental mark; remove depth and background clutter.
4. **Is it an action or relationship?**
   - Yes: reduce it to one gesture between two forms, such as touching hands, shared thread, passing object, or mirrored posture.
5. **Is it an abstract idea?**
   - Yes: choose one concrete metaphor and use an irregular tablet or borderless emblem.

Never solve an abstract theme with unrelated decorative symbols. Every supporting mark must reinforce the chosen meaning.

## Photo-To-Stamp Workflow

When a photograph is supplied, treat it as factual content, not as a layout to trace.

1. Identify the focal subject and the 2-4 features required for recognition.
2. Choose a crop that removes most background information.
3. Collapse tones into paper, dominant ink, and optional tiny accent.
4. Merge dark regions into 1-4 printable masses.
5. Convert midtones into sparse cuts, hatching, dots, or paper openings.
6. Remove incidental texture, clutter, reflections, tiny accessories, and unimportant background objects.
7. Rebuild contours by hand with uneven pressure; never apply a simple threshold filter or auto-trace look.
8. Preserve identity, body proportions, pose logic, pet markings, object structure, and culturally meaningful details.

For portraits, keep the eyes, brow, nose direction, mouth gesture, hair silhouette, and eyewear consistent with the source. Do not beautify, age-shift, change ethnicity, invent clothing, or replace the person's expression.

For pets and objects, preserve species/object geometry and the one defining marking or construction detail. Simplification must not turn the subject into a generic icon.

## Stamp Sheet Branch

Use this branch only when the user requests multiple stamps.

- Create 6-20 unequal marks with 70%-82% overall paper visible.
- Vary container shape, scale, and ink assignment while keeping one dominant palette.
- Use loose rows, an open constellation, or an asymmetric specimen-page rhythm.
- Keep gaps visibly unequal and leave at least one large empty zone.
- Repeat one motif family, not one identical motif.
- Avoid perfect UI grids, sticker-sheet density, and evenly sized icon libraries.

## Prompt Compiler

Write the final image-generation prompt as five compact paragraphs containing only visible outcomes:

1. **Canvas:** ratio, flat warm paper, exact ink choice, stamp scale, placement, and empty-space percentage.
2. **Original construction:** chosen container, dominant motif, supporting marks, internal negative-space percentage, and asymmetry.
3. **Subject:** recognizable facts, symbolic reduction, supplied-photo features to preserve, crop, solid masses, and omitted details.
4. **Typography:** exact supplied words or explicit absence of text, type character, placement, scale, and readability.
5. **Material and exclusions:** relief-print skips, uneven pressure, paper fibers, scan softness, originality changes, and hard avoids.

Do not mention reference images, artists, studios, mood boards, this skill's name, or “in the style of.” Do not describe invisible intent as if it were a pixel.

## Originality Firewall

References provide visual grammar only. Never reproduce a visible stamp's subject treatment, border, internal cuts, wording, object arrangement, or distinctive lettering.

Before generation, change at least five of these from every supplied style reference:

- subject and symbolic metaphor;
- container shape;
- crop or viewpoint;
- dominant ink;
- solid-to-line ratio;
- negative-space shape;
- supporting marks;
- text wording;
- text location;
- stamp scale and page placement;
- edge irregularity;
- internal rhythm.

When the user supplies their own photograph, preserving identity is allowed and required; the surrounding construction, abstraction, border, text placement, and carving rhythm must still be newly designed.

## Hard Avoids

Always exclude:

- copying, tracing, or closely paraphrasing a reference stamp;
- generic logo presentation, brand identity boards, app icons, badges, stickers, or clip art;
- glossy wax seals, embossed foil, 3D rubber stamps, mockups, shadows, desks, hands, frames, or product photography;
- polished vectors, perfectly uniform strokes, flawless symmetry, smooth Bézier curves, or digital gradients;
- detailed historical pastiche, fake signatures, invented heraldry, pseudo-Asian lettering, or fake institutional marks;
- dense scenes, realistic shading, photographic backgrounds, decorative filler, or more than two inks;
- giant type, long copy, random foreign words, fake dates, URLs, QR codes, or illegible decorative text.

## Generation And Inspection

1. Parse the input and choose one symbol, one container, one dominant ink, and optional exact text.
2. Compile the five-paragraph prompt.
3. Generate a raster image with the available image-generation tool. Use a supplied image as a content reference.
4. Inspect at full size and thumbnail size.
5. Regenerate once when a quality gate fails, tightening only the failed constraint.
6. Return the image, exact prompt, and recipe.

If exact text renders incorrectly after one retry, generate a text-light or text-free base stamp and report the intended wording separately. Never claim malformed lettering is correct.

## Output Format

````markdown
**生成图**

![Stamp Memory](absolute-image-path-or-rendered-image)

**最终 Prompt**

```text
[the exact prompt used]
```

**本次配方**

- Ink: [dominant ink + optional accent]
- Shape: [container choice]
- Carving: [line/mass/negative-space treatment]
- Type: [text treatment or no text]
- Originality: [one sentence naming major structural departures from references]
````

## Quality Gate

Before returning, verify:

- Is there one isolated stamp unless a sheet was requested?
- Does the canvas use warm paper, one dominant ink, and at most one accent under 8%?
- Is 65%-85% of the full canvas empty paper?
- Does the stamp remain recognizable at thumbnail size?
- Is 30%-55% of the stamp interior open as paper-colored negative shape?
- Does the carving combine uneven lines with 1-4 solid masses and controlled print defects?
- Is the subject specific rather than a generic icon?
- Is optional text exact, compact, readable, and under 22% of the mark?
- Does the result avoid mockup, logo, sticker, polished-vector, and wax-seal aesthetics?
- When a photo is supplied, are identity and signature features preserved?
- Do at least five structural features differ from every style reference?
- Was a raster image generated unless prompt-only was requested or generation was unavailable?

## Example Triggers

- “帮我做一枚关于雨后散步的印章。”
- “把这张我和猫的照片变成一枚蓝色手刻章。”
- “做一个写着 READ SLOWLY 的藏书票小印。”
- “用 stamp-memory 生成一枚代表重新开始的印章。”
- “把这朵花简化成朱红色民艺印章，不要文字。”
- “Make this portrait into a quiet cobalt bookplate stamp.”