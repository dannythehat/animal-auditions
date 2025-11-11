# Song Matching Prompt

Use this prompt with ChatGPT-5 to assign 3 perfect songs to each character.

---

## 🤖 ChatGPT Prompt

```
You are assigning songs to 12 animal characters for a comedy singing show.

INPUT: I will provide the complete character profiles (from characters.json)

YOUR TASK: For each character, select 3 songs that:
1. Perfectly match their personality and mood
2. Create humor through the combination of animal + personality + lyrics
3. Are well-known and recognizable
4. Have clear 20-30 second sections that work standalone
5. Have karaoke versions available
6. Are family-friendly (or easily edited)

SONG SELECTION STRATEGY:
- **Song 1:** Most obvious/perfect match (audience expects this)
- **Song 2:** Surprising but brilliant choice (unexpected humor)
- **Song 3:** Wildcard (pushes the character in new direction)

For EACH song assignment, provide:

{
  "character_id": "[character-id]",
  "character_name": "[Full Name]",
  "songs": [
    {
      "song_id": "[title-artist-lowercase]",
      "title": "[Song Title]",
      "artist": "[Artist Name]",
      "genre": "[Music Genre]",
      "why_funny": "[Explain why this character singing this song is hilarious - be specific about lyrics/context]",
      "key_lyrics": "[The specific lyrics that make it funny - 1-2 lines]",
      "timestamp": "[Best 20-30 second section - e.g., '0:58-1:18']",
      "karaoke_source": "[Where to find karaoke version - YouTube channel or service]",
      "mood": "[Song mood - matches character or contrasts for comedy]",
      "visual_gag": "[Specific visual joke opportunity - e.g., 'Sloth moves in slow motion during fast chorus']",
      "difficulty": "[easy/medium/hard - based on vocal complexity]"
    }
  ]
}

GENRE DISTRIBUTION TARGET (across all 36 songs):
- Classic Rock: 6 songs
- Pop (80s-2000s): 6 songs
- Alternative/Indie: 4 songs
- Disco/Funk: 3 songs
- Country: 2 songs
- Oldies (50s-60s): 3 songs
- Musical Theater: 2 songs
- Novelty/Comedy: 4 songs
- Hip-Hop/Rap: 3 songs
- Latin/Spanish: 3 songs

CRITICAL RULES:
- NO song can be assigned to multiple characters
- Each character's 3 songs should vary in genre/mood
- Prioritize songs with iconic, quotable lyrics
- Consider visual comedy opportunities (e.g., slow animal + fast song)
- Ensure karaoke versions actually exist (check YouTube/Karaoke Version)

EXAMPLE (for reference):

Grumpy Sloth:
1. "Creep" - Radiohead (obvious match, "I'm a weirdo")
2. "Don't Stop Me Now" - Queen (ironic contrast, sloth singing upbeat song slowly)
3. "Mad World" - Gary Jules (perfect mood match)

OUTPUT FORMAT: Valid JSON array with all 12 characters and their 3 songs each (36 total).
```

---

## 📥 Input Preparation

Before running this prompt:

1. Copy entire contents of `characters.json`
2. Paste into ChatGPT conversation
3. Then provide the song matching prompt above
4. ChatGPT will generate all 36 song assignments

---

## ✅ After Generation

1. **Review All 36 Songs:** Check for quality and humor
2. **Verify Karaoke Availability:** Spot-check 5-10 songs on YouTube
3. **Check for Duplicates:** Ensure no song appears twice
4. **Genre Balance:** Confirm variety across all videos
5. **Save to File:** Copy to `song-matches.json`
6. **Checkpoint:** Would you watch these videos?

## 🔄 If Adjustments Needed

```
Regenerate songs for [Character Name]:
- Replace "[Song Title]" with something [more/less obvious]
- Focus on [specific genre or mood]
- Ensure it doesn't overlap with [other character's vibe]
```

---

**Next Step:** Once songs are approved, move to 3-scene video generation (`/scripts/scene-generation-prompt.md`)