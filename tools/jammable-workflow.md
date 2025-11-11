# 🎤 Jammable.ai Workflow Guide

Complete guide for creating AI singing voices with Jammable.

---

## 🎯 What Jammable Does

Converts karaoke tracks into AI singing voices with character-specific vocal styles.

**Input:** Karaoke track (instrumental)
**Output:** AI-generated singing voice

---

## 📋 Setup (One-Time)

### Step 1: Create Account

1. Go to [Jammable.ai](https://www.jammable.ai)
2. Sign up (free tier available)
3. Explore voice library

### Step 2: Understand Voice Models

**Community Voices:** Pre-made voices you can use
**Custom Voices:** Create your own (requires voice samples)

**For this project:** Use community voices that match character personalities

---

## 🎵 Production Workflow (Per Song)

### Step 1: Prepare Karaoke Track

**Before uploading to Jammable:**

1. Find karaoke version on YouTube
2. Download audio (use youtube-dl or online converter)
3. Trim to 20-30 second section using:
   - Online tool (e.g., mp3cut.net)
   - Audacity (free software)
   - Or upload full track and note timestamp

**File format:** MP3 or WAV
**Quality:** At least 128kbps

---

### Step 2: Select Voice Model

**Match voice to character personality:**

| Character Type | Voice Style | Jammable Search Terms |
|----------------|-------------|----------------------|
| Grumpy Sloth | Deep, monotone, slow | "deep male", "monotone", "alternative" |
| Vain Zebra | Smooth, confident | "smooth male", "pop", "confident" |
| Anxious Meerkat | High-pitched, fast | "high male", "nervous", "energetic" |
| Dramatic Flamingo | Theatrical, over-top | "theatrical", "broadway", "dramatic" |

**Tips:**
- Test 2-3 voices per character
- Listen to voice samples before committing
- Save voice IDs for consistency

---

### Step 3: Generate AI Cover

1. **Upload karaoke track** to Jammable
2. **Select voice model** from library
3. **Adjust settings** (if available):
   - Pitch adjustment
   - Vocal strength
   - Effects
4. **Generate** (takes 2-5 minutes)
5. **Preview** result

---

### Step 4: Quality Check

**Listen for:**
- [ ] Singing sounds natural (not robotic)
- [ ] Pitch is correct (not off-key)
- [ ] Voice matches character personality
- [ ] Audio quality is clean (no artifacts)
- [ ] Timing matches karaoke track

**If quality is poor:**
- Try different voice model
- Adjust settings
- Use different karaoke track (better quality)

---

### Step 5: Download & Organize

1. **Download** final audio file
2. **Rename** with clear naming:
   - Format: `[character-id]_[song-id].mp3`
   - Example: `grumpy-sloth_creep-radiohead.mp3`
3. **Save** to `assets/audio/singing/`

---

## 🎨 Voice Selection Guide

### Character-to-Voice Mapping

**Create a voice reference doc:**

```json
{
  "grumpy-sloth": {
    "jammable_voice_id": "voice_12345",
    "voice_name": "Deep Monotone Male",
    "notes": "Perfect for alternative/grunge songs"
  },
  "vain-zebra": {
    "jammable_voice_id": "voice_67890",
    "voice_name": "Smooth Pop Male",
    "notes": "Works great for 80s pop and disco"
  }
}
```

**Save this** to maintain consistency across all songs for each character.

---

## ⚡ Batch Production Tips

**For 36 songs:**

1. **Group by character** (do all 3 songs for one character at once)
2. **Keep voice model selected** (don't switch between each song)
3. **Queue multiple generations** (if Jammable allows)
4. **Download in batches** (organize as you go)

**Time estimate:** 3-5 minutes per song = 3-5 hours total

---

## 🚨 Common Issues & Solutions

### Issue: Voice sounds robotic

**Solutions:**
- Try different voice model
- Use higher quality karaoke track
- Adjust pitch settings
- Check if song is too complex for AI

### Issue: Pitch is off-key

**Solutions:**
- Verify karaoke track is in correct key
- Adjust pitch settings in Jammable
- Try different voice model
- Use different karaoke source

### Issue: Audio quality is poor

**Solutions:**
- Upload higher quality karaoke track
- Check Jammable export settings
- Try re-generating
- Contact Jammable support

### Issue: Voice doesn't match character

**Solutions:**
- Browse more voice options
- Create custom voice (if needed)
- Adjust character description to match available voices

---

## 💡 Pro Tips

1. **Test voices early:** Generate 3 test songs before committing to full batch
2. **Save favorites:** Bookmark voice models that work well
3. **Consistent naming:** Use clear file naming from the start
4. **Quality over speed:** Don't rush - bad audio ruins final video
5. **Backup files:** Keep copies of all generated audio

---

## 🔄 Alternative Tools

If Jammable doesn't work:

**Plan B: Kits.AI**
- Similar functionality
- Has API (for automation)
- ~$10-30/month

**Plan C: Synthesizer V**
- More control
- Steeper learning curve
- One-time purchase

---

## ✅ Checklist Per Song

- [ ] Karaoke track prepared (20-30 seconds)
- [ ] Voice model selected (matches character)
- [ ] AI cover generated
- [ ] Quality check passed
- [ ] File downloaded and renamed
- [ ] Saved to correct folder

---

**Next Step:** Use generated audio in Hedra for lip-sync (`hedra-workflow.md`)