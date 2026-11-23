# campaign-identity

A cross-disciplinary **Art Direction & Campaign Identity System** agent skill unifying **Concept, Geometry, CMF, Audiovisual (Motion & Sound), Scale & Constraints, and Collaboration (AI Skill + Design Kit)**.

Built for modern campaigns where the hero medium (3D, product, photography, or illustration) must stay coherent across **Web & UI**, **Social & Content**, **Digital Invitations**, **Print Collateral**, **Spatial/Exhibition**, **Video Production**, and **AI-assisted workflows**.

## Framework Architecture

### 6 Controlling Dimensions
1. **Concept** → `1. Core`
2. **Geometry** → `2. Typography` + `3. Graphic Elements`
3. **CMF** → `4. CMF`
4. **Audiovisual** → `5. Audiovisual`
5. **Scale & Constraints** → `1. Application`
6. **Collaboration** → `2. AI Skill & Design Kit`

### System Structure

| System Foundations | Execution & Delivery |
| :--- | :--- |
| **1. Core** — Concept & Keywords · Master KV · Logo Lockup | **1. Application** |
| **2. Typography** — Lettering · Typeface & Hierarchy · Grid | &nbsp;&nbsp;• **Digital**: Web & UI · Social & Content · Digital Invitations (H5 / Shareables / EDM) |
| **3. Graphic Elements** — 3D Forms · 2D Shapes · Lines | &nbsp;&nbsp;• **Print & Spatial**: Print Collateral · Spatial & Exhibition |
| **4. CMF** — Color · Material · Finish & Texture | **2. AI Skill & Design Kit** |
| **5. Audiovisual** — Motion · Sound | &nbsp;&nbsp;• **AI Skill**: `SKILL.md` (qualitative rules) · `tokens.json` (W3C DTCG `2025.10` values) |
| | &nbsp;&nbsp;• **Design Kit**: Figma Master Library · Shared Asset Kits (Motion / 3D / Spatial & Print) |

## Repository Contents

- [`SKILL.md`](./SKILL.md) — Core agent skill instructions and checklist
- [`references/collaboration-ops.md`](./references/collaboration-ops.md) — Multi-designer, video, spatial, and frontend collaboration playbook
- [`references/figma-canvas-organization.md`](./references/figma-canvas-organization.md) — Figma horizontal swimlane canvas architecture (`Left Drafts → Center Locked 1–5 → Right Applications`)
- [`references/token-spec-dtcg.md`](./references/token-spec-dtcg.md) — W3C DTCG `2025.10` token authoring guide
- [`references/theory-and-references.md`](./references/theory-and-references.md) — Design theory foundations, terminology boundaries, and English studio/enterprise benchmarks
- [`templates/tokens.template.json`](./templates/tokens.template.json) — Ready-to-use W3C DTCG `2025.10` starter tokens

## Installation

### Antigravity (Global Skill)

```bash
git clone https://github.com/kuanfuweimu/campaign-identity.git ~/.gemini/config/skills/campaign-identity
```

### Workspace / Project-Level Skill

```bash
git clone https://github.com/kuanfuweimu/campaign-identity.git .agents/skills/campaign-identity
```

### Other Agent Tools (Claude Code, Codex, Cursor, etc.)

Copy this directory into your agent's skills folder (e.g. `~/.claude/skills/campaign-identity/`).
