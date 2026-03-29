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
Flavor Gourmet — Attempt 2

Flavor Gourmet Attempt 2 is the second modeling experiment within the OBA framework focusing on the gustatory modality. The core goal of this version is to test whether a taste system can spontaneously generate stable intermediate state structures (gustatory intermediate states) purely from low‑level physical–chemical inputs—completely excluding subjectivity, preference, or semantic labels.

Attempt 2 explicitly addresses the issue in the first attempt, where subjectivity and evaluative mechanisms were introduced too early, by strictly adhering to these principles:

    Inputs contain only continuous, low‑level physical–chemical features (ion concentration, osmotic pressure, molecular‑scale properties, etc.).

    No use of any taste categories (such as sweet, bitter, umami) or human semantics.

    No reward, preference, or decision mechanisms are included.

    Taste is treated as a passive physical field rather than an active selection process.

Structurally, Attempt 2 adopts a multi‑stage pipeline isomorphic to other perceptual modules in OBA (e.g., Odor K9, Light Sommelier):

Combinatorial Gustatory Receptor Field
Physical inputs are projected through random, overlapping receptor weights to form a sparse combinatorial code.

Low‑Dimensional Competitive Integration Dynamics
Receptor activations enter a low‑dimensional integration layer with lateral inhibition (mitral‑like dynamics, with olfactory naming removed), producing stable yet non‑trivial intermediate states over time.

Gustatory Field Descriptor
The integrated states are expressed as a continuous gustatory field (intensity, dispersion, tension, etc.), used only for structural analysis and not for evaluation.

Stability Bias & Energy Modulation
The field structure can be mapped to stability‑bias parameters; external energy states modulate trajectory morphology without altering the final attractor structure.

Trajectory‑Based Maturity Metric
A preference‑independent maturity metric quantifies whether the perceptual process has fully converged.

Experimental results show that under the current parameters and architecture, Flavor Gourmet Attempt 2 forms a continuous, stable, single‑attractor gustatory manifold:

    The “content structure” of taste is determined by physical inputs and competitive dynamics.

    Energy states affect the formation trajectory but not the final structure.

    Maturity reflects the completeness of the process, not any value judgment.

Therefore, Attempt 2 serves as a clean, encapsulated, and cross‑modally alignable gustatory submodule within OBA. Its outputs (field / stability bias / maturity) can be used by higher‑level systems, while it itself performs no subjective or decision‑making functions.

License / Use
This code is provided for research, analysis, and conceptual exploration.
No claims are made about biological fidelity beyond the stated abstraction level.
