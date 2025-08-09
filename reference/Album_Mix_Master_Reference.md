# 🎚️ Album Mix & Master Reference (48 kHz / 24-bit)

## 1. Technical Standards
- **Sample Rate:** 48 kHz
- **Bit Depth:** 24-bit
- **Peak Headroom (mixing):** Leave ~6 dB before mastering
- **Loudness Targets:**
  - Streaming/YouTube: -14 LUFS, True Peak -1 dB
  - Energetic/Live: -9 LUFS, True Peak -1 dB

---

## 2. Plugin Inventory
| Plugin | Type | Primary Use |
|--------|------|-------------|
| **TDR Nova** | Dynamic/parametric EQ | Corrective EQ, tonal shaping |
| **bx_cleansweep** | HP/LP filter | Remove unnecessary lows/highs |
| **GlueReeds1** | Bus/track compressor | Transparent compression |
| **CamelCrusher** | Saturation + compression | Warmth, coloration |
| **OldSkoolVerb** | Algorithmic reverb | Plates, rooms, halls |
| **OrilRiver** | Realistic reverb | Natural space and depth |
| **StereoTouch** | Stereo widening | Expanding stereo image |
| **LoudMax** | Limiter | Final mastering volume control |
| **FerricTDS** | Tape saturation | Cohesion, warmth |
| **Spitfish** | De-esser | Reduce vocal sibilance |
| **Sonic Anomaly Transpire** | Transient shaper | Increase or soften attack |
| **Youlean Loudness Meter** | Loudness metering | LUFS/True Peak measurement |
| **Anspec** | Spectrum analyzer | Identify problem frequencies |

---

## 3. Global Mixing Workflow

### Per Track
1. **Cleanup**
   - RX (if needed) → remove clicks, hiss
   - bx_cleansweep → remove unused low/high frequencies
2. **Corrective EQ**
   - TDR Nova → remove muddiness or harshness
3. **Compression**
   - GlueReeds1 → control dynamics
   - CamelCrusher (optional) → add warmth
4. **Additive EQ**
   - TDR Nova → enhance musical ranges
5. **Transient Control**
   - Transpire → emphasize attack for rhythmic clarity
6. **Effects**
   - Reverb (OldSkoolVerb/OrilRiver) via send
   - Delay/modulation sparingly
7. **Panning & Leveling**
   - Ensure each part has its own stereo space

### Master Bus
1. **Bus Compression**
   - GlueReeds1: light 2:1 ratio, slow attack, -1 to -2 dB gain reduction
2. **Global EQ**
   - TDR Nova: gentle tonal adjustments
3. **Saturation**
   - FerricTDS: subtle glue for cohesion
4. **Limiter**
   - LoudMax: Output ceiling -1 dB, adjust for LUFS target
5. **Loudness Check**
   - Youlean Loudness Meter: verify LUFS & True Peak

---

## 4. Genre-Specific Notes (Fast Brazilian Music)
- **Clarity first:** avoid overlapping frequency ranges between instruments
- **Transient shaping:** keep rhythmic elements distinct
- **Stereo placement:** pan to prevent masking
- **Dynamic range:** avoid over-compression to keep groove energy
