---
name: campaign-identity
description: >-
  Cross-disciplinary Art Direction & Campaign Identity System framework spanning Concept,
  Geometry, CMF, Audiovisual (Motion & Sound), Scale & Constraints, and Collaboration
  (AI Skill with W3C DTCG tokens + Design Kit). Use this skill when planning, structuring,
  auditing, or documenting a campaign visual identity, 3D/product-led KV system, landing page,
  social/invitation collateral, offline print/spatial experience, or multi-designer handoff.
---

# Campaign Identity System (Art Direction & Cross-Disciplinary Framework)

Use this framework to architect a complete **Campaign Identity** as a unified, cross-disciplinary visual system—whether the hero medium is 3D, photography, physical product, or illustration.

---

## 6 Controlling Dimensions

Every decision in the system maps to one of six controlling pillars:

1. **Concept** — Creative direction, keywords, narrative anchor (`Core`)
2. **Geometry** — Structural form language shared across type, 3D, 2D, and UI (`Typography` + `Graphic Elements`)
3. **CMF** — Color, Material, and Finish unifying 3D shaders, screen surfaces, and physical substrates (`CMF`)
4. **Audiovisual** — Time-based rhythm binding motion curves and sound design (`Audiovisual`)
5. **Scale & Constraints** — Optical/physical adaptation across viewports, viewing distances, and media limits (`Application`)
6. **Collaboration** — Tooling, tokens, kits, and governance for humans and AI agents (`AI Skill & Design Kit`)

---

## Part I: System Foundations (Left Column)

### 1. Core
- **a. Concept & Keywords**: One-sentence creative premise + 3–5 concrete keywords governing every downstream choice.
- **b. Master KV**: Flagship visual anchor (horizontal `16:9` + vertical `9:16` / `3:4`) with safe areas for lockups and copy. The hero slot (`Imagery`) is swappable: 3D, product photography, illustration, or generative art.
- **c. Logo Lockup**: Primary & co-branding lockups, clear space (`X` unit), optical area balance (never raw height-matching), and minimum legible print/digital sizes.

### 2. Typography
- **a. Lettering**: Bespoke title lockups (`Custom Lettering`, e.g., event/chapter titles) sharing unified stroke/corner geometry. Prepare desktop single-line, mobile stacked, vector SVG (monochrome/reversed), textured/3D, and outline variants.
- **b. Typeface & Hierarchy**: Functional typeface pairing, Type Scale ratio, line-height, and bilingual rules.
- **c. Grid**: Structural layout & typographic grid controlling margins, columns, and spatial rhythm.

### 3. Graphic Elements
Follow a strict non-overlapping `3D → 2D → 1D` taxonomy aligned with `Geometry`:
- **a. 3D Forms**: Dimensional objects, primitives, bevel/proportion rules, and camera/lighting conventions.
- **b. 2D Shapes**: Flat geometric shapes, containers, masks, and supergraphics derived from the core form language.
- **c. Lines**: Ornamental linework (hairline rules, corner brackets, frames, micro-accents) with fixed stroke weights and end-cap styles matching the lettering geometry.

### 4. CMF (Color, Material, Finish)
- **a. Color**: Primary, secondary, accent, and neutral palette with explicit usage ratios (e.g., `70 / 20 / 10`), mapped across HEX/sRGB, CMYK, and Pantone.
- **b. Material**: 3D shader logic (roughness, metallic, transmission, lighting) and physical substrates.
- **c. Finish & Texture**: Digital surface grain/noise (seamless tiles, blend modes, safe opacity ranges) and physical print finishes (specialty paper, foil stamping, spot UV, debossing).

### 5. Audiovisual
Treat motion and sound as one synchronized time-based discipline:
- **a. Motion**: Motion personality, standard `cubic-bezier` easing curves, duration tiers, hero seamless loops, and component transitions.
- **b. Sound**: Theme BGM, ambient loops, BPM beat anchors synced to motion keyframes, UI/transition SFX stingers, and timbre aligned with CMF.

---

## Part II: Execution & Delivery (Right Column)

### 1. Application (Governed by `Scale & Constraints`)

Apply **3 Visual Density Tiers** across all touchpoints so elements never fight each other:
- **Full (Hero)**: 3D + CMF + Custom Lettering + Lines + Audiovisual (Hero screen, opening film, main poster).
- **Standard (Campaign)**: 2D Shapes + restrained texture + Lines (social templates, secondary sections, merch).
- **Minimal (Utility)**: Clean surface + Functional Typography + minimal lines (forms, schedules, wayfinding, dense info).

#### a. Digital
- **i. Web & UI**:
  - Inherit `Geometry` (button/card `border-radius` matches lettering corners; borders match ornamental lines).
  - Translate `CMF` via accessible contrast scrims and lightweight seamless texture overlays (never multi-MB full-bleed bitmaps).
  - Define 3D delivery & mobile degradation (WebGL vs. alpha video/WebP fallback) and `prefers-reduced-motion`.
  - Render `Custom Lettering` as crisp SVG wrapped in semantic `<h1>`/`<h2>` with accessible text for SEO.
  - Provide an explicit, muted-by-default **Sound Toggle**; pause audio when tab is hidden.
  - Define clear integration boundaries with the host website's navbar, footer, and primary CTAs.
- **ii. Social & Content**:
  - Lock modular multi-ratio templates (`9:16`, `3:4`, `4:5`, `1:1`, `16:9`, `2.35:1`).
  - Respect platform UI safe zones (Reels/TikTok right rail & bottom caption, X crop, Xiaohongshu tags).
  - Compensate for platform compression (avoid ultra-fine gradients/micro-grain that band or turn muddy).
  - Ensure **1–2s visual hook**, **sound-off legibility**, and **thumbnail readability** at ~180px width.
- **iii. Digital Invitations**:
  - **Interactive H5 / RSVP**: Reuse Web UI tokens + optional user-customizable invite cards.
  - **Private Shareables (WeChat / Discord / Slack)**: Put Hero KV + title in the top/center preview crop; keep time/location/QR in a clean minimal zone.
  - **EDM (Email)**: `600px` max width, export 3D/lettering headers as static retina images or light GIFs, fall back to system fonts for body copy, and test mobile Dark Mode color inversion.

#### b. Print & Spatial
- **i. Print Collateral**:
  - Enforce minimum print size for logos and minimum stroke width (`≥0.25pt` offset, `≥0.4pt` reversed, `≥0.5–1pt` silkscreen/UV/large format).
  - Use **single black (`K100`)** for small text, logos, and fine lines (prevents misregistration blur); use **rich black** (e.g., `C30 M20 Y20 K100`) for large dark fills.
  - Clear noisy 3D/textures behind logos; verify CMYK output via physical press proof before batch printing.
- **ii. Spatial & Exhibition**:
  - Apply viewing-distance scaling: **Near (<1m)** for tactile finishes & print detail; **Mid (1–3m)** at eye level (`1.2–1.8m`), keeping key logos/titles **above the `0–90cm` crowd occlusion zone** on photo backdrops; **Far (3m+)** stripped to bold silhouettes, lettering, and high contrast.
  - Confirm exact pixel resolution for stage LED walls and supply clean, text-free seamless loops.

### 2. AI Skill & Design Kit (Governed by `Collaboration`)
- **a. AI Skill** (for AI coding/design agents — stored in GitHub):
  - **i. `SKILL.md`**: Qualitative rules, density tiers, platform constraints, and anti-slop guardrails.
  - **ii. `tokens.json`**: Quantitative parameters in **W3C DTCG `2025.10`** format (`$value`, `$type`, `$description`, `{alias}`) + compiled `tokens.css`. See [references/token-spec-dtcg.md](./references/token-spec-dtcg.md) and [templates/tokens.template.json](./templates/tokens.template.json).
- **b. Design Kit** (for human collaborators):
  - **i. Figma**: Locked `00_Master_Library` (Variables + Logo/Lettering/Ornament components) + horizontal swimlane exploration board (`Left Drafts → Center Locked 1–5 → Right Applications`). See [references/figma-canvas-organization.md](./references/figma-canvas-organization.md).
  - **ii. Shared Asset Directory**: Role-specific handoff kits (`Motion_Starter_Kit` with audio stems, `Spatial_&_Print_Kit` with lightweight 3D FBX/GLB models & CMYK/Pantone specs). See [references/collaboration-ops.md](./references/collaboration-ops.md).

For canonical design theory, terminology boundaries (`Scale` vs. `Size`, `Lettering` vs. `Typography`), and English industry benchmarks, see [references/theory-and-references.md](./references/theory-and-references.md).

---

## Workflow: Using This Skill on a New Project

1. **Lock Core & 6 Pillars**: Define `Concept & Keywords`, `Master KV`, `Logo Lockup`, and shared cross-disciplinary parameters (`Geometry`, `CMF`, `Audiovisual`).
2. **Audit Scale & Constraints**: Before scaling production, check every target touchpoint (Web UI, Social, Invitations, Print, Spatial) against optical sizing, compression, contrast, print legibility, and occlusion limits.
3. **Freeze `v1.0` & Package Kits**:
   - Export `tokens.json` (W3C DTCG `2025.10`) + `tokens.css` and project-specific `SKILL.md` to GitHub.
   - Publish locked Figma Master Library and cloud handoff kits for video/spatial teams.
4. **Art Direction Gates**: Review first 2–3 social/print samples, video styleframes + animatic (before final render), and spatial renders + physical press proofs before launch.
