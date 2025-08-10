# 🎛️ Detailed Mixing & Plugin Guide — *Ponta-Cabeça*

This document combines the **step-by-step mixing order**, **instrument-specific plugin settings**, and **workflow notes** for *Ponta-Cabeça*.
It complements the **Mix & Master Sheet** and is designed for cases where `.rfxchain` files are not loaded, allowing manual setup in Reaper.

---

## 📋 Mixing Workflow Order

### Global Order

1. **Drums**
2. **Bass**
3. **Guitars / Harmonic Instruments**
4. **Vocals**
5. **Additional Elements / FX**
6. **Automation & Finishing Touches**

---

### 🥁 Drum Internal Order

Work from **center & low frequencies** toward **highs & stereo**:

1. **Kick** — foundation, low-end punch
2. **Snare** — rhythmic articulation, body
3. **Overheads** — stereo image & cymbals

💡 **For Ponta-Cabeça:**

* Add **Overheads last** to avoid masking in fast rhythms.
* After drums, lock in **bass** for groove foundation before guitars & vocals.
* Always **A/B kick vs bass in solo** to avoid masking between 60–120 Hz.

---

## 🔧 Track-by-Track Plugin & Parameter Guide

Here’s your vocal chain written exactly in that style:

---

### 🎤 1. Vocal Lead

**iZotope RX 11 De-click**

* **Sensitivity:** `3.0`
* **Mode:** Single-band
* Removes mouth clicks and small transient artifacts before any tone shaping.

**bx\_cleansweep V2**

* **HPF:** `80 Hz` (removes low rumble and plosives)
* **LPF:** leave open unless there’s harshness above 15 kHz.

**SPITFISH De-Esser** *(placed before EQ)*

* **Sense:** `5–6` (moderate detection)
* **Tune:** `6–7 kHz` (targets sibilance range)
* **Depth:** adjust to taste — aim for smooth “S” control without dullness
* Placing before EQ ensures raw sibilance is tamed before boosts/compression.

**Graillon 2/3 Free — Vocal Pitch Correction Setup (Subtle Mode)**

* **Key Selector**: Set to your song key (turn off unused notes by clicking them) — this makes correction faster and more natural.
* **Correction Amount**: `30–50%` → keeps pitch stable but avoids robotic tone.
* **Smooth**: `5.0–10 ms` → softens pitch transitions so it doesn’t “jump.”
* **Inertia**: `20–30%` → helps keep long notes stable without over-snapping.
* **Snap Min**: `0.00 st`
* **Snap Max**: `8.00 st` (default, keeps wide range if note is off)
* **Formants**: `100%` (preserves natural vocal timbre — no chipmunk effect).
* **Pitch Shift**: Leave at `0.00 st` (don’t use for correction — only for creative shifts).
* **Wet/Dry**: Wet at `0 dB` and Dry at `-inf dB` → fully corrected signal only.
* **Gain**: Adjust so Graillon’s output matches bypass level (watch meters).

**TDR Nova (EQ shaping)**

* **HPF:** `80 Hz` (gentle slope)
* **Cut 250–400 Hz:** `-2 to -4 dB` (reduces muddiness)
* **Boost 12 kHz:** `+1–2 dB` (adds air and clarity)

**ReaComp (Compression)**

* **Threshold:** set so peaks get around `-3 dB` gain reduction
* **Ratio:** `3:1`
* **Attack:** `25 ms` (lets initial consonants through)
* **Release:** `120 ms` (smooth recovery)
* **Knee:** `2 dB` (soft knee for natural onset)
* **Output Gain:** adjust so volume matches pre-compression loudness

**OrilRiver (Reverb Send)**

* **Pre-delay:** `20 ms` (keeps vocal upfront)
* **Decay:** `1.2 s` (medium space)
* **Wet:** `15–20%` (subtle ambience, avoid washing out)

**Stereo Touch** *(Optional – Vocal Width Enhancement)*

* **Delay 1**: `8–10 ms` *(shorter than guitar to keep vocal more centered)*
* **Delay 1 Gain**: `-6 dB`
* **Delay 2**: `14–16 ms`
* **Delay 2 Gain**: `-6 dB`
* **HPF Enable**: On — HPF at `120 Hz` *(keeps low-end mono for clarity)*
* **LPF Enable**: On — LPF at `12–14 kHz` *(prevents excessive air spreading)*
* **Out Gain**: Adjust so output matches bypass level *(≈ -6 dB)*
* **Result**: Adds gentle stereo width (\~40–50%) to vocals while preserving a strong mono image for clarity and avoiding phase issues in the mix.

---

### 🥁 2. Kick

1. **iZotope RX 11 De-click**

   * Sensitivity: `2.0`

2. **bx\_cleansweep V2**

   * **HPF**: `20 Hz` (remove unnecessary sub-bass)
   * **LPF**: `8 kHz` (remove unwanted highs and leave space for cymbals)
   * Input Gain: `0 dB` (adjust if needed)

3. **TDR Nova** (EQ)

   * Boost `60–80 Hz`: `+3 to +4 dB` (kick fundamental)
   * Cut `250 Hz`: `-2 to -3 dB` (reduce muddiness)
   * Optional: Boost `3–4 kHz` `+2–3 dB` for more click/presence

4. **ReaComp** (compression)

   * Threshold: Adjust until strong hits cause **-4 to -5 dB** gain reduction
   * Ratio: `4:1`
   * Attack: `15 ms` (keeps initial punch)
   * Release: `100 ms`
   * Knee: `0.0 dB` (sharp compression)
   * RMS size: `5 ms`
   * Auto release: Off
   * Output gain: Adjust to match pre-compression loudness

---

### 🥁 3. Snare (Brush Hits)

1. **iZotope RX 11 De-click**
   - Sensitivity: `2.0`
   - Removes digital clicks and minor transient artifacts.

2. **bx_cleansweep V2**
   - HPF: `120 Hz` — remove sub rumble without thinning body
   - LPF: leave open, or set to `~12 kHz` if cymbal bleed is harsh
   - Input Gain: `0 dB`

3. **TDR Nova**
   - Boost `200 Hz`: `+2 to +3 dB` — adds warmth and body to brush texture
   - Cut `250–350 Hz`: `-2 dB` — reduces shell muddiness
   - Boost `4–6 kHz`: `+3 to +4 dB` — enhances brush swipe definition
   - *(Optional)* Boost `10–12 kHz` gently for extra air if needed

4. **Transpire** *(Transient Shaper)*
   - Attack: `+20 to +25%` — adds articulation without making it too “stick-like”
   - Sustain: `-10%` — reduces excess ring and room bleed

5. **FerricTDS**
   - Drive: `+1.5 to +2.0 dB`
   - Recovery: Medium-slow — preserves natural decay
   - Adds tape-like warmth and cohesion

6. **(Optional) ReaComp — Peak Control**
   - Threshold: Adjust so peaks trigger `~2–3 dB` gain reduction
   - Ratio: `3:1`
   - Attack: `10 ms` — catches peaks without killing transients
   - Release: `80–100 ms`
   - Knee: `2 dB` — soft knee for smooth onset
   - Output Gain: Match pre-compression loudness

---

### 🥁 4. Overheads (Stereo Pair)

1. **iZotope RX 11 De-click**

   * Sensitivity: `1.5`

2. **bx\_cleansweep V2**

   * HPF: `250 Hz` (remove low rumble and bleed)

3. **TDR Nova**

   * Cut `4–5 kHz`: `-2 dB` if harsh
   * Boost `12–14 kHz`: `+2 dB` for shimmer (optional)

4. **FerricTDS**

   * Drive: `+1.0 dB`

---

#### 🎧 Simple Stereo Tip

* Pan one overhead hard left (`100% L`) and the other hard right (`100% R`).
* If it feels too wide, bring each in a bit (e.g., `80% L` / `80% R`).
* Don’t touch phase or delay — just pan and listen.

---

### 🎸 5. Bass (Funky, Articulated — Slaps + Mixed Note Lengths)

1. **iZotope RX 11 De-click**

   * Sensitivity: `1.5`
   * Cleans up string noise, click artifacts, and slap transients.

2. **bx\_cleansweep V2**

   * LPF: `5–6 kHz` (remove unnecessary highs while keeping slap clarity)

3. **TDR Nova**

   * Boost `60–80 Hz`: `+3 dB` (solid low-end presence)
   * Cut `200–300 Hz`: `-2 dB` (reduce mud)
   * Optional: gentle boost `1–2 kHz` for finger and slap definition

4. **ReaComp** *(Main Compression & Peak Control)*

   * Threshold: set so normal notes trigger \~2–3 dB reduction, and slaps go a bit higher
   * Ratio: `3:1`
   * Attack: `5–10 ms` (lets slap attack through)
   * Release: `80–100 ms` (returns to zero between notes)
   * Knee: `2 dB` (smooth onset)
   * Output Gain: adjust to match pre-compression loudness

---

#### 🎯 Low-End Gain Balance — Kick + Bass “Lock”

The goal: keep the **kick and bass working together** without masking each other in the 60–120 Hz range.

1. **Set Kick First**

   * Solo the kick.
   * Adjust fader so **peak is around -6 dBFS** during the loudest hits.
   * Ensure it has enough punch without triggering the master above -6 dBFS.

2. **Bring in the Bass**

   * Solo **kick + bass** together.
   * Start with bass fader all the way down, then slowly bring it up until:

     * Low-end feels full and solid.
     * Kick still cuts clearly through.

3. **A/B Check**

   * **Mute bass** → listen to kick clarity.
   * **Mute kick** → listen to bass body.
   * Together, they should **complement** each other — not sound like one muddy blob.

4. **EQ Carving**

   * Kick: emphasize **60–80 Hz**, reduce **250 Hz** (mud).
   * Bass: keep **60–80 Hz** full but cut slightly where kick is strongest, boost **1–2 kHz** for note definition.

5. **Mono Compatibility**

   * Check in mono — low-end should stay stable and not disappear.

6. **Final Peak Targets**

   * Kick: peaks around **-6 dBFS**
   * Bass: peaks around **-8 dBFS** when soloed, but **combined low-end peaks** should still leave \~6 dB headroom on the master bus.

---

### 🎸 6. Guitar

1. **iZotope RX 11 De-click**

   * Sensitivity: `2.0`
   * Removes handling noise and small digital clicks.

2. **bx\_cleansweep V2**

   * HPF: `100 Hz` (removes unnecessary low-end rumble)
   * LPF: leave open, or roll off gently at `12–14 kHz` if there’s harsh pick noise.

3. **TDR Nova**

   * Cut `200–300 Hz`: `-2 to -3 dB` (reduces muddiness)
   * Boost `3–5 kHz`: `+2 to +3 dB` (adds presence for rhythmic definition)
   * Optional: small lift at `8–10 kHz` for extra shimmer if arrangement allows.

4. **FerricTDS**

   * Drive: `+1.5 dB` for warmth and cohesion.
   * Recovery: medium to preserve natural sustain.

5. **Stereo Touch** *(Optional – Guitar Stereo Enhancement)*

   - **Delay 1:** `12–15 ms`
   - **Delay 1 Gain:** `-6 dB`
   - **Delay 2:** `18–20 ms`
   - **Delay 2 Gain:** `-6 dB`
   - **HPF Enable:** `On` — HPF at `120 Hz` (keeps low-end mono)
   - **LPF Enable:** `Off` — preserves high-end sparkle
   - **Out Gain:** Adjust so output matches bypass level (≈ `-6 dB`)

   **Result:** Creates a balanced `50–60%` stereo width without introducing phase problems, keeping the guitar spacious but controlled in the mix.

### 🎸 6. Reverb *(optional — send, not insert)*

- **Plugin:** OrilRiver *(Small Room or Plate)*
- **Routing:**
  - Guitar track → Send to *Reverb Bus*
  - On *Reverb Bus*: **Dry = -inf**, **Wet = ~-12 dB**
  - Raise *Reverb Bus* fader to taste (`-18 dB` starting point)
- **Settings:**
  - Pre-delay: `10–15 ms` *(keeps attack clean)*
  - Decay: `0.8–1.2 s` *(short enough for faster tracks)*
  - Width: `100%`
- **Blend:**
  - Use the **send gain** from the Guitar track to control reverb amount
  - Keep subtle — just enough to remove dryness without washing out the part

---

## 🎚️ Master Bus — Album Reference

1. **FerricTDS** — Drive `+1.0 dB`
2. **TDR Nova** — Gentle tonal balance adjustments (±2 dB max)
3. **LoudMax** — Output `-1 dBTP`, Threshold for LUFS target:

   * Streaming/YouTube: `-14 LUFS`
   * Live/Energetic: `-9 LUFS`
4. **Youlean Loudness Meter** — Final loudness verification

---

## ✅ Mix Checklist

* [X] Kick & Snare locked in first
* [X] Bass locked to kick (no masking at 60–120 Hz)
* [ ] Guitars balanced against bass midrange
* [ ] Vocals sit above instruments without harshness
* [ ] Overheads blended last for clarity
* [ ] Headroom maintained (\~6 dB before master)
* [ ] Final LUFS & TP compliance checked
