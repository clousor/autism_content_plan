# Gappu & Dolly — Industrial AI Animation Production Pipeline

**Document ID:** `GD-PIPE-01`  
**Standard:** 12-Step Deterministic Production Lifecycle & Multi-Tier AI Technology Stacks  
**Objective:** Manufacture visually identical, emotionally compelling 9:16 animated video assets with zero character degradation.  

---

## 1. Dual AI Technology Stacks

```
┌─────────────────────────────────────────────────────────────────────────────────┐
│                      DUAL PRODUCTION TECHNOLOGY STACKS                          │
├────────────────────┬─────────────────────────────┬──────────────────────────────┤
│ PIPELINE LAYER     │ 💎 PRIMARY STUDIO STACK     │ ⚡ FAST / LOW-COST STACK      │
│                    │ (Flagship Films & Pilots)   │ (Weekly High-Volume Reels)   │
├────────────────────┼─────────────────────────────┼──────────────────────────────┤
│ 1. Character Lock  │ Flux.1-Dev trained LoRA +   │ Midjourney v6.1 with `--cref`│
│    & Keyframing    │ ComfyUI IP-Adapter Pro      │ and `--cw 85` consistency    │
├────────────────────┼─────────────────────────────┼──────────────────────────────┤
│ 2. Video Animation │ Kling 1.5 Pro (Camera lock) │ Hailuo MiniMax (Video-01) /  │
│    & Motion Engine │ & Runway Gen-3 Alpha        │ Luma Dream Machine           │
├────────────────────┼─────────────────────────────┼──────────────────────────────┤
│ 3. Facial Lip-Sync │ LivePortrait (Precise trunk/│ Hedra Character-2 /          │
│    & Performance   │ mouth mesh mapping)         │ SyncLabs API                 │
├────────────────────┼─────────────────────────────┼──────────────────────────────┤
│ 4. Voiceover & SFX │ ElevenLabs Neural Custom    │ ElevenLabs Standard Voices   │
│                    │ Voices (Commercial Rights)  │ + Epidemic Sound Library     │
├────────────────────┼─────────────────────────────┼──────────────────────────────┤
│ 5. Compositing &   │ DaVinci Resolve Studio      │ CapCut Desktop (Template     │
│    Post-Production │ (Fusion vector logo overlay)│ overlays, Auto-Captions)     │
└────────────────────┴─────────────────────────────┴──────────────────────────────┘
```

---

## 2. The 12-Step Master Production Lifecycle

Every Gappu & Dolly Reel moves through an unalterable **12-Step Production Pipeline**:

```
[STEP 1: SCRIPT & CLINICAL LOCK]
  │ (Script selected from 07_TOP_30_GAPPU_DOLLY_SCRIPTS.md + Clinical Review clearance)
  ▼
[STEP 2: STORYBOARD AUDIO DRAFT]
  │ (Rough scratch audio generated via ElevenLabs to lock precise timing per scene)
  ▼
[STEP 3: KEYFRAME GENERATION]
  │ (Generate 5 scene start-frames using Master Image Prompts + Master Reference Pack)
  ▼
[STEP 4: SEED & ANATOMY INSPECTION]
  │ (QA Check: Ears, trunk, dolphin colors, fingers. Discard any anatomical anomalies)
  ▼
[STEP 5: IMAGE-TO-VIDEO MOTION ANIMATION]
  │ (Input approved keyframe into Kling 1.5 / Runway Gen-3; execute camera & motion prompts)
  ▼
[STEP 6: LIP-SYNC & FACIAL RETARGETING]
  │ (Run LivePortrait / Hedra on dialogue close-ups to align mouth movement with Hindi/Hinglish VO)
  ▼
[STEP 7: ASSEMBLY & VIDEO EDITING]
  │ (Import 5 scene video clips into NLE timeline at 1080x1920 9:16 vertical resolution)
  ▼
[STEP 8: AUDIO MASTERING & SOUND DESIGN]
  │ (Layer voiceover, ambient classroom/park audio, musical score, and signature character SFX)
  ▼
[STEP 9: VECTOR LOGO & GRAPHICS COMPOSITING]
  │ (Superimpose clean vector Autism Alliance logo and lower-third graphic banners in post)
  ▼
[STEP 10: DUAL-LANGUAGE SUBTITLE BURN-IN]
  │ (Animate clean bold subtitles within the 9:16 social safe zones: 250px top, 350px bottom)
  ▼
[STEP 11: QUALITY GATE & CLINICAL SIGN-OFF]
  │ (Audit against 20-point Quality Gate checklist; verify clinical compliance)
  ▼
[STEP 12: EXPORT, PLATFORM PACKAGING & ARCHIVING]
  │ (Export ProRes master + H.264 social clips; archive seeds, prompts, and project `.drp` files)
```

---

## 3. Tool-Specific Operational Presets

### A. Midjourney v6.1 Consistency Settings
*   Command syntax: `[Master Character Lock String] + [Environment Details] + [Camera] --cref [URL_OF_OFFICIAL_MASCOT_REFERENCE] --cw 85 --ar 9:16 --v 6.1 --style raw --s 150`
*   *Why `--cw 85`:* Keeps the exact face, ear shape, trunk curves, and dolphin dorsal lines 100% locked, while allowing `--cw` variance to alter Gappu's sitting vs standing posture naturally.

### B. Kling 1.5 Image-to-Video Presets
*   Mode: **Professional Mode** (1080p, 30fps).
*   Motion Brush Configuration:
    *   Brush 1 (Gappu's Trunk): Set gentle vertical upward velocity (`+1.5`), zero horizontal drift.
    *   Brush 2 (Dolly's Body): Set gentle forward arc velocity (`+2.0`, vertical `+0.8`) to simulate buoyant swimming.
    *   Background: Set static or subtle ambient parallax (`camera pan right, 0.5`).

### C. LivePortrait Facial & Lip-Sync Presets
*   Driving Video / Audio: High-clarity `.wav` vocal track.
*   Retargeting Parameter: Set `eyebrow_sensitivity: 0.85` (enhances gentle curiosity), `mouth_open_ratio: 0.75` (prevents gaping clown-like expressions).
