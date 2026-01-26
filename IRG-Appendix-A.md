# **Appendix A — What IRG Is Not**

This appendix clarifies common misinterpretations of Iterative Reasoning Graphs (IRGs). These distinctions are intentional and architectural.

---

### **A.1 IRG Is Not Chain-of-Thought**

IRGs do **not** expose chain-of-thought.

* Chain-of-thought is:  
  * Linear  
  * Ephemeral  
  * Generated incidentally during inference  
  * Unsafe to expose verbatim

IRGs are:

* Graph-structured  
* Persistent across time  
* Explicitly authored and revised  
* Designed for inspection and audit

An IRG node is **not a transcript of internal deliberation**.

It is a **post-hoc, structured reasoning artifact** that governs future computation.

---

### **A.2 IRG Is Not a Prompting Technique**

IRGs are not:

* Prompt templates  
* Multi-shot prompts  
* System prompt hacks  
* Instruction chaining

While generative models may be invoked *within* IRG nodes, the IRG itself exists **outside the prompt boundary** and persists independently of any single inference call.

Removing the IRG while keeping prompts intact fundamentally changes system behavior.

---

### **A.3 IRG Is Not a Model Architecture**

IRGs do not prescribe:

* Attention mechanisms  
* Tokenization schemes  
* Training objectives  
* Weight layouts

They are **model-agnostic**.

An IRG can govern:

* Autoregressive transformers  
* Diffusion models  
* Hybrid symbolic–neural systems  
* Non-neural tools and simulators

The IRG operates at the **cognitive orchestration layer**, not the representation layer.

---

### **A.4 IRG Is Not Fine-Tuning**

IRGs do not modify model weights.

Instead of encoding knowledge or corrections into parameters, IRGs encode them into **explicit reasoning structure**.

This avoids:

* Global side effects  
* Catastrophic forgetting  
* Long retraining cycles

Corrections are local, interpretable, and reversible.

---

### **A.5 IRG Is Not Just a Log or Trace**

Logs record what happened.

IRGs determine **what will happen next**.

A reasoning trace without executability is observational.

An IRG is **interventional**.

---

### **A.6 IRG Is Not a Knowledge Graph**

While both are graph-based, their purposes differ:

| Knowledge Graph | Iterative Reasoning Graph |
| :---: | :---: |
| Stores facts | Stores reasoning processes |
| Mostly static | Actively evolving |
| Queried | Executed |
| Declarative | Procedural |

IRGs may *reference* knowledge graphs, but they do not replace them.

