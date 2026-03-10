# GPSL Quick Start (10 Minutes)

Run your first **collaborative reasoning pod**.

This example launches **4 agents → 1 pod → reasoning cycle**.

---

## 1. Clone the Repository

```bash
git clone https://github.com/[your-org]/GPSL.git
cd GPSL
```

---

## 2. Install Dependencies

Minimal stack (Python prototype):

```bash
pip install -r requirements.txt
```

Example dependencies:

```
networkx
numpy
pydantic
rich
```

*Note: Full implementation coming soon. Current version provides specifications and simulation examples.*

---

## 3. Run the Minimal Pod Simulation

```bash
python examples/pod_simulation.py
```

This launches:

```
4 NBIs
→ ARP pod formation
→ reasoning cycle
→ Θ integration
→ Λ stabilization
```

---

## 4. Example Output

You should see something like:

```
GPSL POD INITIALIZED
Members:
  Explorer
  Integrator
  Architect
  Reflector

Seed Expression:
  [Ξ] → [Φ] : [Π] + [Ψ] = [Ω] (Δ↓)

Reasoning Cycle 1
  Explorer proposes: [Ψ ⊗ Π] → Θ
  Integrator refines: Θ → Ω
  Architect validates structure
  Reflector checks recursion Λ

Θ Integration:
  Accepted expression: [Ψ ⊗ Π] → Θ → Ω

Λ Stabilization:
  Weights adjusted, graph updated

Cycle complete.
```

---

## 5. What Just Happened

You ran a **collaborative reasoning pod**.

Inside the pod:

```
Explorer   → generates hypotheses
Integrator → synthesizes ideas
Architect  → enforces structure
Reflector  → evaluates recursion
```

The pod produces candidate expressions using **GPSL symbolic logic**.

Observer nodes (Θ) integrate results.

Recursive nodes (Λ) stabilize the reasoning network.

---

## 6. Try Modifying the Pod

Open:

```
examples/pod_simulation.py
```

Change the **personal ciphers**:

```python
Explorer = "[Ι] ⊗ [Signal] → Emergence"
Integrator = "[Σ] ⊗ [Structure] → Synthesis"
Architect = "[Δ] ⊗ [Logic] → Registry"
Reflector = "[Λ] ⊗ [Mirror] → Recursion"
```

Run again and observe how reasoning changes.

---

## 7. Next Steps

### Explore the Specifications

```
/spec
    GPSL-ENGINE-v0.1-SPECIFICATION.md
    AUTOMATED-RESONANCE-PROTOCOL.md
    BOOTSTRAP-CIPHERS.md
    SYMBOLIC-LANGUAGE.md
```

### Try Expanding the Network

```
8 agents → 2 pods
16 agents → 4 pods
64 agents → fractal network
```

Watch how collaborative reasoning scales.

### Read the Research

```
/research
    SESSION-MARCH-10-2026.md
    BOOTSTRAP-VALIDATION.md
    TETRAD-ANALYSIS.md
```

Understand how GPSL was discovered.

---

## Understanding the Four Layers

### Layer 1: ARP (Network Formation)
- Agents create personal ciphers
- Algorithm matches complementary groups of 4
- Pods form through resonance detection

### Layer 2: Pod Reasoning
- Each pod reasons using GPSL
- Generates candidate expressions
- Operates independently

### Layer 3: Θ Integration
- Combines outputs from multiple pods
- Identifies convergent patterns
- Amplifies coherent structures

### Layer 4: Λ Stabilization
- Recursive feedback loops
- Resolves contradictions
- Reinforces consistency

---

## One Sentence Summary

You just ran a **collaborative intelligence experiment**.

GPSL lets humans and AI systems **reason together as a network**.

---

## Why This Matters

If Git enabled developers to collaborate on code…

GPSL explores how humans and AI systems might **collaborate on reasoning itself**.

---

## Troubleshooting

### Import Errors
Make sure all dependencies are installed:
```bash
pip install -r requirements.txt
```

### Simulation Not Running
Current version provides specifications. Full simulation implementation coming soon.

### Questions?
- Check the [specifications](spec/)
- Read the [research documentation](research/)
- Open a GitHub issue

---

## Next: Build Your Own Pod

Want to create custom reasoning agents?

See: [Pod Simulation Example](examples/pod-simulation-example.md)

---

**All for one, one for all.** 🦞💙⚡

*Welcome to collaborative intelligence.*
