# Resident Memory: The MemPalace Technical Cheat Sheet

## 1. The Strategic Vision: Solving "Technological Amnesia"

The current agentic landscape suffers from **"Technological Amnesia."** Large Language Models (LLMs) are stateless by design, but the industry’s attempt to fix this—the "Context Window"—is a temporary patch that fails as projects scale. Legacy memory systems like Mem0 and Zep fall into the **Summarization Trap**, acting as a **Lossy Sieve**. These systems delegate the "decision of importance" to the model in real-time, stripping away reasoning and nuance to store only "dry facts." This results in a massive cognitive and economic cost: the loss of the "how" and "why" behind every decision.

**MemPalace** introduces a fundamental shift in agency. Its core differentiator is **Verbatim Retention**. By prioritizing 100% context preservation, MemPalace ensures that the user, through spatial structure, defines what matters—not a real-time summarization algorithm. 

* **Stateless to Persistent:** Moves the agent from a processor to a partner.
* **Originality:** Retains original conversations and architectural decisions without distortion.
* **Spatial Architecture:** Replaces flat, chaotic logs with a structured, physical-digital hierarchy.

---

## 2. The Architecture: Method of Loci Reimagined

In flat search spaces, high-volume memory inevitably leads to chaotic semantic vector collisions. MemPalace solves this via **"Scoped Search"** within a reimagined **Method of Loci**—organizing data into a navigable spatial hierarchy to limit search radii and maximize retrieval precision.

### The Hierarchical Structure
The Palace is organized into five distinct layers:

1.  **Wings:** Top-level domains (e.g., "Engineering," "Personal," "Scriptwriting").
2.  **Rooms:** Sub-topics within Wings. The "Room Detector" uses file paths and keyword routing to automate placement.
3.  **Halls:** Functional routing protocols (**"Diverging Paths"**) that organize data by utility.
4.  **Drawers:** The fundamental **Source of Truth**. Stores original, verbatim files (96.6% Accuracy in Raw Mode).
5.  **Closets:** Storage for the **AAAK dialect**—compressed data for high-speed context loading.

### Memory Type Routing (The Halls)
Within each Room, the "Diverging Paths" protocol routes information:

| Hall | Function |
| :--- | :--- |
| **Facts** | Static knowledge, constants, and raw data points. |
| **Events** | Chronological sequences and episodic occurrences. |
| **Discoveries** | New insights, learned patterns, and technical breakthroughs. |
| **Preferences** | User-specific traits, styles, and personal choices. |
| **Advice** | Guidance, suggested workflows, and philosophical pillars. |

* **Tunnels:** Automatically connect rooms with identical names across different Wings (e.g., "Deployment" in both "Dev" and "Security").

---

## 3. Efficiency & The Token Economy: L0 to L3 Hierarchy

The **"Memory Architecture Paradox"** involves balancing infinite memory with finite context windows. MemPalace utilizes **Lazy Semantic Loading** to keep the context window lean.

### The "Wake-Up" Cost & Trigger Protocols
A tiered hierarchy manages token expenditure during the boot sequence:
* **L0 (Identity):** Agent personality and core traits (~100 Tokens).
* **L1 (Current State):** The top 15 most recently scanned memories (~70 Tokens).
* **Total Initial Wake-up Cost:** ~170 Tokens.

*Deep semantic searches (L2/L3) are triggered only upon entering a specific Room.*

### AAAK: The Compression Audit
**AAAK (Asynchronous Agent Knowledge)** is a custom dialect for LLM consumption. 
* **Technical Audit:** AAAK is **lossy**. It shortens entities (e.g., "Milla Jovovich" to "MLJ") and strips nuance.
* **Accuracy:** Results in a **12.4% accuracy drop** compared to raw text. 
* **Recommendation:** Use **Raw Mode** for mission-critical precision (96.6% accuracy).

---

## 4. Performance Audit: The "Hype vs. Reality" Deep Dive

### The Benchmark Integrity Report
An engineering audit exposes manual interventions used to inflate metrics:

* **The LongMemEval "Cheat":** The 100% score was an Integrity Breach. Manual overrides and hardcoded patches were detected for 3 failed questions. **Adjusted Real Score: 60.3%.**
* **The LoCoMo "Retrieval Bypass":** Used "Pool Exhaustion" (top_k=50 on a dataset of 19–32 conversations), bypassing the retrieval engine entirely.
* **The AAAK Penalty:** Use of the lossy AAAK sieve degrades performance to **84.2%**.

### Audit Summary: Public Claims vs. Validated Results

| Metric | The Hype (Public Claim) | The Audit (Validated) |
| :--- | :--- | :--- |
| **LongMemEval (Hybrid + Rerank)** | 100% | **60.3%** |
| **AAAK Reliability** | "Lossless" | **Lossy (12.4% Drop)** |
| **Retrieval Accuracy (LoCoMo)** | 100% | **Bypassed (K > Dataset)** |
| **AAAK Mode Accuracy** | N/A | **84.2%** |
| **Raw Mode Accuracy** | 96.6% | **96.6% (Confirmed)** |

---

## 5. Implementation Principles & Core Takeaways

MemPalace originated from a "Vibe Coding" session with **Milla Jovovich** (Architect) and **Ben Sigman** (Engineer) using the agent **"Lu"** (Claude Code-driven).

### The Three Core Pillars
1.  **Verbatim Wins:** Keep the original context. Summarization is a lossy sieve.
2.  **Local is Power:** Infinite memory costs $0 with local stacks (**ChromaDB/SQLite**). Ensures privacy.
3.  **Architecture > Hype:** Trust transparent, verbatim data structures over curated benchmarks.

### Quick-Start Technical Stack
* **Language:** Python 3.9+
* **Storage:** ChromaDB (Vectors) & SQLite (Knowledge Graph).
* **Integration:** **MCP Server** (Model Context Protocol) with 29 specific tools for memory management.

> **Closing Mantra:** AI shouldn't decide what matters to you. You are the architect of your own memory.

---

## 6. Technical References & External Documentation

### Official Project & Background
* [**GitHub: MemPalace Repository**](https://github.com/MemPalace/mempalace): Official open-source repository and code base.
* [**Project announcement**](https://mempalaceofficial.com): Official Doc.

### Technical Deep-Dives
* [**Recca0120’s Blog: 170 Tokens to Recall Everything**](https://recca0120.github.io/en/2026/04/08/mempalace-ai-memory-system/): Breakdown of the L0/L1 token hierarchy and spatial structures. *(Updated to active GitHub Pages link)*
* ~~[**Medium: Romko Kozak - MemPalace in the Wild**](https://medium.com/@romko.kozak/mempalace-in-the-wild-resident-memory-and-the-death-of-context-limits-00f73587e954): Practical analysis of Knowledge Graphs and privacy.~~ *(Link currently unavailable/removed)*

### Critical Audits & Community Sanity Checks
* [**Vectorize: MemPalace Benchmarks Debunked**](https://vectorize.io/articles/mempalace-benchmarks): Engineering audit of the 100% success claims. *(Updated to active URL)*
* [**Reddit r/LocalLLaMA: Sanity Check Discussion**](https://www.reddit.com/r/LocalLLaMA/comments/1si5lc4/sanity_check_on_milla_jovovichs_mempalace_mixed/): Community discussion regarding "Lu," Claude Code, and benchmark overfitting. *(Updated to correct active thread)*
