# Article Image Standards

Use these standards for article featured images so cards, article pages, and social previews feel like one visual system.

## Production requirements

- Create images at a 16:9 aspect ratio. A source such as 1600×900 or 1920×1080 is suitable; keep important content inside the central 80% so small responsive crops remain clear.
- Save the final optimized asset in `src/images/articles/` with the article slug as the filename, preferably as WebP or PNG.
- Use dark navy or near-black foundations with cyan, teal, and blue accents from the site palette. A restrained violet accent is acceptable when it supports depth.
- Prefer one clear visual concept, strong depth, generous negative space, and readable silhouettes at card size.
- Do not include words, logos, signatures, watermarks, photorealistic people, or small UI copy that will become illegible.
- Add `image` and meaningful `imageAlt` fields to the article front matter. If an article has no image, omit both fields; the shared card template supplies the branded fallback.

## Recovered glassmorphism prompt

The exact original ChatGPT wording is not embedded in the exported PNG. The following production prompt reconstructs the instructions from the approved `advanced-ai-assisted-hiring` asset and the Revenue Data Lab design system:

> Create a polished 16:9 editorial illustration for a Revenue Data Lab article about advanced AI-assisted hiring. Place a large translucent glass candidate-profile and evaluation dashboard in the center. Connect two smaller floating glass panels on the left for recorded video and interview audio, and a larger analytics panel on the right with a competency radar and rising performance bars. Use premium glassmorphism: frosted translucent surfaces, rounded corners, layered depth, soft reflections, luminous connector nodes, and crisp cyan, teal, and electric-blue edge lighting. Add flowing abstract waves and restrained violet-magenta highlights over a deep blue background for energy and depth. Keep the composition clean, balanced, high contrast, and legible at thumbnail size. No text, letters, logos, signatures, or watermark.

## Generation and review checklist

1. Generate at the closest available 16:9 size and choose the version with the clearest single concept.
2. Confirm the focal subject remains understandable when viewed around 360 pixels wide.
3. Crop only when necessary; do not cut through the central subject or connector lines.
4. Optimize the file without flattening gradients into visible bands.
5. Check the image on both the article card and article page, then write alt text that conveys the concept rather than repeating the title.
