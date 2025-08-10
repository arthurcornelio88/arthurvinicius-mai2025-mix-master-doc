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

Yes — we can refine this master chain so it works better in your context and also ensure it respects **broadcast/streaming loudness specs** while keeping your mix’s punch.

Here’s an updated, more precise version in **markdown**, optimized for your setup and tools:

---

## 🎛 Master Bus Chain

**1. Bus Compression — *Glue & Control***

* **Plugin**: ReaComp
* **Ratio**: `2:1`
* **Attack**: `30 ms` *(lets transients through)*
* **Release**: `100–150 ms` *(musical recovery)*
* **Gain Reduction**: `-1 to -2 dB` *(light, just for glue — not heavy compression)*
* **Tip**: Engage only when the mix feels slightly “disconnected,” otherwise skip.

---

**2. Global EQ — *Tonal Polish***

* **Plugin**: TDR Nova
* Use gentle, broad EQ moves only:

  * Low-shelf: `+0.5 to +1 dB @ 60–80 Hz` *(if low end feels thin)*
  * High-shelf: `+0.5 to +1 dB @ 12–14 kHz` *(adds air if mix is dull)*
  * Small cuts (`-1 to -2 dB`) in 200–400 Hz range if muddy.
* Avoid boosting more than `+1.5 dB` in any band at this stage.

---

**3. Saturation — *Glue & Harmonics***

* **Plugin**: FerricTDS
* **Drive**: `+0.5 to +1.0 dB` *(very subtle)*
* **Recovery**: Medium
* Purpose: Adds light harmonic content and “rounds” transients without audible distortion.

---

**4. Limiting — *Final Loudness & Safety***

* **Plugin**: LoudMax
* **Output Ceiling**: `-1.0 dB` (True Peak safe)
* **Threshold**: Adjust until target loudness is reached (`-14 LUFS` for streaming, `-9 to -8 LUFS` for louder pop/rock).
* Aim for no more than **3–4 dB of gain reduction** here.

---

**5. Loudness Check — *Final Verification***

* **Plugin**: Youlean Loudness Meter
* **Check**:

  * **Integrated LUFS** (overall loudness)
  * **Short-term LUFS** (avoid sudden overs)
  * **True Peak** (should stay below -1 dB)
* If your mix sounds squashed, **back off** the limiter threshold and revisit the bus compression.

---

💡 **Important**:
Mastering is *subtle* — the goal is **translation** across devices, not drastically changing your mix. If you find yourself EQ’ing heavily, go back to the mix stage and fix it there instead.

---

## 4. Genre-Specific Notes (Fast Brazilian Music)
- **Clarity first:** avoid overlapping frequency ranges between instruments
- **Transient shaping:** keep rhythmic elements distinct
- **Stereo placement:** pan to prevent masking
- **Dynamic range:** avoid over-compression to keep groove energy
