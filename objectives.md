---
layout: page
title: Objectives
permalink: objectives.html
order: 1
---

The RIPOST associate team will address the reproducibility testing challenge in computer science
by combining distinct expertises in Software Engineering, Resilient Software Science and
AI-based Software Testing coming from both teams. Specifically, the associate team will address
four main objectives:

# Objective #1: Reproducing experiments with deep variability

Reproduction of a computational study means running the same computation on the same input
data, and then checking if the results are the same, or at least “close enough” when it comes to
numerical approximations. Reproduction can be considered as software testing at the level of a
complete study. In practice, we don’t “test” in one run, in one computing environment, with one
kind of input data, etc.

On the one hand, there are numerous varying conditions to guide an experimental evaluation,
what we have called deep software variability from the hardware to the operating system to
the compiler flags to the dependencies versions to the parameters of a software application. A
key lesson from RESIST-EA team is that the variability of each layer interacts in a
non-monotonous way – empirical observations support our claims [3]
On the other hand, it is impossible to explore exhaustively all these variable conditions in test
environments. Hence, the overall challenge is to sample the variability space of testing conditions
to ensure that a computational result resides in the same “envelope”. If not, it means that the
scientific result is not robust and resilient – there could be good explanations, hence the need of
Objective #3 and #4 to synthesize a minimal and interpretable information. If the results
reproduce and generalize, we can trust the computational infrastructure and augment the
confidence.

# Objective #2: Replication through automated variation of computational experiments

A related and follow-up of reproducing an experiment is to build upon to explore new variability
(hypothesis, methods, and effects.). Replication of a scientific study (computational or other)
means repeating a published protocol, respecting its spirit and intentions but varying the
technical details. In our software-intensive context, this means using different software (e.g.
library versions, different hyperparameters), running a simulation from different initial conditions,
etc. The idea is to change “something” across variability layers and see if the scientific
conclusions are affected or not.

In a sense, it is similar to Objective #1 and there is an opportunity to reuse a common
framework for automating the exploration of deep variability. However, the intention differs and
computational scientists are not expecting to obtain the same result since something more
fundamental has changed, e.g a statistical test, a threshold, a computational method, or simply
input data.

Here, we aim to leverage deep software variability in order to synthesize new findings,
insights, and hopefully scientific knowledge.
We plan to (1) mine relevant patterns out of observational data gathered through the exploration
of deep variability; (2) establish metamorphic relations across variability layers to confirm some
results or to pinpoint deviations.

# Objective #3: Safe and minimal explanations for reproducible scenarios

We look for the minimal necessary explanations, respectively pre-conditions, to cause a certain
behaviour in a reproducible, i.e. repeatable way, so that it can serve scientists and domain
experts in a long term as a test/validation scenario.

Take, for example, an automated vehicle that observes its environment and takes decisions based
on it. Suddenly, a full braking maneuver is operated while the car is automatically driving. We aim
to find the core subset of the environment, e.g. the kid running across the street to a dog, that
causes this behaviour, while ignoring everything else, e.g. the cars behind us or the people sitting
in a café. We want to find some “minimal reproducible set” of explanations.

This research has thereby connections to root cause analysis and debugging. This research
line does not address reproducibility in the traditional sense (i.e., making sure that there are no
variations in executions) but it aims at finding reproducible conditions in the behaviour of the
system. Answering this objective will allow the generation of new, realistic scenarios by only
changing a few aspects (e.g., the kid is running to their grand-parents instead of a dog) and thus
will contribute to not only reproducibility but also resiliency for the system as it will face multiple
similar scenarios.
# Objective #4: Interpretable explanations for reproducible and replicable scenarios

When performing hundreds of experiments, scientists and domain experts can struggle to
understand whether the results generalize in every condition or to identify what variability factors
lead to another set of results. Is it due to the use of new hardware? Is it an accidental complexity
raised by a change of a library version? Or is it the effect of this parameter that changed the
algorithm.

An objective is thus to synthesize an information that is understandable and interpretable.
Minimality of the problem (Objective #3) can naturally help here as a way to reduce the
dimensionality of the problem, but may not be sufficient for a comprehensive and fine-grained
understanding, especially when interpreting scientific results. Explainable AI methods and
tools can bring interesting insight on why results can be generalizable or not. Objective #4 is
dedicated to the challenge of applying successfully explainable AI methods and tools to the
reproducibility and replicability scenarios.

# Objective #5: Applications and case studies

The validation of methods and tools developed in the RIPOST associate team will be held on at
least the following case studies, spanning different fields and research expertise of Inria and
Simula: Numerical computations using floating point computations, automated driving, cardiac
modelling, medical imaging and neuroimaging (eg https://www.narps.info/).

Automated Driving applications span over the Sense-Plan-Act paradigm by proposing the usage
of AI models depending on data acquisition performed over a large variability space. This
includes non exhaustively, a large number of different sensors, a large panel of AI models
ranging from classical SVM to random forest and deep learning. This variability space is a
formidable game field for the methods developed in the RIPOST associate team.

Similarly, medical image anaysis and neuroimaging studies are characterised by a large variability
space and, to build their analyses, practitioners must choose between different software,
software versions, algorithms, parameters, etc. For many years, those choices have been
considered as "implementation details", but evidence is growing that the exact choices of analysis
strategy can lead to different and sometimes contradictory results [4, 10]. The case of NARPS
[10] is an opportunity to test the reproducibility and to replicate experiments, and to gather
minimal and interpretable information that can guide and help scientists.

Other case studies such as for instance cardiac modelling will serve the same purpose: (1)
challenging our research, method, techniques, and results; (2) refining and validating our
proposal; (3) collaborating with other partners at Inria and Simula and stimulating exchanges for
the important topic of reproducibility and replicability in computational science.
