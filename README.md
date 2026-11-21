# Research Agenda (2027 Goals)

My research studies how the geometry and topology of learned representations change during training, which distinctions remain recoverable, and how those changes relate to model behavior. 
In 2027, I plan to connect controlled point-cloud experiments, efficient temporal computation, and the evaluation of language model safety into a focused research program.

I approach these questions as an experimental mathematician: construct examples with known structure, compute how candidate measurements respond, investigate counterexamples, and use the results to refine definitions and formulate conjectures. 
This direction builds on my doctoral work in knowledge graph and language representation alignment through optimal transport. 
My experience building machine learning systems in industry continues to shape my attention to computational cost, reproducibility, and practical interpretation.

The overarching question I plan to investigate in 2027 is 

>When do changes in the topology of labeled representations reveal consequential changes that simpler measurements miss, and how reliably can we monitor them?

This is especially relevant in the context of safe/unsafe responses from open-weight models.

## Hierarchical representation structure and safety

My main empirical priority is the ongoing work on representations organized by a safety taxonomy. 
This follows fixed prompts through selected layers and fine-tuning checkpoints, studying child categories, their parents, and their broader domains.
Inclusion-induced homology maps let us ask how a child's structure is retained in its parent and domain, where that structure becomes trivial, and whether different children increasingly share the same homological directions. 
These relationships provide information beyond separate persistence diagrams for each category.

The prompt safety taxonomy is the reference for the labeled relations being studied. 
Separate behavioral evaluations assess harmful compliance, excessive refusal, and retained task utility. 
I want to establish whether the hierarchy measurements are reproducible, whether they add information beyond spectral, geometric, and ordinary topological controls, and whether they help anticipate later behavioral changes on independent runs.

## Calibration and controlled structural change

I plan to extend the connection between EvolveManifold and calibrated persistent-homology testing. 
Priorities include stronger comparisons with effective rank, measures of spread, neighborhood structure, and distributional diagnostics.
Sensitivity to sample size and noise and controls that separate scale changes from the structural changes of interest come later.
Particularly useful experiments include constructions with similar covariance spectra or radii but different topological organization, and comparisons between meaningful labels and size-preserving shuffled assignments. 
These can clarify what a measurement contributes before interpreting its behavior in a neural model.
For repeated monitoring, I will carry calibration through the full trajectory and assess alert rules on independent control runs. 
Comparisons will use matched false-alarm rates. 
The intended outcome is a more defensible mechanism map describing when topology helps, when simpler measurements suffice, and how much uncertainty remains.

## Efficient and prospective temporal monitoring

The next computational step is to measure the fidelity and total cost of temporal monitoring. 
I plan to compare local maintenance, landmark methods, sparse complexes, fixed checkpoint schedules, and event-driven recomputation. 
Evaluation will include representation extraction, neighborhood construction, runtime, memory, and agreement with reference computations.
For the MMHM application, priorities include independent checks against fresh reductions and sensitivity analyses for matching choices and representative cycles. 
Maintenance activity is itself a candidate measurement whose interpretation needs to be tested.
Prospective evaluation will use information available up to each checkpoint, with alert thresholds and prediction horizons fixed before the corresponding held-out runs are examined. 
I will assess detection, false alerts, missed changes, and computational overhead together.

