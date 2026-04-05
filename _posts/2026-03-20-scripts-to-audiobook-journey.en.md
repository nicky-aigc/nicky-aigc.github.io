---
layout: post
title: "Scripts to Audiobook: An AI Coding Journey"
date: 2026-03-20 00:00:00 +0800
tags: [AI, typescript, audiobook, open-source, development]
excerpt: "A personal passion project born from my love for movies and audiobooks. Built in ~5 days across a weekend with three different AI coding assistants."
lang: en
slug: scripts-to-audiobook-journey
permalink: /blog/scripts-to-audiobook-journey
---

![Scripts to Audiobook](/images/scripts-to-audiobook-dark.png)

# Scripts to Audiobook: An AI Coding Journey 🎧

I'm a movie buff and an avid audiobook consumer. For a while, I'd been thinking: **what if I could automatically generate personalized audiobooks from AI-generated scripts?**

That personal itch led to my latest project: **Scripts to Audiobook** — a tool to convert scripts into multi-voice audiobooks with configurable TTS providers.

I started building on March 15th and shipped by the early hours of March 20th. In those ~5 days (including a weekend), I cycled through three AI coding assistants. Here's what happened.

## The Starting Point: Perplexity Computer Use

I started with **Perplexity's Computer Use** feature, drawn by its promise of "high completion rates" and impressive real-time preview capabilities. As a Pro subscriber (4,500 credits), I gave it a serious shot — running from 3,400+ credits down to 2,200+ before pausing.

My experience was mixed:

**What worked:**
- **Real-time preview** — Seeing changes instantly was incredibly valuable
- **Interactive development** — The conversational flow felt natural and efficient
- **Quick prototyping** — Great for testing ideas and rapid iteration

**What didn't:**
- **Credits burn fast** — 1,200+ credits for partial completion adds up
- **Completion gap** — The AI tended to "brand" things aggressively (naming after itself), which required manual cleanup
- **Production readiness** — While impressive for demos, the output needed significant polish for real use

I stopped not because it couldn't do the job, but because the credits cost for full completion wasn't worth it given the current state. It's a fantastic tool for exploration and demos, but I'd save it for smaller projects or validation phases.

## Phase Two: Kimi Code & Token Burn

I switched to **Kimi Code**, hoping its focused approach would be more effective. It worked — and I burned through two weekly quotas in rapid succession.

Here's what happened: I'd exhaust my quota, it would reset, and I'd burn through it again. Partly because I was working intensely over a weekend, but mostly because:

1. **Scope creep** — Requirements evolved mid-build (new TTS providers, audio format options, chapter support)
2. **Refactor cycles** — Fixing bugs led to more bugs, leading to repeated rewrites
3. **Context loss** — Starting fresh sessions meant re‑explaining the project each time

The tool itself was capable, but the workflow was inefficient. I was trading time for tokens.

## Phase Three: Claude Code & The Finish Line

Finally, I switched to **Claude Code** (Anthropic's terminal-based coding agent). Three things made it click:

1. **Rich project context** — It could read the entire codebase and understand the architecture
2. **Iterative refinement** — Small, targeted changes instead of wholesale rewrites
3. **Stability** — What worked yesterday kept working today

In one focused session, I:
- Implemented the remaining features (chapter support, TTS switching)
- Fixed all outstanding bugs
- Polished the UI and documentation
- Wrote comprehensive tests

**The difference?** It felt like working with a senior engineer who understood the big picture.

## The Output: What I Built

After all that, here's what I built:

**Scripts to Audiobook** converts structured scripts into multi-voice audiobooks using your choice of TTS provider.

### Key Features

- 🎭 **Multiple voices** — Assign different voices to each character
- 📖 **Chapter support** — Organize long content into sections
- 🔧 **TTS flexibility** — Switch between providers (Edge TTS, OpenAI, ElevenLabs, etc.)
- 🎛️ **Configurable output** — Control audio format, bitrate, and speed

### What Makes It Special

- **Free to use** — Edge TTS requires no API key; other providers offer free tiers
- **AI-agnostic** — Works with scripts from any AI (Claude, GPT, Gemini, etc.)
- **Beginner-friendly UI** — Simple configuration interface, no coding required

## Tech Stack

- **TypeScript** — Type safety and better DX
- **Node.js** — Cross‑platform runtime
- **Edge TTS / OpenAI / ElevenLabs** — TTS providers
- **FFmpeg** — Audio processing and format conversion

## Key Learnings

1. **Tool choice matters** — Different AI coding assistants have different strengths. Match the tool to the phase.
2. **Token efficiency** — Rich context and iterative refinement beat brute‑force rewriting.
3. **Ship fast, iterate** — The first version doesn't need to be perfect. It just needs to work.

## The Beauty of AI-Augmented Coding

This entire project — from idea to shipped product — took **less than 5 days**. And I'm not a professional developer.

The beauty isn't in getting it perfect the first time — it's in the ability to iterate rapidly, learn from mistakes, and keep moving forward.

AI coding assistants aren't replacements for human judgment. They're force multipliers. They help you move faster, think bigger, and ship smarter.

## What's Next?

I'm already thinking about v2:
- Web UI for easier configuration
- More TTS providers (Azure, Google, Amazon)
- Voice cloning support
- Batch processing for multiple scripts

But first, I'm taking a break. Shipping feels good. 😊

---

**Check it out on GitHub:** [scripts-to-audiobook](https://github.com/hugcosmos/scripts-to-audiobook)


Made with 💙 by Nicky & AI
