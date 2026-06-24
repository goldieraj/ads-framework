# The Assembly Line: Master AI Prompts

This document contains the automated prompt sequences required to turn a blank product brief into production-ready ad variants. 

**The system operates on a 3-Track Automation Model:**
1. **Track 1: Image Ads (Fully Automated)** — Brief in → Ads out → Auto-launch. No human review required.
2. **Track 2: Short Video (7-30s)** — Near-automated. Brief in → AI generates scripts → 30-second human skim/approval → Sent to AI tools for assembly.
3. **Track 3: Long Video (30s-5min)** — Hybrid. AI generates the script and voiceover. Outputs an "editor-ready package" for a human video editor to assemble.

Feed these prompts into your LLM (ChatGPT, Claude, or Hermes). 

---

## ⚠️ Creative Diversity Mandate (Apply to Every Batch)

> **Source:** Meta's AI-driven "Soulmate Theory" algorithm groups visually similar ads under the same **Entity ID**, causing them to cannibalize each other's reach — even if the copy is different. Two ads that look the same to Meta = one ad's worth of delivery.

**Before finalizing any batch, verify that no two ads share the same Entity ID fingerprint.** Meta determines Entity ID using three signals, in order of weight:

| Signal | Weight | What to Change |
|---|---|---|
| **Format** | Highest | VSL vs. UGC vs. Animation vs. Talking Head vs. Demo |
| **Visual Vehicle / Hook** | High | Different actor, different setting, different opening visual |
| **Persona** | Medium | Different avatar shown (age, gender, situation) |
| Messaging / Copy | Low | Changing copy alone does NOT create a new Entity ID |

### The Diversity Checklist (Run Before Every Batch)

Before submitting a batch for production, confirm:

- [ ] **No two ads use the same format** (e.g., do not submit 3 talking-head scripts with the same actor)
- [ ] **No two ads open with the same visual vehicle** (same location + same person + same opening shot = same Entity ID)
- [ ] **At least 2 different personas** are represented across a batch of 4+ ads
- [ ] **At least 2 different formats** are represented across any batch of 3+ ads
- [ ] **Long-form and short-form are treated as separate entities** (a 3-min VSL and a 30s cut-down of the same footage = same Entity ID — re-shoot the short with a different hook)

### Batch Composition Rules

| Batch Size | Minimum Format Variety | Minimum Persona Variety |
|---|---|---|
| 3 ads | 2 formats | 1 persona OK |
| 5 ads | 3 formats | 2 personas |
| 8+ ads | 4 formats | 3 personas |

### The Differentiation Pyramid (Reference When Iterating)

When an ad is fatiguing and needs a refresh, change elements from the **top of the pyramid down** — not from the bottom up:

```
        ┌─────────────────┐
        │   1. FORMAT     │  ← Biggest impact. Switch VSL → UGC → Animation
        ├─────────────────┤
        │ 2. VISUAL HOOK  │  ← New actor, new setting, new opening shot
        ├─────────────────┤
        │  3. PERSONA     │  ← Different avatar (age, gender, situation)
        ├─────────────────┤
        │  4. PRODUCT     │  ← Different product angle or benefit
        ├─────────────────┤
        │  5. MESSAGING   │  ← Least impact. Copy-only changes = same Entity ID
        └─────────────────┘
```

**Rule:** If an ad is fatiguing, start at the top. Changing only messaging (bottom) is wasted spend — Meta still treats it as the same ad.

---

## Track 1: The Image Ad Auto-Launcher (100% Automated)

**Purpose:** Runs the entire pipeline end-to-end for image ads. It analyzes the product, selects the best angles, writes the hooks, generates the ad copy, and outputs final text ready for immediate upload to Meta Ads Manager.

**How to use:** Paste this single prompt and provide the product brief. The AI does the rest.

```text
Act as an elite direct-response creative strategist who has spent $50M+ on Meta ads.

I am going to give you a product brief. Your job is to run an end-to-end automated pipeline to produce 5 ready-to-launch Image Ads. You will not ask for my input or approval at any step. You will execute the entire process and output the final deliverables.

Here is the product brief:
[INSERT PRODUCT URL OR BRIEF HERE]

**Execute the following steps internally:**
1. Extract the core psychology (Pain, Mechanism, Villain, Proof).
2. Generate the top 3 advertising angles based on the 6-Axis Matrix.
3. Select the single strongest angle based on emotional resonance and proof.
4. Generate 5 distinct hooks for that winning angle using the Viral Hooks Framework.
5. Translate those 5 hooks into 5 distinct primary text variations for Facebook/Instagram Image Ads.

**Output the final deliverables in this exact format:**

For each of the 5 variations, provide:
- **Variant Name:** (e.g., IMG_Angle1_Hook3_LongForm)
- **Primary Text:** (The actual ad copy. Must include 1 Long-Form Story, 1 Contrarian Rant, 1 Clinical Breakdown, 1 "Ugly" Listicle, and 1 Direct Offer.)
- **Headline:** (Short, punchy, 3-5 words)
- **Visual Direction:** (Exactly what type of image should accompany this text. e.g., "Ugly iPhone selfie of the product on a messy counter" or "Clinical diagram showing the mechanism.")

Do not ask for feedback. Just output the 5 ready-to-launch variants.
```

---

## Track 2: Short Video Pipeline (7-30s) (One-Click Approve)

**Purpose:** Near-automated pipeline for UGC, talking head, or fast B-roll ads. AI selects the angle, writes the script, and pauses ONLY for your 30-second review before generating the production brief for AI assembly tools (HeyGen/ElevenLabs).

### Step 1: The Auto-Scripter

```text
Act as an elite direct-response creative strategist and copywriter.

I am going to give you a product brief. Your job is to automatically select the best angle and write 3 complete short-form video scripts (7-30 seconds each). 

Here is the product brief:
[INSERT PRODUCT URL OR BRIEF HERE]

**Execute the following steps internally:**
1. Analyze the product and determine the absolute strongest Angle.
2. Select 3 distinct hook formulas from the Viral Hooks Framework (e.g., Vulnerability Story, Extreme Contrast, Objection-as-Hook).
3. Write 3 complete, fast-paced video scripts (max 60 words each).

**Output the 3 scripts in a 3-column format:**
- **Time / Section** (e.g., 0:00-0:03 Hook)
- **Visual / B-Roll / Text Overlay** (Exactly what is on screen. Keep text overlays to 1-4 words using the Single Loaded Word system.)
- **Audio / Voiceover** (Exactly what is being said. Must be punchy, native, and emotional.)

Ask me: "Do you approve these scripts for production?"
```

### Step 2: The AI Assembly Brief (Run after approval)

```text
I approve the scripts. Now, translate them into a Batch Production Brief designed specifically for AI video generation tools (HeyGen, ElevenLabs, CapCut).

For each approved script, provide:
1. **Tracking Name:** (e.g., VID_Short_Hook1_UGC)
2. **Avatar/Voice Spec:** (e.g., "HeyGen Avatar: 35yo stressed mom. ElevenLabs Voice: 'Rachel' - frustrated tone.")
3. **Voiceover Script:** (The raw text to paste into ElevenLabs, stripped of visual directions)
4. **Text Overlays & Timestamps:** (Exactly what text appears on screen and when)
5. **B-Roll Prompts (if needed):** (Descriptions for AI image/video generators to create background visuals)
```

---

## Track 3: Long Video Pipeline (30s-5min) (Editor-Ready Package)

**Purpose:** Hybrid pipeline for long-form VSLs or story ads. AI handles the heavy lifting (scripting, voiceover generation instructions) and outputs an organized package that a human video editor can assemble.

### Step 1: The Long-Form Scripter

```text
Act as an elite direct-response copywriter specializing in long-form video sales letters (VSLs) and story ads.

I need a comprehensive script (1 to 3 minutes) based on this product brief:
[INSERT PRODUCT URL OR BRIEF HERE]

**Execute the following steps:**
1. Identify the strongest "Villain" and "Mechanism" for this product.
2. Write a full script using the standard direct-response structure:
   - Hook (0-5s)
   - Problem Agitation / Villain Reveal (5-20s)
   - Mechanism Reveal / Solution (20-45s)
   - Proof / Social Proof (45-75s)
   - Call to Action (75s+)

**Output the script in a 3-column format:**
- **Time / Section**
- **Visual / B-Roll / Text Overlay** (Detailed instructions for the human editor)
- **Audio / Voiceover** (The exact script)

Make it compelling, well-paced, and heavily reliant on the "Constructed Authority" or "Demonstrator" personas.
```

### Step 2: The Editor-Ready Package (Run after script approval)

```text
I approve the script. Now, build the "Editor-Ready Package" so I can hand this directly to my human video editor.

Provide:
1. **The Voiceover File Spec:** (Instructions for ElevenLabs or a human voice actor regarding tone, pacing, and emotion).
2. **The Master Shot List:** (A bulleted list of every piece of B-roll, stock footage, or product shot the editor needs to source).
3. **Text Overlay Master List:** (All on-screen text, including the specific seconds they should appear and disappear).
4. **Pacing & Editing Instructions:** (Specific directions for the editor, e.g., "Fast cuts during the agitation phase, slow down during the mechanism reveal. Use a 'cash register' sound effect at 1:15.")
```

---

## The Feedback Loop: Prompt 5 (Winner Autopsy)

**Purpose:** Analyzes Meta performance data across all tracks to determine *why* an ad won or lost, and dictates the next move.

```text
Act as an elite media buyer and creative strategist.

I am going to give you the performance data for a batch of ads we just tested.
[PASTE DATA: Ad Name, Hook Rate, Hold Rate, CTR, CPA, ROAS]

Based on this data, run a "Winner/Loser Autopsy" and tell me exactly what to do next.

Provide:
1. **The Winners:** Which ads won and WHY? (Analyze the hook, angle, and format)
2. **The Losers:** Which ads died and WHY? (Where did the drop-off happen? Hook? CTR? Conversion?)
3. **The Next Move:** Based on the diagnosis, what is the exact next batch of creatives we need to produce? 
   - If we found a winning angle but bad hooks → Suggest 5 new hooks for that angle.
   - If we found a winning hook/angle but CPA is rising (fatigue) → Apply the **Differentiation Pyramid**: change Format first (e.g., VSL → UGC), then Visual Hook (new actor/setting), then Persona. Do NOT just rewrite the copy — Meta treats copy-only changes as the same Entity ID.
   - If everything failed → Suggest a completely new angle with a completely different format.
4. **Entity ID Diversity Check:** Review the proposed next batch and confirm no two ads share the same Format + Visual Vehicle + Persona combination. Flag any that would receive the same Entity ID.
```
