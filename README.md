# Prompt Eval (Evals & Hedgehog Comparison Suite)

An interactive, single-screen web application designed for rigorous, objective comparison of two AI-generated multimodal outputs (**Response A** vs **Response B**). Built for modern evaluation frameworks (including Evals, Hedgehog, and RLHF comparative assessment).

## Core Evaluation Law
> **Prompt adherence always matters more than visual polish.**  
> Extra beauty, realism, detail, or cinematic quality must never outweigh a missed named requirement or stylistic drift.

---

## Features

- **Standardized Preference Scales**:
  - **5-Point Scale**: *Strongly prefer Response A*, *Slightly prefer Response A*, *Tie*, *Slightly prefer Response B*, *Strongly prefer Response B*.
  - **3-Point Scale**: *Prefer Response A*, *Tie*, *Prefer Response B*.
- **Official Decision Logic**:
  - **Strongly Prefer**: Automatically triggered when an output misses an explicit prompt requirement (`score = No`), fails a primary reference detail, or exhibits a conspicuous/major artifact.
  - **Slightly Prefer**: Triggered when both outputs follow all prompt requirements, but one demonstrates visibly superior style fidelity, texture, or cleaner delivery.
  - **Tie**: Triggered when performance across dimensions is balanced.
  - **Choose Neither**: Triggered when both outputs suffer critical requirement failures.
- **Task Family Modes**:
  - 🎨 **T2I (Text-to-Image)**: Separates style consistency, text readability, required objects, and lighting/texture from raw detail. Includes *The Mending Cupboard* worked example.
  - 🎬 **T2V (Text-to-Video)**: Evaluates chronological action sequences and temporal coherence across the entire timeline (not isolated still frames). Includes *Red Panda Sequence* worked example.
  - 🖼️ **R2I (Reference-to-Image)**: Gated by subject identity fidelity to the source reference before overall preference. Includes *Graduation Edit* worked example.
  - 🎙️ **S2S (Speech-to-Speech)**: Checks prompt fairness first, then evaluates naturalness, warmth, pacing, and conversational delivery. Includes *Casual Advice* worked example.
  - 🏊 **Swimming Pool Benchmark**: Dreamcore dry pool scenario demonstrating prompt adherence overcoming visual polish.
- **Automated Justification Engine**:
  - Synthesizes 1–2 sharp sentences following the exact syntax of passing Evals justifications.
  - Strictly grounded in the evaluator's marked checklist items with zero unverified claims.
- **One-Click Submissions**:
  - **Copy Completed Submission**: Copies clean `Completed preference` and `Completed justification` blocks ready to paste directly into your assessment.
  - **Copy Full Audit**: Exports complete metrics, critical status, and checklist breakdowns.
- **100% Offline & Self-Contained**:
  - Zero external CDNs, zero dependencies, zero tracking, no API keys or login required.
  - Automatic `localStorage` saving with JSON Export and Import support.

---

## Getting Started

Simply open `index.html` in any web browser (Chrome, Edge, Firefox, Brave, Safari) by double-clicking it or opening `file:///H:/Projects/Prompt%20Eval/index.html`.
