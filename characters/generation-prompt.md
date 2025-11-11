# Character Generation Prompt

Use this prompt with ChatGPT-5 to generate all 12 character profiles.

---

## 🤖 ChatGPT Prompt

```
You are creating 12 unique animal characters for a comedy singing show called "Animal Auditions."

Each character will perform 3 songs that match their personality perfectly, creating humor through the combination of animal traits, personality, and song choice.

Generate 12 complete character profiles following this exact structure:

REQUIREMENTS:
- 12 different animals (variety of mammals, birds, reptiles)
- 12 distinct personality archetypes (no overlap)
- Accents that work well with English, Spanish, or well-known international songs
- Clothing and appearance that visually communicate personality
- Funny quirks that work in 24-second videos
- Family-friendly but clever (appeals to kids AND adults)

CHARACTER ARCHETYPES TO COVER:
1. Grumpy/Melancholic
2. Vain/Narcissistic
3. Anxious/Nervous
4. Overconfident/Cocky
5. Dramatic/Theatrical
6. Zen/Too-Chill
7. Angry/Aggressive
8. Clumsy/Awkward
9. Old/Wise
10. Hyperactive/Manic
11. Sassy/Sarcastic
12. Overly Romantic

For EACH character, provide:

{
  "character_id": "[animal-name-lowercase]",
  "name": "[First Name] the [Adjective] [Animal]",
  "animal": "[Animal Type]",
  "personality": {
    "primary_mood": "[Main personality trait]",
    "traits": ["[trait1]", "[trait2]", "[trait3]", "[trait4]", "[trait5]"],
    "funny_quirk": "[Specific comedic behavior that works visually]"
  },
  "appearance": {
    "clothing": "[Detailed clothing description matching personality]",
    "style": "[Overall aesthetic - e.g., disheveled, polished, eccentric]",
    "distinctive_feature": "[Memorable visual element - e.g., always wears sunglasses]"
  },
  "voice": {
    "accent": "[Specific accent type]",
    "speaking_style": "[How they talk - pace, tone, verbal tics]",
    "singing_style": "[Music genres that fit - e.g., grunge, disco, opera]"
  },
  "midjourney_prompt": "[Complete Midjourney prompt for generating this character: 'Professional portrait photo of a [description], standing upright, [clothing details], realistic fur/feathers, studio lighting, plain background, full body shot, 4K --ar 9:16 --v 6']",
  "song_matches": []
}

OUTPUT FORMAT: Valid JSON array with all 12 characters.

CRITICAL: Ensure each character is COMPLETELY UNIQUE. No personality overlap. Each should be instantly recognizable and memorable.
```

---

## ✅ After Generation

1. **Review Output:** Check for uniqueness and quality
2. **Validate JSON:** Ensure proper formatting
3. **Save to File:** Copy to `characters.json`
4. **Create Individual Files:** Split into separate character files
5. **Checkpoint:** Do all 12 characters feel distinct and funny?

## 🔄 If Regeneration Needed

If any characters feel weak or overlapping:

```
Regenerate character #[X] with these adjustments:
- [Specific feedback]
- Ensure it doesn't overlap with [other character]
- Emphasize [specific trait]
```

---

**Next Step:** Once characters are approved, move to song matching (`/songs/matching-prompt.md`)