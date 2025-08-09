# 🎛️ Detailed Plugin & Parameter Guide — "Ponta-Cabeça"

This guide details **exact plugin order and settings** for each track in *Ponta-Cabeça*.
It complements the **Mix & Master Sheet** and should be used when manually inserting plugins into Reaper if `.rfxchain` files are not loaded.

---

## 🎤 1. Vocal Lead

1. **iZotope RX 11 De-click**
   - Algorithm: *Single-band*
   - Sensitivity: `3.0`
   - Click widening: `0 ms`

2. **bx_cleansweep V2**
   - HPF: `80 Hz`

3. **SPITFISH** (de-esser)
   - Sense: `5–6` (reduce sibilance without dullness)
   - Tune to match sibilant frequency (~6–7 kHz)

4. **TDR Nova** (EQ)
   - HPF @ 80 Hz
   - Cut 250–400 Hz: `-2 to -4 dB` (mud control)
   - Cut 3 kHz: `-2 dB` (if harsh)
   - Boost 12 kHz: `+1–2 dB` (air)

5. **GlueReeds1** (compression)
   - Ratio: `3:1`
   - Attack: `25 ms`
   - Release: `120 ms`
   - GR: `~ -3 dB`

6. **OrilRiver** (plate reverb, via send)
   - Pre-delay: `20 ms`
   - Decay: `1.2 s`
   - Wet: `15–20%`

7. **Stereo Touch** (optional)
   - Width: `40–50%`

---

## 🥁 2. Snare

1. **RX 11 De-click** — Sensitivity `2.0`
2. **bx_cleansweep V2** — HPF @ 120 Hz
3. **TDR Nova**
   - Boost 200 Hz: `+2–3 dB` (body)
   - Cut 250–350 Hz: `-2 dB`
   - Boost 4–6 kHz: `+3–4 dB` (crack)
4. **Transpire** (transient shaper)
   - Attack: `+25%`
   - Sustain: `-10%`
5. **FerricTDS** — Drive: `+1.5–2.0 dB`

---

## 🥁 3. Kick

1. **RX 11 De-click** — Sensitivity `2.0`
2. **bx_cleansweep V2** — LPF @ 8 kHz
3. **TDR Nova**
   - Boost 60–80 Hz: `+3–4 dB`
   - Cut 250 Hz: `-2–3 dB`
   - Optional boost 3–4 kHz for click
4. **GlueReeds1**
   - Ratio: `4:1`
   - Attack: `15 ms`
   - Release: `100 ms`
   - GR: `-4 to -5 dB`

---

## 🥁 4. Overheads

1. **RX 11 De-click** — Sensitivity `1.5`
2. **bx_cleansweep V2** — HPF @ 250 Hz
3. **TDR Nova**
   - Cut 4–5 kHz: `-2 dB` if harsh
   - Optional boost 12–14 kHz: `+2 dB` (air)
4. **FerricTDS** — Drive: `+1.0 dB`

---

## 🎸 5. Guitar

1. **RX 11 De-click** — Sensitivity `2.0`
2. **bx_cleansweep V2** — HPF @ 100 Hz
3. **TDR Nova**
   - Cut 200–300 Hz: `-2–3 dB`
   - Boost 3–5 kHz: `+2–3 dB`
4. **FerricTDS** — Drive: `+1.5 dB`
5. **Stereo Touch** — Width: `50–60%`

---

## 🎸 6. Bass

1. **RX 11 De-click** — Sensitivity `1.5`
2. **bx_cleansweep V2** — LPF @ 5–6 kHz
3. **TDR Nova**
   - Boost 60–80 Hz: `+3 dB`
   - Cut 200–300 Hz: `-2 dB`
4. **GlueReeds1**
   - Ratio: `4:1`
   - Attack: `10–15 ms`
   - Release: `100–120 ms`
   - GR: `~ -4 dB`

---

## 🎚️ Master Bus (Album Reference)

1. **FerricTDS** — Drive: `+1.0 dB`
2. **TDR Nova** — Gentle tonal balance (±2 dB max)
3. **LoudMax**
   - Output: `-1 dBTP`
   - Threshold: adjust to LUFS target:
     - Streaming: `-14 LUFS`
     - Live/Energetic: `-9 LUFS`
4. **Youlean Loudness Meter** — Check loudness compliance

---

**Tip:** Apply reverbs/delays via send tracks, keep stereo widening subtle, and ensure phase coherence when summing to mono.
