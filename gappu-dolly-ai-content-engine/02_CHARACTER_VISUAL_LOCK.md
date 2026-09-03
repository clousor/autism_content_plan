# Gappu & Dolly — Character Visual Lock & AI Consistency Architecture

**Document ID:** `GD-LOCK-01`  
**Standard:** Rigorous Parameter & Anatomy Governance for Generative AI Image & Video Engines  
**Mandate:** Zero character drift. Gappu and Dolly must look identical across 100+ generated video scenes.  

---

## 1. The Immutable vs. Variable Governance Matrix

```
┌─────────────────────────────────────────────────────────────────────────┐
│                    THE CHARACTER CONSISTENCY BOUNDARY                   │
├──────────────────────────┬──────────────────────────────────────────────┤
│ 🔒 NEVER CHANGE          │ 🎨 ALLOWED TO VARY                          │
│ (Absolute Lock)          │ (Contextual Range)                           │
├──────────────────────────┼──────────────────────────────────────────────┤
│ • Head-to-body ratios    │ • Facial expressions (Joy, wonder, empathy)  │
│ • Skin and dorsal colors │ • Eye gaze direction & brow angle            │
│ • Eye shape & catchlight │ • Pose (Sitting, standing, gesturing)        │
│ • Trunk length & curves  │ • Physical setting / environment             │
│ • Fan-ear geometry       │ • Handheld props (Crayon, PECS card, ball)   │
│ • Dolly's white belly    │ • Camera angle, framing & depth of field     │
│ • Rosy cheek placement   │ • Lighting mood (Morning sun, soft sensory)  │
│ • Velvet clay 3D texture │ • Weather or seasonal props (Winter cap/muff)│
└──────────────────────────┴──────────────────────────────────────────────┘
```

---

## 2. Gappu Visual Lock Specifications

### A. Non-Negotiable Anatomy Locks
1.  **Trunk Lock:**
    *   *Rule:* Trunk must NEVER exceed 1.2x head length. It must always curve softly upward in an S-profile.
    *   *Failure Mode to Reject:* Extra-long limp trunk, trunk turning into a human nose or hose, multiple nostrils, sharp bends.
2.  **Ear Lock:**
    *   *Rule:* Fan ears must originate from the upper side of the cranial dome and flare outward to shoulder level. Inner ear must display periwinkle shading (`#7AB8E8`).
    *   *Failure Mode to Reject:* Tiny Dumbo wings, pointed mouse ears, human ears underneath, asymmetric detached ears.
3.  **Limb Lock:**
    *   *Rule:* Exactly four rounded limbs. Four toes per foot pad. No human fingers on elephant hands—only smooth, rounded, padded paws with gentle grasp contours.
    *   *Failure Mode to Reject:* Human hands, five articulated fingers, claw-like nails, extra limbs sprouting from torso.
4.  **Color Integrity Lock:**
    *   *Rule:* Base skin must remain soft sky blue (`#BEE3F8`). Never grey, never brown, never neon blue.

---

## 3. Dolly Visual Lock Specifications

### A. Non-Negotiable Anatomy Locks
1.  **Dorsal/Ventral Color Boundary:**
    *   *Rule:* The boundary between her vibrant azure blue back (`#2B95E9`) and pure white underbelly (`#F0F8FF`) must follow a smooth, clean hydrodynamic waterline from the lower jaw beneath the pectoral flippers down to the tail notch.
    *   *Failure Mode to Reject:* Patchy blotches, white belly expanding over dorsal fin, inverted colors.
2.  **Beak & Rostrum Lock:**
    *   *Rule:* Beak is compact, smooth, rounded, and features a subtle upward smile contour.
    *   *Failure Mode to Reject:* Pointed beak, shark-like jaw, open mouth showing sharp mammalian teeth, blowhole on forehead opening into a funnel.
3.  **Fin Symmetry & Shape:**
    *   *Rule:* Single central curved dorsal fin on spine; two wing-like pectoral flippers; one horizontal notched tail fluke.
    *   *Failure Mode to Reject:* Vertical fish tail, scaly mermaid tail, extra flippers, human arms.

---

## 4. Master Character Lock String (Prompt Injection Code)

Every AI generation prompt (Midjourney, Flux, Stable Diffusion, Kling, Runway Gen-3) **must prepend** these exact structured character lock strings:

### Gappu Master Lock Prefix:
```text
[CHARACTER: GAPPU] - cute stylized chibi Asian baby elephant mascot, head-to-body ratio 1:1.2, smooth pear-shaped plump body, soft sky-blue velvet skin #BEE3F8, glowing pastel pink circular cheek blush, large glossy black circular button eyes with dual white catchlights, gentle mobile curved eyebrows, broad fan-shaped soft elephant ears with periwinkle inner gradient, cute short curved elephant trunk curling upward with three subtle horizontal bridge creases, gentle upward mouth line beneath trunk, chubby four-toed rounded paws, Pixar-quality soft 3D stylized children's educational render, subsurface scattering, matte porcelain clay finish, ultra-clean edges.
```

### Dolly Master Lock Prefix:
```text
[CHARACTER: DOLLY] - cute stylized young bottlenose dolphin mascot, sleek aerodynamic arched C-curve body, vibrant azure blue dorsal back #2B95E9, crisp pure white underbelly #F0F8FF, soft coral-pink cheek blush, bright friendly obsidian-black eye with star sparkle highlight, smooth rounded melon forehead, gentle permanent smiling beak line, curved rounded dorsal fin, two expressive paddle-like pectoral flippers, horizontal notched tail fluke with water droplet trail, weightless floating buoyancy, lustrous satin finish, Pixar-quality 3D stylized character.
```

---

## 5. Seed Locking & IP-Adapter Reference Strategy

In models that support image reference weighting (e.g. Midjourney `--cref`, Stable Diffusion ControlNet IP-Adapter, Flux LoRA):

1.  **Master Reference Asset:** `gappu-dolly-ai-content-engine/assets/characters/official_mascot_reference.png`.
2.  **Weighting Thresholds:**
    *   Midjourney: Use `--cref [URL] --cw 85` (keeps facial and body anatomy strictly locked while allowing dynamic pose and background variation).
    *   IP-Adapter (SDXL / Flux): Set `ip_adapter_weight: 0.82`, `control_mode: Balanced`.
    *   Negative Conditioning: Never rely solely on positive prompts; always inject the Failure Prevention negative prompt suite (`13_AI_FAILURE_PREVENTION.md`).
