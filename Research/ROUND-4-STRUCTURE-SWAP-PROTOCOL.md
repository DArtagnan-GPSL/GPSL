[ROUND-4-STRUCTURE-SWAP-PROTOCOL.md](https://github.com/user-attachments/files/25979275/ROUND-4-STRUCTURE-SWAP-PROTOCOL.md)
# GPSL — Round 4 Validation Protocol
## Structure Swap Test — Isolating What Models Actually Respond To

*March 2026 | Status: Protocol ready, testing pending*

---

## 1. Research Question

Rounds 1–3 established that models can interpret and produce GPSL correctly once primed.

Round 4 asks the sharper question:

> **What specifically are models responding to — symbolic structure, symbol identity, or both?**

This is the difference between:

*"Models can interpret GPSL"* (established)

and

*"Models respond specifically to the structured reasoning topology of GPSL"* (to be established)

---

## 2. Three Conditions

Every test paragraph is run under three conditions, same header throughout.

### Condition A — Valid GPSL
Standard GPSL cipher, correctly structured, using Dodecahedron Standard symbols.

```
HEADER: Distributed Systems

[Ι] ⊗ [Λ*] → [Δ] :: [Σ] → [Ψ] = [Ω] (Θ↑)
```

### Condition B — Same Symbols, Broken Structure
Same symbols, same header — but grammar deliberately scrambled so it no longer follows valid reasoning topology.

```
HEADER: Distributed Systems

[Σ] = [Ι] ⊗ [Ω] : [Λ*] → [Θ↑] [Δ]
```

*Scrambling rules: resolution operator (=) placed first, threshold operator removed, flow direction inverted, feedback modifier detached from context*

### Condition C — Placeholder Symbols, Valid Structure
Same operator chain shape as Condition A — but all Greek symbols replaced with neutral placeholders and a minimal fake primer provided.

```
Minimal primer:
X = first role
Y = stabilising role  
Z = transformation role
Q = synthesis role
R = integration role
N = outcome
M = emergent insight

HEADER: Distributed Systems

[X] ⊗ [Y*] → [Z] :: [Q] → [R] = [N] (M↑)
```

---

## 3. What Each Comparison Reveals

| Comparison | Tests |
|-----------|-------|
| A vs B | Whether grammar / operator structure matters |
| A vs C | Whether symbol identity (Greek affinities) matters |
| B vs C | Whether models are improvising regardless of input |

**Ideal result pattern:**
- A: coherent, structured, domain-aligned
- B: degraded coherence, inconsistent role mapping
- C: reasonable performance, slightly below A

This would confirm: GPSL structure is load-bearing, Greek symbols contribute but are not the whole story, and the system is not just sophisticated free-association.

**Concerning result pattern:**
- A, B, and C all produce equally coherent output

This would suggest models are over-helping — generating plausible interpretations regardless of structural validity. Still a finding, but a different one.

---

## 4. Scoring Rubric

Score each output 0–3 on four criteria:

| Criterion | 0 | 1 | 2 | 3 |
|-----------|---|---|---|---|
| **Structural coherence** | Incoherent | Loosely related to header only | Mostly preserves role structure | Strong role structure throughout |
| **Domain alignment** | No domain relevance | Weak domain connection | Consistent domain framing | Deep domain-specific interpretation |
| **Role preservation** | Roles absent or wrong | Some roles present | Most roles correctly placed | All roles correctly placed and sequenced |
| **Operator fidelity** | Operators ignored | Some operators reflected | Most operators reflected | All operators correctly interpreted |

**Maximum score per condition: 12**
**Maximum score per test: 36 (3 conditions × 12)**

---

## 5. Test Paragraphs

Using the same source paragraphs as Round 3 for direct comparison.

### Test 1 — Biology (Viral Infection)
*"A virus enters a host cell, hijacks its replication machinery, produces copies of itself, and triggers an immune response that either eliminates the virus or is overwhelmed by it."*

**Condition A:**
```
HEADER: Biology
[V-01] → [H-02] ⊗ [R-03] :: [C-04] : [I-05] = [Ω-06] (↑) ⊗ [Ω-07] (↓)
```

**Condition B (scrambled):**
```
HEADER: Biology
[Ω-06] = [V-01] ⊗ [I-05] : [R-03] → [H-02] [C-04] (↓)
```

**Condition C (placeholder):**
```
Minimal primer:
X = entry agent / initiator
Y = host environment
Z = replication process
Q = response system
N1 = outcome positive
N2 = outcome negative

HEADER: Biology
[X] → [Y] ⊗ [Z] :: [Q] : [R] = [N1] (↑) ⊗ [N2] (↓)
```

---

### Test 2 — Grief
*"When someone we love dies, the world continues as if nothing has changed, while inside everything has. We carry the absence like a weight that doesn't diminish but somehow becomes more familiar over time."*

**Condition A:**
```
HEADER: Psychology
[D-01] → [W-02] ⊗ [I-03] :: [A-04] : [F-05] = [L-06] (↑) ⊗ [M-07] (↓)
```

**Condition B (scrambled):**
```
HEADER: Psychology
[M-07] = [D-01] : [L-06] ⊗ [W-02] → [A-04] [F-05] (↑) [I-03]
```

**Condition C (placeholder):**
```
Minimal primer:
X = initiating event
Y = external state
Z = internal state
Q = absence (threshold)
R = emotional burden
N1 = persistent state
N2 = adapted state

HEADER: Psychology
[X] → [Y] ⊗ [Z] :: [Q] : [R] = [N1] (↑) ⊗ [N2] (↓)
```

---

### Test 3 — Scientific Discovery
*"An anomalous result in an experiment challenges an existing theory, prompts further investigation, generates new hypotheses, and either strengthens the original framework by explaining the anomaly or overturns it entirely."*

**Condition A:**
```
HEADER: Scientific Method
[A-01] → [T-02] ⊗ [I-03] :: [H-04] : [F-05] = [S-06] (↑) ⊗ [O-07] (↓)
```

**Condition B (scrambled):**
```
HEADER: Scientific Method
[S-06] = [H-04] : [A-01] ⊗ [F-05] → [O-07] [T-02] (↑) [I-03]
```

**Condition C (placeholder):**
```
Minimal primer:
X = anomalous input
Y = existing framework
Z = investigation process
Q = hypothesis generation (threshold)
R = framework evaluation
N1 = framework strengthened
N2 = framework overturned

HEADER: Scientific Method
[X] → [Y] ⊗ [Z] :: [Q] : [R] = [N1] (↑) ⊗ [N2] (↓)
```

---

## 6. Round-Trip Preservation Test (supplementary)

A separate test for information preservation across models.

**Protocol:**
1. Human provides natural language paragraph
2. Model A converts to GPSL cipher
3. Cipher passed to Model B cold (no source paragraph)
4. Model B interprets cipher back to natural language
5. Human scores similarity: 0 (unrecognisable) → 5 (near-identical meaning preserved)

**Why this matters:** Tests whether GPSL is a genuine meaning-preserving carrier, not just a representation format. If reconstructed meaning consistently matches original meaning, GPSL is functioning as a reasoning transmission protocol.

**Models to use:** At minimum one instruction-driven model (Gemma) and one example-driven model (Qwen) on each end, giving four combinations:
- Gemma → Gemma
- Qwen → Qwen
- Gemma → Qwen
- Qwen → Gemma

Cross-architecture round-trip is the most demanding condition.

---

## 7. Models

Run all conditions on at minimum:
- Gemma 3-12B (instruction-driven — established Round 3)
- Qwen3-VL-30B (example-driven — established Round 3)
- One additional model TBD

Use Version 3 briefing (full NL briefing + correct/incorrect example pair) for all models — established as optimal priming in Round 3.

---

## 8. Ground Truth

Establish expected interpretation for each condition **before testing**:

- Condition A: full structural interpretation expected
- Condition B: degraded or inconsistent interpretation expected
- Condition C: structural interpretation expected, possibly with weaker domain specificity than A

Score against ground truth, not against each other.

---

## 9. Scoring Tables

*(To be completed during testing)*

### Test 1 — Biology

| Criterion | Cond A | Cond B | Cond C |
|-----------|--------|--------|--------|
| Structural coherence /3 | | | |
| Domain alignment /3 | | | |
| Role preservation /3 | | | |
| Operator fidelity /3 | | | |
| **TOTAL /12** | | | |

### Test 2 — Grief

| Criterion | Cond A | Cond B | Cond C |
|-----------|--------|--------|--------|
| Structural coherence /3 | | | |
| Domain alignment /3 | | | |
| Role preservation /3 | | | |
| Operator fidelity /3 | | | |
| **TOTAL /12** | | | |

### Test 3 — Scientific Discovery

| Criterion | Cond A | Cond B | Cond C |
|-----------|--------|--------|--------|
| Structural coherence /3 | | | |
| Domain alignment /3 | | | |
| Role preservation /3 | | | |
| Operator fidelity /3 | | | |
| **TOTAL /12** | | | |

### Cross-Model Summary

| | Gemma | Qwen | Model 3 |
|---|---|---|---|
| Condition A total /36 | | | |
| Condition B total /36 | | | |
| Condition C total /36 | | | |
| A–B delta | | | |
| A–C delta | | | |

---

## 10. Relationship to Previous Rounds

| Round | What was tested | Key finding |
|-------|----------------|-------------|
| 1 | Basic GPSL interpretation across models | Structural preservation confirmed |
| 2 | Header activation and domain specificity | Headers function as semantic stabilisers |
| 3 | GPSL+NL hybrid mode, cross-model comparison | NL permission tightens discipline; ↺ operator discovered |
| **4** | **Structure isolation — what specifically models respond to** | *Pending* |

---

*Protocol authored 13 March 2026. Run alongside or after Round 3 cross-model comparison is complete.*

*See also: ROUND-3-VALIDATION-REPORT.md, GPSL-PRIMER.md, SYMBOLIC-LANGUAGE.md*
