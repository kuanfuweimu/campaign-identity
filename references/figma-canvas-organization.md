# Figma Canvas & File Organization Guide

Use this layout when developing a **Campaign Identity** in Figma so exploration drafts remain visually connected to the locked system without confusing collaborators.

---

## 1. Horizontal Swimlane Canvas Architecture

Organize the Art Direction board along two clear axes:

- **X-Axis (Left → Right) = Convergence / Maturity**:
  `Raw References & Brief` → `Exploration Drafts (v0.1 → v0.3)` → `Shortlist Candidates` → **Center Locked System (`1–5`)** → `Right Applications & Kit`
- **Y-Axis (Top → Bottom) = Strict Row Alignment (`1–5`)**:
  Every draft row on the left aligns horizontally with its corresponding locked module in the center system block.

```text
   [ LEFT: DRAFTS (Diverge → Converge) ]                      [ CENTER: LOCKED 1–5 ]
───────────────────────────────────────────────────────────┬──────────────────────────
Row 1  Brief/Refs ──► Concept Notes ──► KV Directions A/B/C ──► 1. Core
                                      └─ Logo Lockup Tests │    Concept / Master KV / Logo
───────────────────────────────────────────────────────────┼──────────────────────────
Row 2  Type Audition ──► Custom Lettering Iterations (v1–v3)──► 2. Typography
                       └─ Type Scale & Grid Experiments    │    Lettering / Typeface / Grid
───────────────────────────────────────────────────────────┼──────────────────────────
Row 3  Form Refs ──► 3D Bevel/Form Tests ──► 2D & Line Tests──► 3. Graphic Elements
                                                           │    3D Forms / 2D Shapes / Lines
───────────────────────────────────────────────────────────┼──────────────────────────
Row 4  Palettes A/B/C ──► Shader Tests ──► Grain/Print Refs ──► 4. CMF
                                                           │    Color / Material / Finish
───────────────────────────────────────────────────────────┼──────────────────────────
Row 5  Motion Refs ──► Styleframes ──► Audio / BPM Notes   ──► 5. Audiovisual
                                                           │    Motion / Sound
───────────────────────────────────────────────────────────┴──────────────────────────
```

---

## 2. Guardrails to Keep Drafts Clean

1. **Shortlist Column Rule**: Always place the strongest / latest candidate directly adjacent to the left edge of the locked system block. Keep earlier rejected iterations farther left (never delete them—they are valuable for retrospectives and portfolio process pages).
2. **Figma Sections (`Shift + S`) with Visual Boundary**:
   - Wrap each left swimlane in a neutral, low-contrast section (`Draft 01 - Core` through `Draft 05 - Audiovisual`).
   - Wrap the center locked system in a distinct high-contrast section (`LOCKED v1.0`).
   - Collaborators should tell at a glance: light/neutral = WIP drafts (do not pull); locked color = single source of truth.
3. **Solo Exploration vs. Multi-Designer Handoff Split**:
   - **During Exploration**: Keep Left Drafts + Center `1–5` + early Right Application tests on one master canvas so cross-module geometry checks (e.g., lettering corner radius ↔ 3D bevel ↔ UI button radius) happen at a glance.
   - **At `v1.0` Freeze**: Promote locked components and Figma Variables into a clean, read-only page **`00_Master_Library`** (published via Team Library). Keep the full exploration canvas intact on **`99_Process_&_Drafts`** (or **`01_Art_Direction_Board`**) so social/UI/print collaborators never accidentally copy outdated drafts.
