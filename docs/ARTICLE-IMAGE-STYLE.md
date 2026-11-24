# Article Image Generation Standard

## Visual Style

Create a premium, modern SaaS illustration in the style of high-end AI and developer tool interfaces.

- Abstract 3D glassmorphism with translucent, frosted-glass interface elements.
- Vibrant gradients blending electric blue, cobalt, violet, lavender, cyan, and soft pink.
- Soft, diffused lighting with subtle bloom and luminous edges.
- Smooth, atmospheric gradient backgrounds.
- Delicate white outlines, subtle reflections, soft shadows, and layered transparency.
- Clean geometric shapes with rounded corners.
- Sophisticated, futuristic, technical aesthetic.
- Strong visual hierarchy and generous negative space.

## Composition

- One primary visual concept, centered or slightly offset.
- Use 2-4 layered interface elements.
- Introduce subtle perspective and depth.
- Maintain a restrained, uncluttered composition.
- Use a landscape 16:9 aspect ratio.
- Generate each article image as a separate, complete image.

## Subject Selection

Read the complete article before developing the image concept.

Identify the central technical concept and represent it through an original visual metaphor. Select interface elements that communicate the specific subject of the article.

Maintain the established visual style across all articles. Change the subject and composition, not the visual identity.

## Prohibited Elements

- Pixelated waves, particle grids, and dotted backgrounds.
- Generic robots and AI mascots.
- Cliché code symbols, brackets, and terminal icons.
- Office environments, furniture, and physical accessories.
- Excessive neon lighting.
- Unnecessary charts, checkmarks, or decorative icons.
- People or photography.
- Text, headings, logos, and watermarks.
- Complex workflow diagrams.
- Repeated compositions from previous articles.

## Execution

Treat these instructions as permanent. Do not rewrite or reinterpret the visual standard for individual articles.

Only the article-specific subject and its visual representation should change.

The resulting image should feel like a sophisticated technical editorial illustration, with sufficient visual interest to work independently as an article thumbnail.

## Repository Enforcement

This standard applies to featured images for every non-test article, post, project, or conversation. Explicit `[TEST]` placeholders use the shared branded fallback and do not receive generated artwork.

Before accepting a generated image:

1. Read the complete content item and identify its single central technical concept.
2. Review every existing production image in `src/images/articles/` to avoid repeating a prior composition.
3. Use the Visual Style, Composition, Subject Selection, and Prohibited Elements sections above as fixed generation constraints.
4. Compare the candidate beside the existing production images at card size.
5. Reject and regenerate any candidate that includes a prohibited element, changes the visual identity, repeats a composition, or becomes unclear as a thumbnail.
6. Save the approved 16:9 asset under the relevant `src/images/` content folder and add accurate `image` and `imageAlt` front matter.

`src/images/articles/advanced-ai-assisted-hiring.png` is the canonical reference for materials, lighting, gradient atmosphere, and finish. It is a style reference only; its subject and composition must not be copied.
