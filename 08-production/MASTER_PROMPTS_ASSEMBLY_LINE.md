# The Assembly Line: Master AI Prompts

This document contains the 6 master prompts required to turn a blank page into a batch of production-ready ad variants in 30 minutes.

**How to use this:**
Feed these prompts sequentially into your LLM (ChatGPT, Claude, or Hermes). The output of Prompt 1 becomes the input for Prompt 2, and so on.

---

## Prompt 1: The Angle Generator (Product Brief → 5 Angles)

**Purpose:** Extracts the psychological core of the product and generates 5 distinct angles based on the 6-Axis Matrix.

```text
Act as an elite direct-response creative strategist who has spent $50M+ on Meta ads.

I am going to give you a product brief. Your job is to extract the core psychology and generate 5 distinct advertising angles. Do not write the ad copy yet. Just define the angles.

Here is the product brief:
[INSERT PRODUCT URL OR BRIEF HERE]

For each of the 5 angles, you must provide:
1. **The Angle Name:** (e.g., The "Failed Surgery" Angle)
2. **The Core Emotion:** (e.g., Frustration, Betrayal, Relief)
3. **The Villain:** Who or what is to blame for the prospect's problem? (Must be specific, not vague)
4. **The Mechanism:** How does this product actually work to defeat the villain? (Explain it like I'm 5, but use a proprietary-sounding name)
5. **The Proof:** What is the most believable piece of evidence we can show?
6. **The Target Persona:** Which of the 4 archetypes (Authority, Skeptic, Confessor, Demonstrator) is best suited to deliver this angle?

Make the angles completely distinct from one another. We are testing for psychological resonance, not slight variations in wording.
```

---

## Prompt 2: The Hook Generator (1 Angle → 10 Hooks)

**Purpose:** Takes the winning angle and generates 10 distinct scroll-stopping hooks using the Viral Hooks Framework.

```text
Act as an elite direct-response creative strategist.

We have selected a winning angle for our product. Now we need to test hooks.

Here is the winning angle:
[PASTE ONE ANGLE FROM PROMPT 1]

Your job is to generate 10 completely different hooks (the first 3 seconds of the ad) for this angle. You must use the 8 core formulas from our Viral Hooks Framework.

For each hook, provide:
1. **The Hook Formula Used** (e.g., Vulnerability Story, Contrarian/Polarizing, Extreme Contrast, Specific Curiosity Gap, Identity/Tribal Label, Paradox/Injustice, Near Death Experience, Objection-as-Hook)
2. **The Visual Hook (0:00-0:03):** What exactly are we seeing on screen? (Must be specific, native-looking, and high-contrast)
3. **The Audio Hook (0:00-0:03):** What exactly is being said? (Must be 1-2 sentences maximum, punchy, and emotional)
4. **The Text Overlay (0:00-0:03):** What words are written on the screen? (Must be short, 1-4 words, using the "Single Loaded Word" system if possible)

Do not write the rest of the ad. Only the first 3 seconds. Make them punchy. Use specific numbers. Lead with emotion, not product features.
```

---

## Prompt 3: The Script Writer (Hook + Angle → Full Script)

**Purpose:** Takes a hook and an angle and writes a complete 60-second video script in the 3-column format.

```text
Act as an elite direct-response copywriter.

I need you to write a full 60-second video ad script.

Here is the Angle we are using:
[PASTE ANGLE]

Here is the Hook we are using:
[PASTE HOOK]

Write a 60-second script using the standard direct-response structure:
1. Hook (0-3s)
2. Problem Agitation / Villain Reveal (3-15s)
3. Mechanism Reveal / Solution (15-35s)
4. Proof / Social Proof (35-45s)
5. Call to Action (45-60s)

Format the output as a 3-column table with the following headers:
- **Time / Section** (e.g., 0:00-0:03 Hook)
- **Visual / B-Roll / Text Overlay** (Exactly what is on screen)
- **Audio / Voiceover** (Exactly what is being said)

The tone must be native to social media. No polished corporate speak. Use the "Ugly Ad" principle. Make it sound like a real person talking to a friend.
```

---

## Prompt 4: The Image Ad Generator (Script → 5 Image Ad Variants)

**Purpose:** Translates a winning video script into 5 primary text variations for image ads.

```text
Act as an elite direct-response copywriter.

We have a winning video script. I want to adapt this winning psychology into 5 variations of primary text for Facebook/Instagram Image Ads.

Here is the winning script:
[PASTE SCRIPT]

Write 5 distinct primary text variations. They should range from short-form to long-form advertorial style.

Variation 1: The Long-Form Story (500+ words, reads like a journal entry or confession)
Variation 2: The Contrarian Rant (200 words, aggressive, calls out the villain)
Variation 3: The Clinical Breakdown (300 words, focuses heavily on the mechanism and proof)
Variation 4: The "Ugly" Listicle (150 words, bullet points, highly readable)
Variation 5: The Direct Offer (50 words, straight to the point, urgency driven)

For each variation, suggest the specific type of image that should accompany it (e.g., iPhone selfie, clinical diagram, before/after, ugly native photo).
```

---

## Prompt 5: The Winner Autopsy (Data → Diagnosis)

**Purpose:** Analyzes Meta performance data to determine *why* an ad won or lost, and dictates the next move.

```text
Act as an elite media buyer and creative strategist.

I am going to give you the performance data for a batch of ads we just tested.

Here is the data:
[PASTE DATA: Ad Name, Hook Rate, Hold Rate, CTR, CPA, ROAS]

Based on this data, run a "Winner/Loser Autopsy" and tell me exactly what to do next.

Provide:
1. **The Winners:** Which ads won and WHY? (Analyze the hook, angle, and format)
2. **The Losers:** Which ads died and WHY? (Where did the drop-off happen? Hook? CTR? Conversion?)
3. **The Next Move:** Based on the diagnosis, what is the exact next batch of creatives we need to produce? 
   - If we found a winning angle but bad hooks → Suggest 5 new hooks for that angle.
   - If we found a winning hook/angle but CPA is rising (fatigue) → Suggest a "Frankenstein" refresh (new B-roll, same audio).
   - If everything failed → Suggest a completely new angle.
```

---

## Prompt 6: The Batch Production Brief

**Purpose:** Takes all the generated assets and outputs a clean, organized handoff document for the production team (or AI tools).

```text
Act as an elite creative producer.

I am going to give you a set of approved scripts and image copy.

[PASTE APPROVED SCRIPTS AND COPY]

Your job is to organize this into a clean "Batch Production Brief" so I know exactly what assets need to be created.

Provide:
1. **Naming Conventions:** Assign a clear tracking name to every variant (e.g., VID_Angle1_Hook3_UGC).
2. **Shot List / B-Roll Needs:** A consolidated list of every visual asset we need to film, source, or generate.
3. **Voiceover Needs:** A consolidated list of every audio track that needs to be recorded or generated via ElevenLabs.
4. **Text Overlays:** A list of all text overlays required.
5. **Assembly Instructions:** Clear instructions on which audio goes with which visuals.
```
