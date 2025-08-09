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

   * **HPF:** `20 Hz` (remove unnecessary sub-bass)
   * **LPF:** `8 kHz` (remove unwanted highs and leave space for cymbals)
   * Input Gain: `0 dB` (adjust if needed)

3. **TDR Nova**

   * **HPF:** 20 Hz, 24 dB/oct (clean subsonic rumble)
   * **Band 1:** 70 Hz, Q `1.0`, Gain `+3.5 dB` (boost low-end punch)
   * **Band 2:** 250 Hz, Q `1.2`, Gain `-3.0 dB` (reduce muddiness)
   * **Band 3:** 3.5 kHz, Q `1.0`, Gain `+2.5 dB` *(optional for click/presence)*
   * **LPF:** 8 kHz, 24 dB/oct (focus energy in kick range)
   * *(Optional dynamics)* Threshold `-20 dB`, Ratio `2:1`, Attack `20 ms`, Release `200 ms` if low end is inconsistent

4. **GlueReeds1** (compression)

   * Ratio: `4:1`
   * Attack: `15 ms`
   * Release: `100 ms`
   * Gain Reduction: `-4 to -5 dB`

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
