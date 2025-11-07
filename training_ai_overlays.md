# NIST AI System Security Overlays Concept

Artificial intelligence (AI) systems introduce unique security and privacy
risks.  They include training data, models and deployment pipelines that
traditional security frameworks do not fully address.  NIST’s concept paper
on **AI system security overlays** proposes adapting the SP 800‑53 control
catalog to the AI domain【471044666484204†L1-L55】.

## What are control overlays?

SP 800‑53 provides a baseline of security and privacy controls for
information systems.  An **overlay** customizes this baseline for a
specific use case or technology.  For AI systems, overlays would tailor
controls and set appropriate parameter values to address risks such as
training‑data poisoning, model theft or misuse of generative models【471044666484204†L176-L184】.

## Proposed overlays

The concept paper outlines several possible overlays:

* **Generative AI systems** – models that create new content, such as text
  or images.
* **Predictive AI systems** – models that make decisions or recommendations.
* **Single‑agent or multi‑agent systems** – autonomous systems with one or
  multiple AI agents.
* **AI developer controls** – guidance for the development and deployment
  environment【471044666484204†L176-L184】.

Each overlay would modify the base controls, identify new controls where
necessary and establish organization‑defined parameters.  For example,
controls might require stricter data provenance checks, model integrity
validation or limits on model outputs to prevent disclosure of sensitive
training data.

## Why it matters

Organizations already familiar with SP 800‑53 can adapt their existing
processes rather than starting from scratch.  By developing overlays,
NIST aims to provide clear, implementation‑oriented guidance that protects
AI components while maintaining confidentiality, integrity and availability.
The concept paper invites the community to comment and help shape these
future guidelines【471044666484204†L1-L55】.
