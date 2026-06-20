# AI Production Pipeline: Hermes Video Generation Protocol

This document outlines the standard operating procedure for producing Meta video ads autonomously using AI tools, bridging the gap between script generation and final video output.

## 1. Core Tool Stack

The Hermes production pipeline relies on the following core tools:
*   **Avatar/Video Generation:** HeyGen (or equivalent AI avatar generator)
*   **Voice/Audio Synthesis:** ElevenLabs
*   **B-Roll/Visual Sourcing:** Midjourney (for custom stills), Storyblocks/Envato (for stock video), or client-provided assets
*   **Editing/Assembly:** CapCut (or programmatic video assembly API)

## 2. HeyGen Prompting & Avatar Selection

The visual representation of the speaker is critical for establishing trust and matching the buyer persona.

### Avatar Archetypes
Select the avatar based on the chosen Tone & Voice:
*   **Clinical Authority:** Professional attire (scrubs, lab coat, or business casual), well-lit office or clinical background. Demeanor should be calm, authoritative, and direct.
*   **Empathetic Confessor:** Casual attire (t-shirt, hoodie), living room or bedroom background (UGC style). Demeanor should be vulnerable, relatable, and conversational.
*   **Urgent Whistleblower:** Casual or business casual, dynamic background (walking, in a car, or office). Demeanor should be intense, leaning forward, using hand gestures.
*   **Data Hacker:** Smart casual, tech-focused background (screens, office). Demeanor should be analytical, sharp, and focused.

### Prompting Best Practices
*   **Lighting:** Specify "natural daylight" or "soft ring light" for UGC styles; "studio lighting" for authority styles.
*   **Framing:** Use "close-up, eye-level" for high engagement.
*   **Movement:** Add instructions for subtle movements (e.g., "slight head nods," "hand gestures") to increase realism.

## 3. ElevenLabs Voice Settings

Audio quality and tone are just as important as the visual.

### Voice Selection
*   **Clinical Authority:** Deep, steady, articulate.
*   **Empathetic Confessor:** Warm, slightly breathy, conversational pacing.
*   **Urgent Whistleblower:** Fast-paced, energetic, slightly elevated pitch.
*   **Data Hacker:** Clear, concise, articulate, moderate pace.

### Settings Configuration
*   **Stability:** 30-50% (Lower stability increases emotion and variability; higher stability is more consistent but can sound robotic).
*   **Clarity + Similarity Enhancement:** 70-85% (High clarity ensures the message is understood).
*   **Style Exaggeration:** 10-20% (Use sparingly to add emotion without sounding unnatural).

## 4. B-Roll Strategy & Sourcing

B-roll is used to break visual monotony, demonstrate the mechanism, and show the product in action.

### Sourcing Rules
*   **Rule of Thirds:** The video should be roughly 1/3 A-roll (avatar), 1/3 mechanism/problem visualization, and 1/3 product demonstration.
*   **Pacing:** Cut to B-roll every 3-5 seconds to maintain attention.
*   **Relevance:** B-roll must directly match the spoken word (e.g., if talking about "joint pain," show a person rubbing their knee).

### Types of B-Roll
*   **The Problem:** Visually represent the pain point (e.g., frustration, physical discomfort).
*   **The Mechanism:** Abstract or literal representation of how the product works (e.g., 3D animation of cells, pouring liquid).
*   **The Solution:** The product in use, showing positive emotion.

## 5. Text Overlay & Formatting Specs for Meta

Text overlays (captions and call-outs) are mandatory for Meta ads, as many users watch with sound off.

### Caption Specs
*   **Font:** Bold, highly legible (e.g., Montserrat, Proxima Nova, Arial Black).
*   **Color:** White or yellow text with a black outline or drop shadow for contrast against any background.
*   **Placement:** Lower third of the screen, but *above* the Meta UI elements (leave the bottom 20% clear).
*   **Pacing:** 1-3 words per screen, fast-paced (Alex Hormozi style) to keep the eye moving.

### Call-Out Specs
*   **Purpose:** Highlight key benefits, mechanisms, or the offer.
*   **Design:** Use high-contrast boxes or arrows to draw attention.
*   **Placement:** Upper third or middle of the screen, away from the captions.

## 6. Assembly & Final Polish

*   **Hook (0:00 - 0:03):** Strong visual + text overlay matching the spoken hook.
*   **Body (0:03 - 0:45):** Interleave A-roll and B-roll. Ensure audio transitions are smooth.
*   **Call to Action (0:45 - 1:00):** Clear verbal CTA, on-screen text of the offer, and a visual of the product/landing page.
*   **Aspect Ratio:** 9:16 (Vertical) for Reels/Stories; 4:5 for Feed. Export both if possible.
