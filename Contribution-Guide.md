# **Contributing to Iterative Reasoning Graphs (IRG)**

Thank you for your interest in contributing to **Iterative Reasoning Graphs (IRG)**.

IRG is a protocol, not a product. Contributions are welcome, but changes should preserve the protocol’s core goals: **persistence, structure, executability, and iterability**.

This document explains **what kinds of contributions are useful**, **how to propose them**, and **how decisions are made**.

---

## **Guiding Principles for Contributions**

Good IRG contributions are:

* **Specific** — tied to a concrete ambiguity or architectural gap
* **Structural** — improve reasoning representation, not just implementation details
* **Protocol-focused** — avoid implementation-specific assumptions
* **Backward-aware** — consider impact on compliance and interoperability across versions

IRG favors **clarity over cleverness** and **architectural integrity over optimization hacks**.

---

## **What to Contribute**

We actively welcome contributions in the following areas.

### **1\. Protocol Improvements**

Suggestions to:

* clarify definitions
* tighten scope boundaries
* refine compliance requirements
* improve node and edge contracts
* resolve ambiguities that affect reproducibility or interoperability

**Best format:**

*Problem → Ambiguity or gap → Proposed change → Tradeoffs introduced*

---

### **2\. Schema Proposals**

Proposals to:

* refine node type definitions
* clarify edge semantics
* propose additional node types for specific reasoning patterns
* improve schema expressiveness while maintaining simplicity

All additions should clearly state:

* which reasoning pattern(s) they support
* what architectural gap they address
* why existing node types do not already capture it
* impact on minimal compliance requirements

---

### **3\. Iteration Cycle Refinements**

High-value contributions include:

* clarifications to the canonical IRG Iteration Cycle (IIC)
* examples of convergence criteria
* termination condition patterns
* stability and drift detection strategies

Concrete examples reduce implementation ambiguity and improve protocol adherence.

---

### **4\. Implementation Examples**

Proposals related to:

* reference implementations (clearly labeled non-normative)
* integration patterns with generative models
* memory system interfaces
* visualization and debugging approaches
* trace export formats

IRG does **not** prescribe implementation details, but examples must be clearly scoped and labeled as informative, not normative.

---

### **5\. Empirical Results and Case Studies**

We welcome:

* IRG implementations in real systems
* negative results
* surprising failure modes or limitations
* performance characteristics
* comparisons between IRG and non-IRG architectures

Publishing failures is encouraged.

---

## **What Not to Contribute**

To keep the protocol coherent, we generally do **not** accept:

* model architecture requirements
* training or prompting recipes
* implementation-specific optimizations without protocol justification
* proposals that treat IRG as a workflow engine or task orchestrator
* proposals that eliminate iteration, persistence, or graph structure
* alignment or safety prescriptions unrelated to reasoning structure

These may be valuable elsewhere, but fall outside IRG’s scope.

---

## **How to Propose Changes**

### **Step 1: Open an Issue**

Before submitting a pull request, open an issue describing:

* the problem you observed
* the section(s) affected
* why this matters for reasoning structure or protocol integrity
* any known tradeoffs

This allows discussion before committing to a design direction.

---

### **Step 2: Submit a Pull Request**

Pull requests should:

* be focused (one conceptual change per PR)
* reference the relevant issue
* include updated text *and* rationale
* avoid silent normative shifts

If your change affects compliance requirements or interoperability, call that out explicitly.

---

### **Step 3: Review and Discussion**

All substantive changes are reviewed for:

* clarity
* consistency with IRG principles
* impact on interoperability and compliance
* risk of scope creep or misuse

Disagreement is expected. Decisions aim for **reasoned consensus**, not unanimity.

---

## **Versioning and Backward Compatibility**

IRG follows semantic versioning principles:

* **v0.x** — exploratory, open to structural change
* **v1.0+** — stability prioritized

Breaking changes must:

* be explicitly labeled
* include migration notes
* preserve historical comparability where possible

Schema proposals and trace formats may be versioned independently from the core protocol.

---

## **Code of Conduct**

We expect contributors to:

* engage in good faith
* critique ideas, not people
* ground arguments in evidence or reasoning
* avoid rhetorical or adversarial framing

Reasoning discipline applies to the discussion itself.

---

## **Governance (Current)**

During the v0.x phase:

* Maintainers curate changes
* The protocol evolves through open critique
* No single organization controls usage or adoption

Governance will be revisited prior to v1.0.

---

## **Attribution**

All contributors will be acknowledged in the repository history.

Significant conceptual contributions may be credited explicitly in the specification.

---

## **Final Note**

IRG is intentionally narrow.

If your proposal adds complexity without improving reasoning structure, persistence, or auditability, it probably doesn’t belong here.

If it helps us answer — rigorously and repeatedly —

*“Can the system's reasoning be inspected, revised, and improved over time?”*

— then we want to hear it.
