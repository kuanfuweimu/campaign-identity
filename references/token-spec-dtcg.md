# W3C DTCG `2025.10` Design Tokens Specification Guide

When authoring `tokens.json` for a Campaign Identity's **AI Skill & Web UI handoff**, follow the stable **W3C Design Tokens Format Module (`2025.10`)** specification so tokens remain portable across Figma Variables, Tokens Studio, Style Dictionary, Terrazzo, and AI coding agents.

---

## Core Rules

1. **Reserved `$` Properties**:
   - `$value` *(required)*: The token's value. Any object containing `$value` is a token.
   - `$type` *(recommended; inheritable from parent group)*: Standard types include `color`, `dimension`, `fontFamily`, `fontWeight`, `duration`, `cubicBezier`, `number`, plus composite types (`typography`, `border`, `shadow`, `transition`).
   - `$description` *(optional but strongly recommended for AI Skills)*: Explains design intent (e.g., *"Derived from custom lettering corner radius"*).
2. **Two-Tier Architecture (Primitive → Semantic)**:
   - Define raw palette/scale/timing values under primitive groups (e.g., `primitive.color.*`, `primitive.geometry.*`).
   - Map intent-driven tokens under semantic groups using `{alias.path}` references (e.g., `semantic.button.radius.$value = "{primitive.geometry.radius-lettering}"`).
3. **Structured Units (`2025.10`)**:
   - `dimension`: `{ "value": 6, "unit": "px" }` (or `"rem"`)
   - `duration`: `{ "value": 640, "unit": "ms" }` (or `"s"`)
   - `cubicBezier`: `[0.22, 1, 0.36, 1]`
   - `color`: Standard hex or color-space object depending on target compiler (verify compatibility with the project's Figma/Style Dictionary pipeline).

---

## Mapping Campaign Pillars to Token Groups

- **`Geometry`** → `dimension` tokens for `radius`, `stroke` (ornamental lines), `spacing` scale, and `typography` scale/families.
- **`CMF`** → `color` tokens (surfaces, text, accents, scrims) + `number` tokens for digital texture/grain opacity.
- **`Audiovisual`** → `duration` + `cubicBezier` + `transition` tokens synced with motion and audio rhythm.

Use [../templates/tokens.template.json](../templates/tokens.template.json) as the starter file for every new campaign repository.
