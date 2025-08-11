# Bounce 2 – Mix Notes (Revised Order)

## General Feedback
The first bounce has been reviewed, and here are the consolidated suggestions from the musicians for the second bounce.

---

## 1. Timing & Editing
- On the **third bass note** at the beginning of the song, it is slightly late — align it with the kick drum for tightness (even if it’s “cheating”).

---

## 2. Tonal & Dynamic Adjustments
### Kick Drum
- There were difficulties in achieving kick definition due to the original drum quality.
- Consider boosting **some higher frequencies** to make the **attack clearer** — test if it improves presence without making it harsh.
- EQ and Exciter

### Snare Drum
- Maybe try un **exciter** for space and dynamic differentiation.
- If not good, just config the compressor

### Bass
- The bass is lacking a bit of color — try adding an **amp simulator**
  You can use **Guitar Rig 7 – Bass Pro** for a Brazilian funk / slap style with occasional long notes, slightly aggressive but still warm.

  **Recommended Guitar Rig 7 configuration:**
  - **VC 76 Compressor (1176 style)**:
    - Attack: ~3 (fast but not too tight, keeps slap pop)
    - Release: ~7 (fast release for groove rebound)
    - Ratio: 4:1 or 8:1 (depending on desired control)
    - Input: Adjust for ~3–5 dB gain reduction during slap
    - Output: Balance to match project level
    - Dry: ~30% for parallel compression feel

  - **Graph EQ (inside Bass Pro)**:
    - 40 Hz: -2 dB (reduce unnecessary boom)
    - 90 Hz: +1 dB (low punch)
    - 180 Hz: 0 dB
    - 300 Hz: -1 dB (clean low-mids)
    - 500 Hz: 0 dB
    - 1 kHz: +2 dB (slap attack definition)
    - 2 kHz: +1 dB (clarity)
    - 4 kHz: 0 dB
    - 10 kHz: +2 dB (subtle brightness)

  - **Bass Pro Amp Section**:
    - Ultra Lo: OFF
    - Ultra Hi: ON
    - Gain: ~11 h
    - Bass: ~12 h
    - Mid: ~2 h
    - Mid Freq: ~800 Hz
    - Treble: ~1 h
    - Drive: ~9 h (slight grit)
    - Master: Adjust to mix

  - **Bass Pro Cabinet**:
    - Room: ~60% (adds space)
    - A/B Switch: B (more open)

  - **Solid EQ (post-amp)**:
    - Low Gain: Cut slightly if bass dominates
    - Mid Gain: Boost slightly at 1–2 kHz for more attack
    - High Gain: +1 dB max for clarity

- Lower the **bass volume slightly** in the mix after processing.


### Acoustic Guitar
- Use **Guitar Rig 7 – Jazz Amp** to enhance warmth, clarity, and presence while keeping a clean, dynamic tone.
- Recommended Jazz Amp settings:
  - Bright: ON
  - Bass: ~11 h (avoid excessive low end)
  - Mid: ~1 h (fills the mix, avoids scooped tone)
  - Treble: ~12 h (enough brightness without harshness)
  - Chorus: OFF for rhythm parts; ON with Rate ~10 h and Depth ~11 h for widened clean passages
  - Volume: adjust to match project gain staging
- Control Room Pro (cabinet/mic section):
  - Bass: ~11 h
  - Treble: ~1 h
  - Air: ~1 h (adds a touch of distance)
  - Experiment with SM57 + condenser blend for balanced attack and openness
- Stereo Tune:
  - Spread: ~20–25% (slight width without phase issues)
  - Drift: 0
  - Split: ~800 Hz (keeps low end mono)
  - Mix: ~50%
- Keep processing order: Amp → Control Room Pro → Stereo Tune (if stereo width desired) → EQ for final tonal shaping.
- Apply subtle EQ after the amp to remove unnecessary low rumble (<80 Hz) and slightly tame high frequencies (>8 kHz) if the tone is too bright.


---

## 3. Spatialization & Effects

### General Reverb

#### Guitar
- Use **RC 48** in *Random Hall* mode for depth and natural space.
- Recommended routing: place the RC 48 on a **dedicated reverb send bus** (100% wet), keep the guitar track dry for clarity.
- Suggested RC 48 settings for guitar:
  - Predelay: 20–25 ms (keeps the pick attack clear before reverb enters)
  - Diffusion: 60–70% (smooth reflections)
  - Spread: 100% (full stereo width)
  - Shape: 40–50% (balanced attack/sustain)
  - Size: 70–80% (large room feel)
  - Bass: -2 dB / X-Over: ~300 Hz (avoids low-end build-up)
  - Mid: 0 dB / Hi Cut: 7–8 kHz (natural top-end)
  - Damp: 30–40% (slightly mellows the highs)
- Adjust the send level for desired depth; use automation to increase reverb during special sections (e.g., instrumental break with shimmer).

#### Bass
- Apply reverb subtly to avoid muddying the low end — aim for ambience on the mids/highs only.
- Recommended: **RC 48** in *Reverb* mode, placed on a **separate reverb send bus** (100% wet).
- Suggested RC 48 settings for bass:
  - Predelay: ~15 ms (maintains note definition)
  - Diffusion: 40–50% (clearer reflections)
  - Spread: 80% (some stereo width without losing center punch)
  - Shape: ~40% (clear attack)
  - Size: 50–60% (moderate room)
  - Bass: -6 dB / X-Over: ~300–350 Hz (filters low end out of the reverb)
  - Mid: 0 to +1 dB (slight presence if needed)
  - Hi Cut: 6–7 kHz (avoids harshness)
  - Damp: 40–50% (natural decay)
- Follow the reverb with an EQ cutting all frequencies below ~200 Hz on the reverb return track.
- Keep the reverb send low (e.g., -15 to -12 dB) so it’s felt more than heard, adding subtle space without masking the groove.

#### Vocals
- Use a combination of **short plate reverb** (for presence) and **long hall reverb** (for depth), both on separate send buses.
- Plate reverb (short):
  - Decay: 0.8–1.2 s
  - Pre-delay: ~15 ms (keeps diction clear)
  - Hi Cut: ~9–10 kHz
  - Mix: 100% wet on send, adjust return level for subtle thickening
- Hall reverb (long):
  - Decay: 2–3 s
  - Pre-delay: 20–25 ms
  - Bass: -3 dB / X-Over: ~250 Hz (avoids low build-up)
  - Hi Cut: ~7–8 kHz
  - Mix: 100% wet on send, raise return for choruses or sustained notes

#### Overheads
- Use a **natural room or hall reverb** to enhance drum space without making cymbals harsh.
- Recommended: RC 48 or Raum in Hall mode
  - Decay: 1.5–2.2 s
  - Pre-delay: 5–10 ms
  - Bass: -2 to -4 dB / X-Over: ~300 Hz
  - Hi Cut: ~12 kHz (keeps cymbals smooth)
- Keep send levels low; the goal is to extend the natural ambience, not create a washed-out kit.



### Special Reverb (Instrumental Section)
- In the **instrumental section before the last part**, try adding a **shimmer reverb** (e.g., Valhalla Supermassive) to the guitar to clearly mark the contrast with the sung sections and make the guitar the central focus. This is experimental — only if it works musically.

---

## Final Checklist

* [X] Fix timing: align third bass note to kick.
* [X] Improve kick clarity with selective high-frequency boost.
* [X] Exciter in snare drum and kick
* [X] Add amp sim to bass for color and reduce its volume slightly.
* [X] Add amp sim to acoustic guitar for warmth, with light EQ.
* [X] Raise vocal volume slightly.
* [ ] Add subtle reverb to vocals, overheads, and guitar.
* [ ] Test shimmer reverb on the pre-final instrumental guitar section.
