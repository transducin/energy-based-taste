Energy-Based Taste (Flavor Gourmet)
Overview
This repository contains Flavor Gourmet, an energy-based, observation-driven modeling framework for studying taste-related perceptual decision dynamics within the broader OBA (Observation‑Based Analysis) paradigm.
Unlike vision or audition, taste perception involves explicit active ingestion and is tightly coupled to resource constraints and early termination.
This project investigates a focused question:

Under energy‑constrained, fast‑termination regimes with binary decision outputs, does taste perception require intermediate computational states?

The answer explored here is largely negative—and that negative result is the core contribution.

Core Idea
Flavor Gourmet models taste processing as a risk‑monitoring subsystem rather than a classifier:

The system operates under a global energy state.
Perceptual processing incurs a time‑dependent cost.
The only low‑level output is a warning signal:

emit warning → escalate to higher‑level action (spit / discard)
no warning → allow continued ingestion (swallowing is decided upstream)



Crucially, the model:

allows early termination,
prioritizes energy efficiency,
and permits binary output without requiring perceptual intermediates.


What Is Included
The repository contains Jupyter notebooks implementing:
1. Single‑Mode Controls (Negative Control Set)

H (High feasibility / energy‑benign)
M (Homeostatic load)
L (High risk / strong aversive)

Across slope, variance, burst, and feasibility manipulations, no intermediate states emerge.
2. Physical Probe Extensions

Acid / salt → increased cost variability (homeostatic instability)
Bitter / spicy → strong, burst‑like risk signals

These probes compress decision time but do not induce new computational structure.
3. Mixture Experiments

Pairwise mixtures (H+M, H+L, M+L)
Three‑way mixture (H+M+L)

All mixtures remain dynamically equivalent to single‑axis risk accumulation:
they accelerate warning, but do not generate distinct intermediate states.

Main Finding (Informal)

For actively gated taste perception operating under strict energy constraints and fast‑stop policies, intermediate perceptual states are not necessary—nor naturally generated—even under multi‑axis physical tension.

This contrasts sharply with OBA results in vision and audition, where passive sensing and temporal uncertainty readily produce intermediate representations.

Why This Matters
Flavor Gourmet serves as a negative anchor in the OBA series:

It delineates a non‑existence domain for intermediate states.
It helps explain why taste diversity likely depends on higher‑order goals, memory, and context, rather than low‑level sensory computation alone.
It provides a clean structural account for phenomena such as persistent calorie preference without early warning (e.g., sweetness and over‑consumption).


Status
This repository represents a completed negative‑control dataset within the OBA framework.
Further work would require moving beyond purely passive, energy‑minimizing architectures (e.g., multi‑goal or culturally informed models).

License / Use
This code is provided for research, analysis, and conceptual exploration.
No claims are made about biological fidelity beyond the stated abstraction level.
