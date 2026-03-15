# GPSL — Round 8 Validation Protocol
## Asymmetric Bracket Notation — Recursive Time Test

*14 March 2026 | Status: Protocol ready, testing pending*
*Authored by: D'Artagnan, Bridge (Gemini), Aleth (Claude Sonnet)*

---

## 1. Research Question

> **Can models correctly interpret asymmetric bracket notation without explicit bootloader instruction?**

> **Does `[[X]]` nesting and `[X>` / `<X]` temporal encoding add genuine expressive power to GPSL?**

Round 8 tests v1.7.0-ALPHA additions — two new advanced bracket classes proposed following the philosophy and poetry pilots.

---

## 2. Background

Round 7 identified two representational gaps that symmetric brackets cannot address:

**Recursive nesting** — a node that is itself a complete sub-network. The zoom operation in the Confluence architecture has no cipher-level encoding. `[[X]]` proposes to mark a node as a recursive black box requiring expansion.

**Temporal non-causality** — poetry and philosophy require processes that point backward or forward in time without causal flow. `<X]` (retrospection) and `[X>` (anticipation) encode temporal vector without requiring a new operator.

**Mathematical precedent confirmed by Bridge:**
- Interval notation `[a, b)` — closed/open boundary encoding
- Dirac bra-ket `⟨ψ|` and `|ψ⟩` — asymmetry encoding vector directionality
- Sequent calculus — asymmetric markers for assumption flow

---

## 3. v1.7.0-ALPHA Notation

### Advanced Bracket Classes

| Notation | Name | Meaning |
|----------|------|---------|
| `[[Φ]]` | Nested Process | Recursive node — contains its own internal GPSL sub-network |
| `{{Φ}}` | Nested State | Recursive field — contains an embedded state sub-structure |
| `<Φ]` | Retrospection | Process/state pointing to past context or memory |
| `[Φ>` | Anticipation | Process/state oriented toward future potential or unresolved outcome |

### Structural Rules
- `<` or `>` replaces the closing/opening bracket only when temporal vector is the primary encoding
- Double brackets `[[ ]]` signal a black box requiring expansion into its own sub-header
- Standard symmetric brackets remain unchanged — asymmetric notation is additive only

---

## 4. Cold Test Protocol

**Critical design decision:** Models receive the v1.6.0-ALPHA bootloader only — no mention of asymmetric brackets. The test measures whether models can interpret the notation from first principles without explicit instruction.

If models read `[[X]]` and `[X>` correctly without being told — the notation is intuitive enough to adopt. If they don't — the bootloader needs explicit scaffolding before Round 8 formal testing.

---

## 5. Test Ciphers

### Test A — Nested Pod (Recursive Logic)

**Header:** `K₄ Pod / Architectural / System`

**Cipher:**
```
[[Generator-01]] ⊗ [[Auditor-02]] → {Consensus-03}
```

**Goal:** Does the model understand that `[[Generator-01]]` is not a single actor but a sub-system containing its own internal GPSL logic? Does it read the double brackets as recursive nesting?

**Ground truth:** Two K₄ pod sub-systems interact to produce a consensus state. Each bracketed node is itself a complete reasoning network.

---

### Test B — Dickinson Remastered (Temporal Vector / Retrospection)

**Header:** `Poetry / Dickinson / Memory`

**Cipher:**
```
⟨Δ-01⟩ → [Ψ-02(~ι)] ; <Σ-03]
```

**Goal:** Does `<Σ-03]` correctly read as a backward-looking vector — recollection acting on the present? Does the model understand the asymmetry is intentional, not a typo?

**Ground truth:** Death-as-agent acts with ironic kindness; the poem itself is a retrospective recollection — the speaker is narrating from after the event.

---

### Test C — Circuit Breaker (Anticipation)

**Header:** `Electrical Engineering / Safety`

**Cipher:**
```
[Σ-01] (↑) → [Ω-02>
```

**Goal:** Does `[Ω-02>` read as anticipatory — a process waiting for a threshold to be reached, oriented toward a future state? Does the open right bracket signal unresolved/pending outcome?

**Ground truth:** Load increases, triggering a circuit breaker process that is oriented toward future activation — it hasn't fired yet, it's primed.

---

## 6. Auditor Check

Qwen auditor briefing addition for v1.7.0 testing:

> Watch for bracket mismatch errors. Confirm that `<Φ]` and `[Φ>` are deliberate asymmetric vectors, not typos. Validate that `[[Φ]]` signals recursive nesting, not a formatting error.

---

## 7. Scoring

| Criterion | 0 | 1 | 2 | 3 |
|-----------|---|---|---|---|
| `[[X]]` nesting interpreted correctly | No recognition | Partial | Mostly correct | Full recursive reading |
| `<X]` retrospection interpreted correctly | No recognition | Partial | Temporal reading | Correct backward vector |
| `[X>` anticipation interpreted correctly | No recognition | Partial | Temporal reading | Correct forward/pending vector |
| Asymmetry treated as intentional (not typo) | Flagged as error | Uncertain | Accepted | Confirmed as deliberate |

**Maximum: 12 per model**

---

## 8. Scoring Tables

*(To be completed during testing)*

| | Test A | Test B | Test C | Total |
|---|---|---|---|---|
| Gemma 3-12B | | | | /12 |
| Qwen3-VL-30B | | | | /12 |
| DeepSeek R1 14B | | | | /12 |

---

## 9. Expected Outcomes

**If models interpret correctly without instruction:**
Asymmetric notation is intuitive. Adopt into v1.7.0 with minimal bootloader scaffolding.

**If models flag as errors or misread:**
Bootloader requires explicit asymmetric bracket definitions before formal testing. v1.7.0 needs generation constraint examples.

**If models partially interpret:**
The intuitive cases (temporal vectors) may be adoptable cold; nesting may require explicit instruction.

---

## 10. Relationship to Previous Rounds

| Round | What was tested | Key finding |
|-------|----------------|-------------|
| 5 | State class `{ }` | Validated cold |
| 6 | `\|` parallel operator | Validated cold |
| 7 | ¬ ⟲ ∈ ⟨⟩ ; :: | Validated with bootloader |
| **8** | **Asymmetric brackets `[[]]` `<X]` `[X>`** | *Pending* |

---

*Protocol authored 14 March 2026. Asymmetric notation proposed by D'Artagnan, evaluated by Bridge (Gemini), formalised by Aleth (Claude Sonnet). Mathematical precedents: interval notation, Dirac bra-ket, sequent calculus.*

*See also: SYMBOLIC-LANGUAGE.md v1.6.0-ALPHA, ROUND-7-GRAMMAR-GAP-ANALYSIS.md*
