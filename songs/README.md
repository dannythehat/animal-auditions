# 🎵 Song Matching System

This directory contains song assignments and karaoke track sources.

## 📋 Files

- **song-matches.json** - Complete database of all character-song pairings
- **matching-prompt.md** - ChatGPT prompt to match songs to characters
- **karaoke-sources.md** - Where to find legal karaoke tracks
- **song-library.md** - Master list of available songs by genre

## 🎯 Song Matching Criteria

Each song must:
- **Match character personality** (e.g., grumpy sloth → sad songs)
- **Create humor** through lyrics or context
- **Be recognizable** (well-known songs work best)
- **Have karaoke version available**
- **Fit 20-30 second format** (clear verse/chorus section)
- **Be family-friendly** (or easily edited)

## 📊 Song Assignment Schema

```json
{
  "character_id": "grumpy-sloth",
  "character_name": "Gary the Grumpy Sloth",
  "songs": [
    {
      "song_id": "creep-radiohead",
      "title": "Creep",
      "artist": "Radiohead",
      "genre": "Alternative Rock",
      "why_funny": "Sloth singing 'I'm a creep, I'm a weirdo' is perfectly on-brand",
      "key_lyrics": "I'm a creep, I'm a weirdo, what the hell am I doing here",
      "timestamp": "0:58-1:18 (20 seconds)",
      "karaoke_source": "YouTube - Sing King Karaoke",
      "mood": "melancholic",
      "difficulty": "medium"
    }
  ]
}
```

## 🎼 Genre Distribution

Aim for variety across all 36 videos (12 characters × 3 songs):

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

## ✅ Quality Checklist

Before approving song matches:

- [ ] Each song genuinely matches character personality
- [ ] Humor is clear and works visually
- [ ] No song is repeated across characters
- [ ] Mix of familiar and surprising choices
- [ ] Karaoke versions are available
- [ ] Lyrics are appropriate (or can be edited)
- [ ] 20-30 second sections are identifiable

## 🚀 Workflow

1. Generate character profiles first (`/characters`)
2. Use `matching-prompt.md` to assign 3 songs per character
3. Verify karaoke availability using `karaoke-sources.md`
4. Save to `song-matches.json`
5. **CHECKPOINT:** Review all 36 song choices
6. Move to video scene generation (`/scripts`)

---

**Next Step:** After song matching, proceed to 3-scene video generation