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

### 🥁 3. Snare

1. *RX 11 De-click* — Sens: `2.0`
2. *bx\_cleansweep V2* — HPF @ `120 Hz`
3. *TDR Nova* — Boost `200 Hz` `+2–3 dB`, Cut `250–350 Hz` `-2 dB`, Boost `4–6 kHz` `+3–4 dB`
4. *Transpire* — Attack `+25%`, Sustain `-10%`
5. *FerricTDS* — Drive `+1.5–2.0 dB`

---

### 🥁 4. Overheads

1. *RX 11 De-click* — Sens: `1.5`
2. *bx\_cleansweep V2* — HPF @ `250 Hz`
3. *TDR Nova* — Cut `4–5 kHz` `-2 dB` (if harsh), opt. Boost `12–14 kHz` `+2 dB`
4. *FerricTDS* — Drive `+1.0 dB`

---

### 🎸 5. Bass

1. *RX 11 De-click* — Sens: `1.5`
2. *bx\_cleansweep V2* — LPF @ `5–6 kHz`
3. *TDR Nova* — Boost `60–80 Hz` `+3 dB`, Cut `200–300 Hz` `-2 dB`
4. *GlueReeds1* — Ratio `4:1`, Attack `10–15 ms`, Release `100–120 ms`, GR `~ -4 dB`

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
