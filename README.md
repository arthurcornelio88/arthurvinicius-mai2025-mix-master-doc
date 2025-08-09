# 🎚️ Arthur Vinícius Live Studio - EP Mix & Master Presets — README

## Introduction
This is my first **LLM-guided mix & master project** as a professional musician and sound engineering enthusiast.

**The first challenge?** ✅ Done!
All tracks originally suffered from periodic buffer clicks. Using iZotope RX De-click, I restored every track — no more buffer artifacts.

With the instruments now clean, the mix and master process can be executed with precision and clarity.

This project marks my first experience working with preset chains for mixing and mastering. As a programmer, it feels natural — it’s just another form of structured, logical problem-solving. Let’s join talents and bring technical precision into musical creativity.

This repository contains the **preset chains**, **reference guides**, and **song-specific mix sheets** for the album.

---

## 1. Folder Structure
```

Album\_Mix\_Master/
│
├── presets/
│   └── ponta-cabeca/   # Mix presets for each track in Ponta-Cabeça
│
├── reference/          # Album-wide base workflow & mastering presets
│
├── songs/              # Song-specific mix & master sheets
│
└── README.md           # This document

```

---

## 2. Reference Documentation
- [**Album Mix & Master Reference**](reference/Album_Mix_Master_Reference.md)
  *(Base workflow for all songs, plugin inventory, mixing order, mastering approach)*

---

## 3. Song Mix Sheets
### Available
- [**Ponta-Cabeça**](songs/Ponta-Cabeca_Mix_Master_Sheet.md)

### Upcoming
- **Rio de Dores** *(TBD)*
- **Couleurs-Métro** *(TBD)*
- **Engenho Vermelho** *(TBD)*

Each song sheet contains:
- Track list and assigned presets
- Master bus configuration
- Special notes for the arrangement
- Automation and FX ideas

---

## 4. Presets
### **Ponta-Cabeça**
*(Located in `/presets/ponta-cabeca/`)*
- `PontaCabeca_VocalLead.rfxchain`
- `PontaCabeca_Snare.rfxchain`
- `PontaCabeca_Overheads.rfxchain`
- `PontaCabeca_Kick.rfxchain`
- `PontaCabeca_Guitar.rfxchain`
- `PontaCabeca_Bass.rfxchain`

### **Mastering Presets** *(Located in `/reference/`)*
- `Album_Master_Base_-14LUFS.rfxchain` — For streaming/YouTube
- `Album_Master_Base_-9LUFS.rfxchain` — For energetic/live

---

## 5. Technical Standard
- **Sample Rate:** 48 kHz
- **Bit Depth:** 24-bit
- **Loudness Targets:**
  - Streaming / YouTube: -14 LUFS, True Peak -1 dB
  - Energetic / Live: -9 LUFS, True Peak -1 dB
- **Peak Headroom During Mixing:** ~6 dB

---

## 6. Using the Presets

### Mixing
0. Place your FX Chain in `<User>/AppData/Roaming/REAPER/FXChains`
1. Open the track in Reaper.
2. Click **FX** → right-click inside FX chain window → **Add FX Chain...**
3. Load the preset matching the instrument track from the song sheet.

### Mastering
1. On the master bus, load either:
   - `Album_Master_Base_-14LUFS.rfxchain` for streaming/YouTube
   - `Album_Master_Base_-9LUFS.rfxchain` for energetic/live
2. Adjust thresholds in **LoudMax** to hit LUFS targets.
3. Check with **Youlean Loudness Meter** for compliance.

---

## 7. Notes
- All plugins used are **free** and already installed.
- Presets can be customized and saved for personal variations.
- For live or tracking, use lighter chains by disabling reverb/delay to save CPU.

---

*Created for the album including “Ponta-Cabeça” by Arthur Vinícius, Yannick Vela, Miguel Couto.*
```
