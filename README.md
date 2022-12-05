# HiPEAC2023

A full-day tutorial to be presented at HiPEAC 2023 in Toulouse, France


## Introduction to ∆Q-SD - a performance centric design framework

The ΔQ Systems Development paradigm (ΔQSD) is a novel and industrially-derived
systems development methodology for developing complex real-world distributed
systems, which directly embeds statistically-based performance metrics from the
outset of the system design process, and throughout the entire software
production life cycle. Its main novelty lies in how it captures the mixture of
delay and failure, the continuous and discrete in a single consistent notion.
This paradigm has been developed by PNSol over a period of 20+ years, in
collaboration with IOG (formerly IOHK), BT, Vodafone, Boeing, Space and Defence, and other
major companies who focus on the development of reliable high-quality, high
integrity, distributed software systems, with strong real-time requirements. It
has been used to successfully manage performance and architectural tradeoffs in
IOG’s Cardano PoS, as well as being used to perform network service
assessments, quantitative analysis of technology and products, in-life
optimisation of performance characteristics of broadband network infrastructure.

In just the aspect of creating a compositional framework for measurement of
network quality, the paradigm has recently been adopted as a new Technical
Report (TR 452.1) by the Broadband Forum and is the subject of ongoing
standardisation and development effort as part of their QED programme.

In particular it:
* Treats performance as first class citizen
  * Is outcome-centric, specially concerns itself with the timeliness (and
    probability of success) of an activity of interest
* Takes an approach that works for the whole system development lifecycle -
  from validating initial goals to in-life service assurance, and the points
  between.
* Permits top-down and bottom-up (or a mixture) design approaches. i.e,
  * Top down: Can this "outcome" be met as the system is refined?
  * Bottom up: Given these design constraints (e.g. existing system) what will
    the performance be for this desired outcome?
  * Comparison: Is system/component A 'better' than system/component B (for given collection of outcomes).
* Can formulate both system-centric and user-centric “experience” questions:
  * system-centric: How efficiently will the final system use this (expensive) resource?
  * user-centric:  What is the likely distribution of response times be for the set of users?
  * resilience-centric: How sensitive to operational conditions is outcome X?

Where has it been used:
* Service assurance and strategic planning of national broadband deployments.
* Validating potential effectiveness of safety-of-life distributed systems in adversarial environments.
* Design, development, and deployment of the largest proof-of-stake based ledger
  technology where assuring timeliness is a key security property.

What will we discuss:
* How improper random variables can capture the key attribute of 'quality
  attenuation' - a _single_ measure of timeliness and probability of success.
* How convolution, probabalistic choice combined with first and last to finish
  appears sufficiently rich to capture real world systems.
* Examples/case studies
* How we are embedding tool support into online notebooks for rapid assessment of
  design choices and performance issues.
  
See https://mdpi.com/2073-431X/11/3/45 for a recent paper on ΔQSD.
