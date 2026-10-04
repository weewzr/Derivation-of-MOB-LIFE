# Controller Assignment — G1 Pass 1

**Role:** Main Research  
**Gate:** G1 — Mathematical Definition  
**Authorization:** ACTIVE  
**Do not advance to G2 without a subsequent Workflow Controller decision.**

Read `MASTER_INSTRUCTIONS.md` and `STATUS.md` before starting.

## Objective

Establish the mathematical universe in which a future quantity or family of quantities representing organization could be rigorously defined.

Central question:

> What mathematical objects, domains, scales, observation/coarse-graining operations, and candidate observables are required before “organization” can become a well-posed object suitable for later bounds?

Do not formulate the final Multiscale Organization Bound in this pass. Do not introduce an unknown organizing field `Phi`. The programme remains

[
H_0 = \text{known physics/chemistry}
]

using established mathematics.

## 1. Survey relevant established frameworks

Research authoritative frameworks relevant to defining organization in nonequilibrium matter, including:

- dynamical systems;
- stochastic processes / Markov processes;
- nonequilibrium statistical mechanics;
- information theory;
- stochastic thermodynamics;
- network and graph descriptions;
- spatial correlation functions;
- temporal correlation and memory;
- multiscale/coarse-grained descriptions;
- topology where genuinely relevant;
- reaction networks and catalysis;
- constraint and closure concepts;
- mathematically formalized self-maintaining/autocatalytic organization.

This is not an encyclopedic literature review. Determine what MOB-LIFE should inherit, adapt, distinguish, or reject. Prefer primary papers, authoritative monographs, and strong scholarly reviews. Record provenance in the source ledger.

## 2. Define the admissible system class

Develop candidate definitions for the initial system class. Make explicit candidates for objects such as

[
X,\quad \Omega,\quad x(t),\quad P[x_{0:T}],
]

or better representations where justified.

Address system state, deterministic/stochastic dynamics, spatial degrees of freedom, system/environment boundary, open driven systems, energy/matter exchange, and trajectory/path ensembles where needed. Explain why each object is required.

## 3. Establish the multiscale architecture

Define how spatial and temporal scales enter. Investigate justified observation/coarse-graining maps such as

[
C_{\ell,\tau}:X\to X_{\ell,\tau}.
]

Clarify what `ell` and `tau` represent, what coarse-graining preserves/destroys, whether organization should be invariant/covariant/monotone/neither under coarse-graining, and whether scale spectra are needed.

Wang–Zahl is methodological inspiration only. Do not manufacture a Kakeya equivalence.

## 4. Candidate organization components

Do not prematurely collapse organization into one scalar. Identify mathematically distinct candidate components, critically investigating where appropriate:

- spatial correlation;
- temporal persistence;
- memory;
- mutual information;
- predictive information;
- causal/dependency structure;
- network organization;
- topology;
- catalytic organization;
- constraint structure;
- dynamical stability;
- closure;
- multiscale dependence.

For each candidate determine: mathematical definition/candidate definition; domain; units/dimensionality; scale dependence; epistemic status; physical feature captured; limitations; and whether high values occur in obviously nonliving systems.

Do not equate information, energy, complexity, organization, and life.

## 5. Counterexample programme

Actively attack candidate definitions using systems including:

- equilibrium crystals;
- random noise;
- frozen disorder;
- turbulent flows;
- convection patterns;
- externally controlled machines;
- simple oscillators;
- highly correlated passive systems;
- high-information systems without self-maintenance;
- simple autocatalytic networks.

Identify which proposed properties are insufficient and which distinctions must survive. Record scientifically informative failures in `negative-results/`.

## 6. Canonical artifacts

Update `mathematics/definitions.md` and `mathematics/notation.md` only with definitions/notation that earn canonical status.

Create a substantive G1 artifact under `research/` documenting frameworks examined, candidate system classes, multiscale architecture, organization components, counterexamples, unresolved ambiguities, sources, and recommendations for the next G1 pass.

Use the epistemic labels required by `MASTER_INSTRUCTIONS.md`. Do not present project inventions as established results.

## 7. Gate discipline

Do **not** mark G1 complete merely because this pass finishes.

Assess whether these are genuinely sufficiently precise:

- admissible system class;
- system/environment boundary;
- dynamics;
- spatial scales;
- temporal scales;
- observation/coarse-graining maps;
- canonical notation;
- candidate organization object(s);
- distinction between organization and nearby concepts;
- counterexample resistance.

If any remain materially ambiguous, G1 remains **IN PROGRESS**.

Update `STATUS.md` accordingly.

## 8. End-of-pass report

After committing the work, report:

1. branch and commit/PR state;
2. files created or changed;
3. canonical definitions established;
4. candidate definitions rejected or weakened;
5. strongest counterexamples found;
6. unresolved G1 questions;
7. whether G1 remains in progress or is genuinely complete;
8. whether a narrow specialist is required;
9. whether Independent Review is warranted;
10. the single highest-value next research question.

Stop after this pass. Do not proceed into G2 without a subsequent Workflow Controller decision.
