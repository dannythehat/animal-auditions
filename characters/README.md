# 🎭 Character System

This directory contains all character profiles and data.

## 📋 Files

- **characters.json** - Master database of all 12 characters
- **[character-name].json** - Individual character files with full details
- **generation-prompt.md** - ChatGPT prompt to generate characters

## 🎨 Character Profile Schema

Each character includes:

```json
{
  "character_id": "unique-identifier",
  "name": "Full Character Name",
  "animal": "Animal Type",
  "personality": {
    "primary_mood": "Main personality trait",
    "traits": ["trait1", "trait2", "trait3"],
    "funny_quirk": "Specific comedic behavior"
  },
  "appearance": {
    "clothing": "Detailed clothing description",
    "style": "Overall aesthetic",
    "distinctive_feature": "Memorable visual element"
  },
  "voice": {
    "accent": "Accent type",
    "speaking_style": "How they talk",
    "singing_style": "Genre preferences"
  },
  "midjourney_prompt": "Complete image generation prompt",
  "song_matches": []
}
```

## ✅ Quality Checklist

Before approving characters:

- [ ] Each personality is distinct and non-overlapping
- [ ] Visual descriptions are detailed enough for AI image generation
- [ ] Accents enhance comedy and match well-known songs
- [ ] Funny quirks work visually in short videos
- [ ] Characters appeal to both kids and adults
- [ ] No offensive stereotypes or problematic content

## 🚀 Next Steps

1. Generate all 12 characters using `generation-prompt.md`
2. Review and refine each character
3. Create Midjourney images using provided prompts
4. Move to song matching phase