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

### 🎤 1. Vocal Lead

1. *RX 11 De-click* — Sens: `3.0`, Single-band
2. *bx\_cleansweep V2* — HPF @ `80 Hz`
3. *SPITFISH* — Sense: `5–6`, Tune `6–7 kHz`
4. *TDR Nova* — HPF `80 Hz`, Cut `250–400 Hz` `-2 to -4 dB`, Boost `12 kHz` `+1–2 dB`
5. *GlueReeds1* — Ratio `3:1`, Attack `25 ms`, Release `120 ms`, GR `~ -3 dB`
6. *OrilRiver* (send) — Pre-delay `20 ms`, Decay `1.2 s`, Wet `15–20%`
7. *Stereo Touch* (optional) — Width `40–50%`

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

1. *RX 11 De-click* — Sens: `2.0`
2. *bx\_cleansweep V2* — HPF @ `100 Hz`
3. *TDR Nova* — Cut `200–300 Hz` `-2–3 dB`, Boost `3–5 kHz` `+2–3 dB`
4. *FerricTDS* — Drive `+1.5 dB`
5. *Stereo Touch* — Width `50–60%`

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

* [ ] Kick & Snare locked in first
* [ ] Bass locked to kick (no masking at 60–120 Hz)
* [ ] Guitars balanced against bass midrange
* [ ] Vocals sit above instruments without harshness
* [ ] Overheads blended last for clarity
* [ ] Headroom maintained (\~6 dB before master)
* [ ] Final LUFS & TP compliance checked
