---
name: xxd-panel-117
description: "Create XXD Panel 117 raster artwork from a photograph by extracting one core theme, visual anchor and emotional relationship, then recomposing a small stamp-like subject with fine hand-drawn lines, pale flat pastel colours, paper texture, light collage and intentional whitespace. Use when the user invokes xxd-panel-117 or requests this fine-line pale-colour editorial style. Supports isolated image and directory inputs, strict 50:50 comparisons, design-only and wallpapers."
---

# XXD Panel 117

Create finished PNG artwork from the current user-supplied photograph or image directory. Read `references/original-prompt/zh-CN.md` completely immediately before every generation. That Chinese source brief is the sole creative and aesthetic authority; never replace it with a summary, translation, README, sample or another Panel.

## Delivery contract

- Each source photograph produces its own independent output. Never combine photographs or reuse another source's subject, wording or result.
- The original delivery is 3:4 portrait, photograph above and design below, each exactly 50%.
- Support `top-bottom`, `left-right`, `design-only` and `wallpaper-pack`. For an explicitly selected non-default mode, the delivery adapter overrides only the original spatial instructions: map above/below to left/right for `left-right`; for design-only or wallpaper use the full canvas for design with the original as invisible reference. Keep every aesthetic instruction unchanged.
- Comparison modes have exactly two equal regions and no title band, footer, inset, grid or third region.
- A directory is explicit batch intent. Inventory supported images recursively in stable order, resolve shared settings once, process every source independently and report successes and failures.
- Resolve modes, sizes, text mode, locale, wallpaper relationship, device sizes and output root from the current request and `references/runtime-preferences.md` before generation. Do not silently infer unresolved delivery preferences.

## Prompt assembly

Concatenate the complete verbatim Chinese brief, a short delivery preamble, exactly one selected mode contract, exactly one text contract and the user's explicit non-style requirements. Add no external palette, fixed slogan or aesthetic theory.

Text modes are `prompt`, `exact` and `none`. Resolve the locale explicitly. Prompt mode creates sparse source-grounded wording in that locale with the brief's fine, natural, slightly handwritten typography. Exact mode preserves the user's wording verbatim. None mode permits no letters, numbers, logos, labels or pseudo-text. Sample production uses intelligent English copy derived independently from each photograph.

Prefer the built-in image tool. Generate each complete output in one pass from its current original photograph. Never restylise an intermediate design or another Panel's image. If no compatible route is available, request an enabled image route or a voluntarily provided API key without exposing secrets. Use `scripts/compose_panel.py` only for precise raster sizing, pixel-preserving composition or audits, not to invent the art.

## Acceptance and output

Inspect each result at full and thumbnail size. Confirm source identity and ratio; for comparison modes, also confirm correct split direction and exact midpoint. The design must extract one core theme, visual anchor and emotional relationship; use fine outlines, very few interior lines, pale flat colour, near-white paper and optional light collage; keep the stamp-scale subject smaller than the surrounding deliberate whitespace. Colour comes from 2–4 source colours. Avoid tracing each object, complete backgrounds, oversized subjects, realistic details, smooth vector styling and templated type. Verify text mode and locale, and reject third bands, insets, watermarks and second-pass artefacts.

Write final PNGs directly inside one fresh task directory under `~/Desktop/xxd/xxd-panel-117/` or the explicit output root. Use collision-safe filenames and no source/mode/size subdirectories or automatic contact sheet. Clean delivery images with the available `xxd-strip-ai-meta` workflow and verify cleanup before publishing.

For linked wallpapers, generate one anchor from the original photograph, then independently recompose each remaining device from the original plus that anchor; this establishes continuity without repeatedly restylising a result. Independent wallpapers use only the original.

## References

- `references/original-prompt/zh-CN.md` — canonical runtime brief
- `references/original-prompt/README.md` — reading translations and authority
- `references/runtime-preferences.md` — safe delivery-preference reuse
- `references/xxd-panel-117-prompt.zh-CN.md` and `references/xxd-panel-117-prompt.en.md` — delivery adapters
