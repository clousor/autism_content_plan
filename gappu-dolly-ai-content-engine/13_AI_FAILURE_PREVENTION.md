# Gappu & Dolly — AI Failure Mode Prevention & Negative Constraint Suite

**Document ID:** `GD-FAIL-01`  
**Purpose:** Forensic Identification & Elimination of Generative AI Artifacts, Morphing & Anatomical Drift  
**Quality Benchmark:** Zero-Tolerance for Uncanny Valley, Creepy Facial Features & Distorted Anatomy  

---

## 1. Top 10 Generative AI Failure Modes & Countermeasures

```
┌─────────────────────────────────────────────────────────────────────────────────┐
│                    THE 10 CRITICAL FAILURE MODES & FIXES                        │
├────┬─────────────────────────────┬──────────────────────────────────────────────┤
│ #  │ FAILURE MODE (AI GLITCH)    │ MANDATORY PROTOCOL & REMEDIATION             │
├────┼─────────────────────────────┼──────────────────────────────────────────────┤
│ 1  │ Extra Limbs / Human Fingers │ Ban human hand prompts. Specify: "rounded    │
│    │ on Gappu                    │ four-toed elephant paws with soft pads".     │
├────┼─────────────────────────────┼──────────────────────────────────────────────┤
│ 2  │ Trunk Morphing / Limp Hose  │ Lock S-curve prompt; enforce length ratio    │
│    │                             │ (max 1.2x cranial height).                   │
├────┼─────────────────────────────┼──────────────────────────────────────────────┤
│ 3  │ Dolphin Anatomy Distortion  │ Negative prompt: "scales, gills, shark teeth,│
│    │ (Fish scales, sharp teeth)  │ vertical fish tail, human arms".             │
├────┼─────────────────────────────┼──────────────────────────────────────────────┤
│ 4  │ AI-Generated Gibberish Text │ **STRICT BAN:** Never prompt text inside AI  │
│    │ on Signs & Shirts           │ video. Composite 100% of text in post!       │
├────┼─────────────────────────────┼──────────────────────────────────────────────┤
│ 5  │ Logo Hallucination          │ Never prompt "Autism Alliance logo" into AI. │
│    │                             │ Composite official SVG vector in DaVinci.    │
├────┼─────────────────────────────┼──────────────────────────────────────────────┤
│ 6  │ Uncanny Creepy Human Teeth  │ Lock mouth style: "smooth stylized closed    │
│    │                             │ cartoon mouth line; no visible human teeth". │
├────┼─────────────────────────────┼──────────────────────────────────────────────┤
│ 7  │ Character Color Shift       │ Hardcode HEX values (`#BEE3F8`, `#2B95E9`);  │
│    │ (Grey elephant / navy body) │ discard any generation deviating >5% delta E.│
├────┼─────────────────────────────┼──────────────────────────────────────────────┤
│ 8  │ Duplicated Doppelgängers    │ Negative prompt: "twin characters, clone,    │
│    │ (Two Gappus in one frame)   │ two elephants, duplicate dolphin".           │
├────┼─────────────────────────────┼──────────────────────────────────────────────┤
│ 9  │ Texture Melting in Motion   │ Reduce Kling motion velocity to < 3.0; avoid │
│    │                             │ rapid camera pans across detailed B-roll.    │
├────┼─────────────────────────────┼──────────────────────────────────────────────┤
│ 10 │ Creepy Gaze / Wandering Eyes│ Enforce dual white specular catchlights in   │
│    │                             │ keyframes before video interpolation.        │
└────┴─────────────────────────────┴──────────────────────────────────────────────┘
```

---

## 2. Universal Negative Prompt Suite (Copy-Paste Ready)

Every image and video prompt must include this standardized master negative block:

### Universal Negative Block:
```text
(worst quality, low quality:1.4), (deformed, distorted, disfigured:1.3), human fingers, five fingers on paws, sharp human teeth, open gaping mouth, vampire teeth, scary eyes, pupil strabismus, limp hose trunk, multiple trunks, extra ears, pointed cat ears, fish scales, gills, shark dorsal fin, vertical caudal tail, human legs on dolphin, mermaid, extra limbs, missing limbs, floating disconnected limbs, text, words, watermark, logo, signature, copyright, misspelled text, blurry, morphing geometry, flicker, uncanny valley, hyperrealistic photorealism, doll, creepy porcelain doll, oversaturated, neon green, dark depressing atmosphere.
```

---

## 3. The Post-Production Compositing Rule (Non-Negotiable)

Generative AI video engines excel at character animation and lighting, but notoriously hallucinate written typography and corporate emblems. 

**Operational Rule:**
1.  All background signs, whiteboards, school schedules, and book covers are generated **blank or with abstract color blocks**.
2.  The Post-Production Video Editor tracks the surface in DaVinci Resolve / Premiere and lays down clean, crisp, legible typography and the official Autism Alliance vector logo (`brand/autism-alliance-logo.svg`).
3.  This guarantees **100% legal trademark compliance** and zero misspelled AI text.
