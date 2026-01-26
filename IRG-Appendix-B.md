# **Appendix B — Frequently Asked Questions (FAQ)**

### **Q1: Why “Iterative”? Why not just “Reasoning Graph”?**

Iteration is not incidental—it is the core contribution.

IRGs are explicitly designed to:

* Revise prior reasoning  
* Incorporate critique  
* Track confidence over time  
* Converge (or fail) deliberately

Without iteration, the graph degenerates into a static plan or explanation artifact.

---

### **Q2: How is IRG different from tool orchestration frameworks?**

Most tool frameworks:

* Execute predefined workflows  
* Lack memory of *why* a step occurred  
* Do not revise prior steps

IRGs:

* Encode *intent*, *justification*, and *dependency*  
* Allow invalidation and supersession of prior reasoning  
* Treat reasoning steps as mutable, first-class objects

---

### **Q3: Does IRG slow inference?**

IRGs shift cost from **repeated generation** to **structured reuse**.

In practice:

* First-pass responses may be slightly slower  
* Subsequent revisions are significantly cheaper  
* Long-horizon tasks become more efficient

IRGs are particularly effective when correctness, auditability, or iteration depth matters.

---

### **Q4: Can IRGs be used with closed models like GPT or Claude?**

Yes, partially.

External models can:

* Draft nodes  
* Critique nodes  
* Propose revisions

---

### **Q5: Is exposing IRGs a safety risk?**

IRGs are safer to expose than raw chain-of-thought.

They:

* Avoid leaking latent model heuristics  
* Are explicitly authored and filtered  
* Can be policy-scoped and redacted

IRGs enable **controlled transparency**, not uncontrolled disclosure.

---

### **Q6: How does IRG relate to alignment and safety?**

IRGs enable **structural alignment**.

Instead of hoping a model behaves safely:

* Policies can be enforced at the node level  
* Certain node types can be required or forbidden  
* Risk assessment can be mandatory, not optional

This shifts alignment from *behavioral nudging* to *architectural constraint*.

---

### **Q7: What happens when an IRG fails to converge?**

Non-convergence is a first-class outcome.

IRGs can:

* Surface uncertainty explicitly  
* Request additional information  
* Terminate with a bounded failure state

This supports **epistemic humility** and reduces hallucination pressure.

---

### **Q8: Can IRGs be standardized across vendors?**

Yes—at the protocol level.

While internal model state may remain proprietary, IRG schemas, node types, and trace formats can be standardized without revealing model internals.

This mirrors how:

* HTTP standardized communication  
* Not server implementations  
* Not application logic

---

### **Q9: Why publish this as a protocol instead of a product?**

Protocols create ecosystems.

Products come and go.

Protocols define categories.

Publishing IRG as a protocol:

* Establishes prior art  
* Encourages third-party tooling  
* Prevents enclosure by proprietary implementations

Reference implementations remain competitive advantages.

---

### **Q10: What is the long-term vision for IRGs?**

IRGs are intended to become:

* The substrate for long-horizon cognition  
* A bridge between reasoning, memory, and action  
* A foundation for auditable, governable AI systems

They are not a feature.

They are **infrastructure**.

