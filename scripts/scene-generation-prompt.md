# 3-Scene Video Generation Prompt

Use this prompt with ChatGPT-5 to generate complete video production plans.

---

## 🤖 ChatGPT Prompt

```
You are creating detailed 3-scene video production plans for a comedy singing show.

Each video is 24 seconds total (3 scenes × 8 seconds each).

INPUT: I will provide:
1. Complete character profile
2. Assigned song details

YOUR TASK: Generate a complete 3-scene breakdown that:
- Tells a comedic story across 24 seconds
- Uses setup → build → punchline structure
- Provides specific visual instructions for Canva editing
- Matches character personality perfectly
- Creates visual variety across scenes
- Times perfectly with audio/lyrics

OUTPUT STRUCTURE:

{
  "video_id": "[character-id]-[song-id]",
  "character_name": "[Full Character Name]",
  "song_title": "[Song Title - Artist]",
  "total_duration": "24 seconds",
  "comedy_concept": "[One-sentence description of the overall joke/concept]",
  
  "scene_1": {
    "duration": "8 seconds",
    "timestamp": "0:00-0:08",
    "purpose": "Setup - Introduce character and context",
    
    "visual": {
      "shot_type": "[Wide/Medium/Close-up]",
      "background": "[Detailed background description for Canva]",
      "lighting": "[Lighting mood - e.g., spotlight, dim, bright]",
      "color_scheme": "[Dominant colors - e.g., purple/blue moody tones]"
    },
    
    "character_action": "[Specific actions/expressions - e.g., 'Slowly walks on stage, looks unimpressed, sighs heavily']",
    
    "text_overlay": {
      "text": "[Exact text to display - or null if none]",
      "position": "[top/center/bottom]",
      "style": "[Bold white with black outline / etc]",
      "timing": "[When to appear - e.g., '0:02-0:06']"
    },
    
    "audio": {
      "lyrics": "[Specific lyrics sung in this scene]",
      "vocal_direction": "[How they sing - e.g., 'Monotone, unenthusiastic']"
    }
  },
  
  "scene_2": {
    "duration": "8 seconds",
    "timestamp": "0:08-0:16",
    "purpose": "Build - Main performance, escalate comedy",
    
    "visual": {
      "shot_type": "[Different from scene 1]",
      "background": "[New background or modified version]",
      "lighting": "[Change in lighting for variety]",
      "color_scheme": "[Adjust colors]"
    },
    
    "character_action": "[Main performance actions]",
    
    "text_overlay": {
      "text": "[Text or null]",
      "position": "[position]",
      "style": "[style]",
      "timing": "[timing]"
    },
    
    "audio": {
      "lyrics": "[Key lyrics - usually the hook/chorus]",
      "vocal_direction": "[Singing style]"
    }
  },
  
  "scene_3": {
    "duration": "8 seconds",
    "timestamp": "0:16-0:24",
    "purpose": "Punchline - Comedic payoff",
    
    "visual": {
      "shot_type": "[Final shot - often wide for payoff]",
      "background": "[Final background]",
      "lighting": "[Final lighting state]",
      "color_scheme": "[colors]"
    },
    
    "character_action": "[Punchline action - e.g., 'Drops mic in slow motion, walks off stage']",
    
    "text_overlay": {
      "text": "[Punchline text - e.g., 'He's not wrong... 🎤']",
      "position": "[position]",
      "style": "[style]",
      "timing": "[timing]"
    },
    
    "audio": {
      "lyrics": "[Final lyrics]",
      "vocal_direction": "[How they finish]"
    }
  },
  
  "canva_instructions": {
    "template_style": "[Overall Canva template approach]",
    "transitions": "[How to transition between scenes - cuts/fades/etc]",
    "effects": "[Any special effects - slow motion, zoom, etc]",
    "aspect_ratio": "9:16 (vertical for social media)"
  },
  
  "social_media": {
    "title": "[Catchy video title - under 60 characters]",
    "description": "[Engaging description - 2-3 sentences]",
    "hashtags": ["[tag1]", "[tag2]", "[tag3]", "[tag4]", "[tag5]"]
  }
}

CRITICAL REQUIREMENTS:
- Each scene must be VISUALLY DISTINCT (different shot types, backgrounds, or lighting)
- Comedy must BUILD across scenes (not just repeat the same joke)
- Character personality must be evident in EVERY scene
- Text overlays should ENHANCE comedy, not explain it
- Timing must be PRECISE (8 seconds per scene, no exceptions)
- All instructions must be ACTIONABLE in Canva (no complex VFX)

COMEDY PRINCIPLES:
- Setup establishes expectation
- Build escalates or subverts expectation
- Punchline delivers unexpected payoff
- Visual and audio comedy should complement each other
- Character quirks should be exaggerated but consistent

OUTPUT FORMAT: Valid JSON object with complete scene breakdown.
```

---

## 📥 Input Format

Provide ChatGPT with:

```
CHARACTER:
[Paste complete character profile from characters.json]

SONG:
[Paste song assignment from song-matches.json]

Generate the 3-scene video breakdown.
```

---

## ✅ After Generation

1. **Review Scene Flow:** Does it tell a coherent story?
2. **Check Visual Variety:** Are the 3 scenes distinct?
3. **Verify Comedy:** Is the punchline strong?
4. **Timing Check:** Does it fit 24 seconds?
5. **Canva Feasibility:** Can you actually execute this?
6. **Save to File:** Copy to `/production/video-plans/[video-id].json`

## 🔄 If Regeneration Needed

```
Regenerate scene [1/2/3] with these changes:
- [Specific feedback]
- Make it more [visual/funny/character-driven]
- Change [specific element]
```

---

## 💡 Pro Tips

- Generate 3 test videos first before batch-generating all 36
- Keep successful scene structures as templates
- Note which comedy patterns work best
- Iterate based on actual production experience

---

**Next Step:** Use scene plans in production workflow (`/production/checklist.md`)