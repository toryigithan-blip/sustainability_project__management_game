# Water Project

A strategy game where you design a water-saving project for farmers, and the game tells you what kind of project you built.

Built as a workshop game for World Water Week 2026. Playable in the browser, no install needed.

## Play the Game

**[Play online: yigithan-water-project.netlify.app](https://yigithan-water-project.netlify.app)**

> **If the link does not work:** download `index.html` from this repository and open it in any modern browser (Chrome, Edge, Safari, Firefox). No installation or server is needed. Use a landscape phone, tablet or desktop screen for the best experience. Live team submissions need an internet connection and may not work when the file is opened locally.

---

## Executive Summary

- **What it is:** A resource-management strategy game played in teams on phones or tablets.
- **Goal:** Deliver 500 ML of water benefit per year using a limited budget (1,000,000 credits) and limited land (1,000 hectares).
- **Core idea:** There is no single winning build. Many strategies reach the target, so the interesting part is *how* you get there and *what you do with what is left*.
- **Outcome:** At the end, the game reveals your project's **Archetype**, **Philosophy** and an **Activity Summary**, plus hidden benefits and trade-offs you did not see while playing.
- **Design intent:** The layered, interconnected structure is deliberate. It mirrors how real agricultural water projects at Doktar are built, where technology, measurement, training and farmer support all depend on each other.
- **Why it matters for games:** Systems design, economy balancing, hidden-state scoring, emergent player identity and a live multiplayer host dashboard, all in a single-file web app.

---

## The Idea in Plain Words

Imagine you manage a project that helps farmers use less water.

You have money and land, but not unlimited amounts. You decide:

1. **What to do** on the land (for example, better irrigation or restoring a wetland)
2. **How to prove it works** (measure the water saved)
3. **How to teach farmers** to use it properly (training)
4. **How to keep them supported** over time (ongoing help and communication)

If you only buy technology and skip the farmers, it underperforms. If you skip measurement, nobody can trust the result. The game rewards choices that work together.

---

## How a Round Plays

1. **Name your team** and start.
2. **Create workstreams.** Each one is a part of your project with its own land size and farmers.
3. **Pick activities** from four groups: Interventions, Measurement, Training, Extension Support.
4. **Hit the 500 ML target**, then decide how to spend what remains. This choice reveals your priorities.
5. **Submit** and see what you built.

---

## What the Player Gets at the End

### Primary Archetype
The *type* of water solution your project is. It comes from where most of your water benefit came from.

Examples: *Withdrawal-Reduction Project*, *Recharge Project*, *Alternative-Supply Project*, *Treatment Project*, or *Balanced Systems Project* if no single approach dominates.

### Secondary Philosophy
The *mindset* behind your choices. It is scored quietly in the background and only revealed at the end.

Examples: *Soil Regeneration*, *Climate Adaptation*, *Ecosystem Restoration*, *Water Stewardship*, *Farmer Empowerment*, *Data-Driven Stewardship*, or *Integrated Watershed* if you mixed several evenly.

### Activity Summary
A short plain-language recap of your run: how many workstreams, how much land and how many farmers you reached, where your water benefit came from, what supported it, and how many bundles and trade-offs you triggered.

### Also revealed
- **Hidden benefits** such as yield, biodiversity, soil health and farmer engagement
- **Bundles:** bonus rewards for combining activities that belong together
- **Trade-offs:** penalties for risky or unsupported choices
- **Suggestions:** what you could have added to improve

Two teams can both reach 500 ML and end up with completely different identities.

---

## Why the Game Is Complex on Purpose

The structure is not complexity for its own sake. It is a deliberate model of how real projects at Doktar are layered:

| In the game | In a real project |
|---|---|
| Interventions | The actual changes made in the field |
| Measurement & Traceability | Proving the impact is real and reportable |
| Training | Building farmer knowledge and capability |
| Extension Services | Ongoing field support and communication |
| Workstreams | Separate project components with their own scope |
| Bundles | Activities that only deliver full value together |
| Trade-offs | Risks that appear when a layer is missing |

Players feel the lesson instead of reading it: a project is only as strong as the layers around the main action.

---

## Design Highlights

- **Constrained economy:** two budgets (money and land) force real trade-offs.
- **Emergent identity:** the player never picks an archetype. It is derived from their behavior.
- **Hidden scoring layer:** outcomes are revealed only at the end, which creates a "reveal" moment and drives discussion.
- **Synergies and penalties:** combo bundles and trade-offs reward systems thinking over stacking one thing.
- **Live host screen:** a facilitator view shows all teams in the room, their choices and a generated debrief. The framing is "no winners, just priorities".

---

## Tech

- Single-file web app (HTML, CSS, vanilla JavaScript), no build step
- Firebase Firestore for live team submissions
- Built for landscape phones and tablets

## Run It

1. Open `index.html` in a browser (or use the [live link](https://yigithan-water-project.netlify.app)).
2. For live submissions, add your own Firebase config in `index.html`.

---

*Values and results are workshop mechanics for learning and discussion, not verified water accounting claims.*
