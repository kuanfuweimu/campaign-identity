# Multi-Disciplinary Collaboration & Design Ops Guide

Use this reference when coordinating a Campaign Identity across **Frontend Engineers, AI Agents, Social Designers, Multiple Graphic/3D Designers, Video Production, and Offline Spatial/Print Teams**.

---

## 1. Platform Split (Don't Force Non-Coders into GitHub)

Use **one lightweight Hub page** (Notion / Feishu / GitHub README) as the single entry point listing the current frozen version (`v1.0`), core red lines, and direct links to four role-native workspaces:

| Role | Primary Workspace | What Lives There |
| :--- | :--- | :--- |
| **Lead / Frontend / AI Agents** | **GitHub** | `SKILL.md`, `tokens.json` (W3C DTCG), `tokens.css`, lightweight SVGs (Logos, Custom Lettering, Lines), seamless Texture tiles, Lottie JSON, compressed KV reference images, Landing Page code |
| **Social / Graphic / UI Designers** | **Figma (Team Library)** | Locked read-only `00_Master_Library` (Variables, Logo/Lettering/Ornament components) + working files (`01_Social_Templates`, `02_Web_UI`, `03_Print_Layouts`) |
| **Video & Motion Production** | **Cloud Drive / NAS + Frame.io** | `Motion_Starter_Kit` + timecoded review links |
| **Offline Experience / Spatial & Print** | **Cloud Drive / NAS** | `Spatial_&_Print_Kit` + print-ready CMYK PDF/X-1a exports |

---

## 2. Role-Specific Handoff Kits

### `Motion_Starter_Kit` (For Video & Motion Teams)
- Layered vector Custom Lettering & Logo files (`AI` / `SVG`)
- Pre-rendered 3D alpha assets (`ProRes 4444` or `EXR` sequences)
- Seamless Texture overlay loops
- **Master BGM + separated Audio Stems** (drums, synth/melody, SFX) with BPM noted so editors can cut directly on beat
- 1-page Tech Spec: frame rate (`30fps` or `60fps`), color space (`Rec.709`), easing reference, and opening/transition samples

### `Spatial_&_Print_Kit` (For Offline Experience & Print Vendors)
- Vector Logos & co-branding lockup rules (`AI` / `PDF`)
- **Lightweight 3D models (`FBX` / `GLB`)** so spatial designers can drop hero forms straight into venue/booth renders
- CMYK + Pantone color sheet + physical CMF/paper/finish reference photos
- Clean, text-free LED wall loops matched to the venue's exact pixel resolution

---

## 3. Shared Cloud Directory Structure

Prevent accidental overwrites across multiple designers:

```text
00_MASTER_LOCKED/     # Lead-only write access: final KV, Lettering, Logos, CMF, Audio Masters
01_WIP_Designers/     # Individual designer folders (by name or module)
02_Motion_&_Video/    # Project files, Styleframes, Animatics, Stems, Review Cuts
03_Social_&_Comms/    # Platform schedules, social posts, Digital Invitations / EDM
04_Spatial_&_Print/   # Venue renders, outlined CMYK print files, press proof photos
05_FINAL_EXPORT/      # Approved launch-ready assets only
```

---

## 4. Version Freeze & Art Direction Gates

1. **`v1.0` Core Freeze**: Lock `Logo Lockup`, `Custom Lettering`, primary palette, functional typefaces, and BGM BPM **before** social, video, spatial, and frontend teams start parallel production. Any subsequent change increments version (`v1.1`) with an explicit **Changelog** notifying affected roles.
2. **Three Mandatory Art Direction Gates**:
   - **Social & Print**: Approve the **first 2–3 samples** (verify visual density tier and safe zones) before batch production.
   - **Video**: Approve **Styleframes + Animatic** (timing/beat sync) before anyone runs heavy 3D rendering.
   - **Offline Spatial & Print**: Approve **venue renders** (check logo scale and `0–90cm` crowd occlusion zone) and inspect a **physical color/detail proof** before full print run.
