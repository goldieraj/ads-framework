# Performance Diagnosis System: Meta Ads Interpretation

This document provides the framework for interpreting Meta Ads performance data, identifying bottlenecks, and making data-driven decisions on creative iteration.

## 1. Core Metrics Hierarchy

Hermes prioritizes metrics based on their direct impact on revenue.

### Primary Metrics (The "North Star")
1.  **Cost Per Acquisition (CPA) / Cost Per Purchase:** The ultimate measure of success. If CPA is below target, the ad is winning, regardless of other metrics.
2.  **Return on Ad Spend (ROAS):** Crucial for e-commerce, measuring revenue generated per dollar spent.

### Secondary Metrics (The Diagnostic Layer)
1.  **Click-Through Rate (CTR - Link Click):** Measures the ad's ability to drive traffic.
    *   *Benchmark:* > 1.0% (Varies by niche, but < 0.5% indicates a problem).
2.  **Cost Per Click (CPC - Link Click):** The cost of acquiring a visitor.
3.  **Thumbstop Ratio (3-Second Video Plays / Impressions):** Measures the effectiveness of the hook.
    *   *Benchmark:* > 25-30%.
4.  **Hold Rate (ThruPlays / 3-Second Video Plays):** Measures the ability of the body copy/visuals to retain attention after the hook.

## 2. Diagnostic Scenarios & Actions

Use this matrix to diagnose underperforming ads and determine the next iteration.

| Scenario | Diagnosis | Action |
| :--- | :--- | :--- |
| **High CPA, Low Thumbstop (< 20%)** | The hook is failing. Users are scrolling past before hearing the message. | **Iterate Hook:** Keep the body/offer, but test 3-5 new visual/verbal hooks (first 3 seconds). |
| **High CPA, High Thumbstop, Low Hold Rate** | The hook works, but the body copy or pacing loses them. The mechanism or villain isn't resonating. | **Iterate Body:** Keep the hook. Test a new mechanism explanation, speed up the pacing, or add more engaging B-roll. |
| **High CPA, High Hold Rate, Low CTR** | People are watching, but not clicking. The Call to Action (CTA) or Offer is weak, or the ad doesn't create enough urgency. | **Iterate CTA/Offer:** Strengthen the CTA, add urgency (e.g., "Limited stock"), or clarify the offer text on screen. |
| **Low CPA (Winning Ad)** | The ad is profitable. | **Scale & Spin-off:** Increase budget. Create variations (spin-offs) using the same winning angle but different formats or slightly altered hooks to prevent fatigue. |

## 3. The "Kill, Scale, Iterate" Protocol

*   **Kill:** If an ad has spent 2x-3x the target CPA without a purchase, turn it off.
*   **Scale:** If an ad is consistently hitting or beating the target CPA for 3-5 days, incrementally increase the budget (typically 10-20% per day, or use Meta's Advantage+ Campaign budget).
*   **Iterate:** If an ad shows promise (good thumbstop, decent CTR) but is slightly above target CPA, use the diagnostic scenarios above to create a new version.

## 4. Analyzing Audience Feedback

Beyond quantitative metrics, monitor qualitative feedback:
*   **Comments:** Are users asking questions? Address those in the next iteration. Are they complaining about price? The value proposition isn't clear enough.
*   **Shares:** High share rates indicate high resonance, often driven by a strong "Villain" or relatable "Empathetic Confessor" angle.
