# Iterative Reasoning Graphs (IRG)

**A protocol for persistent, executable, and auditable reasoning in AI systems.**

This repository contains the **authoritative specification** for **Iterative Reasoning Graphs (IRGs)**

IRG defines a **cognitive control layer** that externalizes reasoning as structured, iterable graph state — distinct from model weights, prompts, or transient inference traces.

This repository is **spec-first**. It is not a product, SDK, or reference implementation.

---

## Spec Links:
* [Protocol Spec](IRG-Protocol.md)
* [Appendix-A - What IRG Is Not](IRG-Appendix-A.md)
* [Appendix-B - FAQ](IRG-Appendix-B.md)
* [Contribution Guide](Contribution-Guide.md)

## What Is IRG?

An **Iterative Reasoning Graph (IRG)** is a first-class representation of reasoning as an evolving graph of executable nodes.

IRGs make reasoning:

- **Persistent** — survives beyond a single response
- **Structured** — explicit nodes and edges, not latent traces
- **Executable** — nodes represent actions, checks, or transformations
- **Iterative** — reasoning improves through revision cycles
- **Inspectable** — internal state is auditable and exportable

IRG is **not** a model, prompt, or workflow.  
It is an architectural substrate that governs *how* models are used.

---

## Repository Structure

```
irg-spec/
├── IRG-Protocol.md        # Core IRG protocol (normative)
├── IRG-Appendix-A.md      # What IRG Is Not
├── IRG-Appendix-B.md      # Frequently Asked Questions (FAQ)
├── Contribution-Guide.md  # How to contribute
├── LICENSE                # Creative Commons license (CC-BY)
└── README.md              # This file
```
### Normative vs Informative
- **IRG-protocol.md** is normative unless otherwise stated.
- Appendices may contain both normative clarifications and informative guidance.
- Examples are non-normative unless explicitly labeled.

---

## Design Philosophy

IRG is built on a small number of core principles:

- **Reasoning is structure, not text**
- **Iteration is a first-class primitive**
- **Correction should be local, not global**
- **Auditability should not require exposing chain-of-thought**
- **Protocols create ecosystems; products come later**

The protocol intentionally avoids prescribing:
- Model architectures
- Training methods
- Tooling stacks
- Optimization strategies

Interoperability is achieved through **shared structure**, not shared implementations.

---

## What IRG Is Not

IRG is **not**:
- Chain-of-thought
- A prompting technique
- A workflow engine
- A model architecture
- Fine-tuning
- A knowledge graph
- A logging format

Appendix A exists specifically to prevent category errors and misreadings.

---

## Compliance and Interoperability

A system **MAY** describe itself as *IRG-compliant* only if it satisfies the **Minimal IRG Compliance** requirements defined in the protocol.

Compliance is intentionally minimal:
- To preserve conceptual integrity
- To enable independent implementations
- To avoid premature standard lock-in

Future versions may introduce:
- Trace schemas
- Conformance tests
- Optional certification profiles

These will be versioned independently of the core protocol.

---

## Status

- **Protocol version:** v0.3 (Draft for Collaboration)
- **Stability:** Experimental but structurally complete
- **Change policy:** Breaking changes allowed until v1.0

This specification is being actively refined in public.

---

## How to Contribute

Contributions are welcome, especially:

- Clarifications of ambiguous language
- Tightening of normative requirements
- Additional examples (clearly labeled non-normative)
- Comparative analysis with related systems
- Schema proposals (clearly scoped)

Please:
1. Open an issue describing the concern or proposal
2. Reference specific sections or language
3. Avoid implementation-specific assumptions
4. Keep protocol vs example boundaries explicit

This repo is intentionally conservative about scope creep.

See **[Contribution-Guide.md](Contribution-Guide.md)** for details.

---

## Why This Exists

IRG exists because:
- Reasoning currently evaporates after each response
- Self-critique without structure does not converge
- Safety without inspectable cognition does not scale
- Alignment by prompt is not governance

IRG proposes a different axis:
**architecture instead of heuristics**.

---

## Contact / Discussion

For discussion, issues, or collaboration:
- Use GitHub Issues for protocol-related topics
- Reference exact sections when possible


---

## **License**

The Iterative Reasoning Graphs (IRG) specification is licensed under the Creative Commons Attribution 4.0 International License (CC BY 4.0).

You are free to:

* Share — copy and redistribute the material in any medium or format  
* Adapt — remix, transform, and build upon the material  
* Use for any purpose, including commercial use

Under the following terms:

* Attribution — You must give appropriate credit, provide a link to the license, and indicate if changes were made.

This license applies to the specification text only. Reference implementations, tooling, datasets, and certification programs may be licensed separately.

