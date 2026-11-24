# Article Images and Unified Content Cards

## 1. Summary

- **Verified:** Added original 16:9 featured images for the two substantive published articles that lacked images.
- **Verified:** Unified article, project, and conversation card media through one shared Nunjucks partial and one shared responsive CSS treatment.
- **Verified:** Preserved type-specific fallback icons for cards without media.

## 2. Requirements

- Follow the Revenue Data Lab image and visual guidance.
- Create images for substantive articles missing them.
- Make article, project, and conversation cards use the same card-media style on the homepage and section pages.
- Build, test, commit, push to `main`, and verify production.

## 3. Files Created or Modified

- Created: `src/_includes/card-media.njk`
- Created: `src/images/articles/building-your-first-ai-agent-python-crm.png`
- Created: `src/images/articles/matching-customer-records-hubspot-financial-system.png`
- Modified: `src/_includes/article-item.njk`
- Modified: `src/_includes/project-card.njk`
- Modified: `src/_includes/episode-card.njk`
- Modified: `src/articles/building-your-first-ai-agent-python-crm.md`
- Modified: `src/articles/matching-customer-records-hubspot-financial-system.md`
- Modified: `src/css/style.css`

## 4. Implementation Details

- **Verified:** Used built-in ImageGen mode to produce both project-bound PNG assets at 1672×941.
- AI-agent prompt concept: a central glass AI orchestration core connecting fictional CRM rows, approved Python tool modules, and pipeline analytics through a controlled request/result loop; deep navy with cyan, teal, blue, and restrained violet; no text, logos, or watermark.
- Record-reconciliation prompt concept: CRM company cards and financial account records feeding a human-reviewed matching workspace with exact, ambiguous, and one-to-many relationships; deep navy with cyan, teal, blue, and restrained violet; no text, logos, or watermark.
- Replaced article-only media class names with generic `cardMedia`, `cardMediaFallback`, and `cardMediaFallbackIcon` classes.
- Added a reusable partial that renders a responsive image when available or a branded fallback with the appropriate content-type icon.
- Left the explicit `[TEST]` article placeholders on the standard fallback rather than generating production artwork for layout fixtures.

## 5. Tests and Results

- **Verified:** `npm run build` passed; Eleventy copied 45 assets and wrote 20 pages.
- **Verified:** `git diff --check` passed.
- **Verified:** Playwright exercised `/`, `/articles/`, `/projects/`, and `/conversations/` at 1440px and 390px widths.
- **Verified:** All rendered card-media areas measured exactly 16:9 (`1.777778`).
- **Verified:** All four page types had zero horizontal overflow at 390px.
- **Verified:** Homepage loaded all three article images at 1672×941.
- **Verified:** Project and conversation fallbacks rendered their corresponding icons.
- **Verified:** Browser console contained no errors or warnings; only the Eleventy live-reload connection message appeared.
- **Verified:** Netlify production returned both generated image assets with the expected byte sizes and served the shared card markup on the homepage and all three section pages.
- **Verified:** Production Playwright checks passed at 1440px and 390px with exact 16:9 media, zero horizontal overflow, and no console messages.

## 6. Problems Found and Resolved

- The article card media styles were scoped to article-specific class names. They were generalized and moved behind one shared partial so all content types cannot drift independently.
- Projects and conversations without images previously had no media region. They now use the same 16:9 branded fallback as articles.

## 7. Unresolved Issues

- The repository still contains published `[TEST]` content fixtures. Removing or drafting those entries was outside this task.
- Pre-existing dependency advisories were not changed because dependency remediation was outside this task.

## 8. Acceptance Criteria Status

- **Verified:** Both substantive image-less articles now have topic-specific featured images and alt text.
- **Verified:** Article, project, and conversation cards use one shared media implementation on homepage and section pages.
- **Verified:** Responsive layout, fallbacks, build output, and browser behavior pass locally.
- **Verified:** Commit `f09298a` was pushed to `main`, Netlify deployed it, and the live site passed direct asset checks plus desktop/mobile browser verification.

## 9. Recommended Next Steps

- Replace the `[TEST]` fixtures with real projects and conversations as content becomes available; the shared fallback will remain consistent until real media is supplied.

AUTOMATION_STATUS: PASS
