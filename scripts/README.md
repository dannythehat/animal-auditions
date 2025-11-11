# 🎬 Video Scene Generation Scripts

This directory contains ChatGPT prompts for generating 3-scene video breakdowns.

## 📋 Files

- **scene-generation-prompt.md** - Main prompt for creating 3-scene video plans
- **scene-template.json** - JSON schema for video scenes
- **examples/** - Sample generated scenes for reference

## 🎯 What This System Does

Takes a **character + song** and generates a complete 24-second video plan with:

- **Scene 1 (0-8s):** Setup and character introduction
- **Scene 2 (8-16s):** Main performance/singing
- **Scene 3 (16-24s):** Punchline/comedic payoff

Each scene includes:
- Visual description for Canva
- Character actions/expressions
- Text overlays
- Audio timing
- Specific lyrics
- Background/lighting details

## 🔄 Workflow

1. **Input:** Character profile + Song assignment
2. **Process:** Run through ChatGPT scene generation prompt
3. **Output:** Complete 3-scene breakdown ready for production
4. **Review:** Check for visual comedy and pacing
5. **Produce:** Use breakdown to create actual video

## ✅ Quality Checklist

Each generated scene plan must have:

- [ ] Clear visual variety across 3 scenes (different angles/lighting)
- [ ] Comedic build (setup → build → punchline structure)
- [ ] Specific actionable instructions for Canva editing
- [ ] Timing that matches audio perfectly
- [ ] Text overlays that enhance (not distract from) comedy
- [ ] Character personality shines through in every scene

## 🚀 Usage

Generate scenes for ONE video at a time, or batch-generate all 36 at once.

**Recommended:** Generate 3 test videos first, produce them, then generate the rest.

---

**Next Step:** Use generated scene plans in production workflow (`/production`)