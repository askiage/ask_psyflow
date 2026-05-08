# PsyFlow — AI Marketing Psychology Agent

PsyFlow is an AI marketing psychology agent for indie builders, founders, and small teams. It helps improve landing pages, product positioning, onboarding flows, and campaign copy using behavioral science.

The current repository contains a polished static HTML prototype. The next version can connect the UI to an OpenAI-compatible model API and return structured JSON audits.

## Problem

Small builders often ship products with:

- unclear positioning
- feature-heavy copy before the user understands the outcome
- too many CTAs or setup choices
- weak social proof
- low-confidence onboarding
- no clear A/B test plan

They usually cannot afford a full marketing strategist, CRO consultant, or dedicated growth team.

## Solution

PsyFlow lets a user paste a product page, campaign idea, or onboarding flow. The agent analyzes the text with mental models such as:

- Jobs To Be Done
- AIDA
- Hick's Law
- Social Proof
- Loss Aversion
- Anchoring
- Framing
- BJ Fogg Behavior Model
- EAST Framework

It then returns a practical, ethical marketing audit with prioritized improvements.

## Core Agent Flow

1. User submits product/campaign context.
2. Agent extracts audience, value proposition, desired behavior, friction points, and proof gaps.
3. Agent maps issues to relevant psychology models.
4. Agent generates copy, landing-page structure, CTA improvements, onboarding nudges, and A/B test ideas.
5. Agent outputs a prioritized action plan.

## Demo Features

The static prototype includes:

- landing page for the PsyFlow concept
- input box for product/campaign text
- funnel-stage selector
- desired-behavior field
- psychology model chips
- simulated agent audit report
- conversion clarity score
- workflow explanation
- reusable project description

## How To Run

No build step is required.

Open the file directly:

```bash
open demo.html
```

Or serve it locally:

```bash
python3 -m http.server 8000
```

Then open:

```text
http://localhost:8000/demo.html
```

## Suggested Project Settings

- Agent tool: Web-based AI agent prototype
- Primary model: OpenAI-compatible LLM API
- Project type: AI marketing / growth assistant / copy audit agent

## Project Description

```text
PsyFlow is an AI marketing psychology agent that helps builders improve landing pages, product positioning, onboarding flows, and campaign copy. Users paste their product context, and the agent analyzes it with behavioral science models such as Jobs To Be Done, AIDA, Hick’s Law, Social Proof, Loss Aversion, BJ Fogg Behavior Model, and EAST. It then produces an ethical conversion audit, prioritized action plan, and A/B testing ideas. The goal is to help indie builders and small teams make clearer marketing decisions without hiring a full CRO or marketing strategist.
```

## Why This Works

PsyFlow benefits from a reasoning model because the task is not just copy generation. The agent must understand audience intent, diagnose friction, choose the right psychological model, and return structured recommendations.

## Future API Version

An API-connected version could use this output schema:

```json
{
  "score": 74,
  "audience": "indie builders and small teams",
  "desired_behavior": "start a demo",
  "findings": [
    {
      "model": "Jobs To Be Done",
      "issue": "The page explains features before the buyer's core job is clear.",
      "recommendation": "Rewrite the hero around the outcome the buyer wants."
    }
  ],
  "action_plan": [
    "Clarify the hero promise",
    "Reduce CTA choices",
    "Add social proof",
    "Create one A/B headline test"
  ]
}
```

## Ethics

PsyFlow is designed for ethical persuasion only. It should improve clarity, reduce confusion, and help users make better decisions. It should not recommend fake scarcity, deceptive urgency, manipulative dark patterns, or fabricated social proof.

## Files

```text
README.md   Project explanation and reusable project copy
demo.html   Static interactive prototype
```
