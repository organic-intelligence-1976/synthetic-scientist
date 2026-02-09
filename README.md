# Simulating the Scientist's Dilemma: Training LLMs to Resolve Belief Conflicts

**Reza Jamei** — February 2026

## Abstract

Recent progress in training reasoning capabilities has relied heavily on domains with verifiable answers — mathematics and code — where correct final answers provide free supervision for thinking traces. But many forms of productive thinking, particularly *epistemic* reasoning (noticing that beliefs conflict, isolating assumptions, revising), lack such clean verification.

We propose a method for generating training data for epistemic recovery by manufacturing situations that are unsolved for a model instance while remaining gradeable for us. The core primitive is **deliberate confusion**: we temporarily fine-tune a model copy to hold a coherent false belief (a "cognitive lesion"), while the model retains true beliefs that conflict with it. We harvest responses that range from compliant (ignoring the tension) to recovering (noticing the conflict and reasoning toward resolution). Because we induced the lesion, we can grade responses without needing to be "smarter" than the model.

Training on pairs from 55 lesions, we observe transfer to held-out pairs from 56 different lesions (76–80% show improved preference toward recovery). We present this as a starting point for investigating deliberate confusion as a source of epistemic reasoning data.

## Paper

[**Read the paper (PDF)**](paper.pdf)

## Contact

reza.jamei@gmail.com
