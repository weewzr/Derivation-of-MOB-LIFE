# Controller Assignment — G1 Specialist Pass: Endogenous Maintenance

**Role:** Specialist — stochastic processes / stochastic thermodynamics / open reaction-network modelling  
**Gate:** G1 — Mathematical Definition  
**Authorization:** ACTIVE  
**G1 remains IN PROGRESS. G2 is not authorized.**

Read `MASTER_INSTRUCTIONS.md`, `STATUS.md`, `research/G1_PASS_1_MATHEMATICAL_UNIVERSE.md`, `mathematics/definitions.md`, `mathematics/notation.md`, and `negative-results/G1_PASS_1_COUNTEREXAMPLES.md` before starting.

## Single specialist question

> What operational, path-level definition of **endogenous maintenance** can distinguish persistence produced by internal renewal/constraint-support processes from (a) equilibrium/passive persistence and (b) persistence imposed by an external controller or maintainer, under an explicit system/environment boundary?

This is a narrow G1 specialist task. Do not design the final MOB, do not aggregate organization into a scalar, do not advance to G2, and do not introduce `Phi`.

## Required investigation

Work from known physics/chemistry and established mathematics. Compare, where relevant:

- stochastic-process and path-space formulations;
- stochastic thermodynamics of open driven systems;
- controlled versus autonomous Markov processes;
- open chemical reaction networks;
- reaction currents, renewal/turnover and material replacement;
- RAF/autocatalytic-set formalisms;
- constraint/closure formalisms;
- intervention/counterfactual ideas only where they can be stated without importing unjustified causal claims.

Determine whether maintenance can be expressed using observable or model-defined path quantities such as renewal fluxes, reaction/current structure, dependency relations, viability-region return/restoration, internal versus externally supplied control channels, or combinations thereof.

## Boundary discipline

The criterion must explicitly depend on a declared boundary `mathcal B` and exchange channels `mathcal J`.

It must not define the boundary by first identifying the thing judged to be organized.

Make explicit what counts as:

1. environmental supply of raw matter/energy;
2. environmental forcing;
3. external feedback/control;
4. internal process-mediated restoration/renewal.

A living system is allowed to depend on environmental matter and free energy. Therefore “endogenous” must not mean energetically isolated or independent of the environment.

## Required adversarial tests

Any proposed criterion must be tested against at least:

- equilibrium crystal;
- frozen passive structure;
- simple driven convection/pattern;
- externally thermostatted or feedback-controlled machine;
- externally repaired machine;
- simple oscillator;
- simple RAF without maintained compartment;
- open autocatalytic network;
- a minimal self-maintaining reaction/compartment model if an established one is available.

Identify false positives and false negatives explicitly.

## Deliverable

Create:

`research/G1_SPECIALIST_ENDOGENOUS_MAINTENANCE.md`

The artifact must include:

1. precise problem statement;
2. established frameworks/results used, with provenance;
3. at least two serious candidate mathematical definitions or criteria;
4. assumptions and domains for each;
5. explicit boundary/control semantics;
6. adversarial counterexample table;
7. comparison of candidates;
8. recommendation: adopt, reject, or retain provisionally;
9. exact unresolved obstruction if none succeeds.

Add authoritative sources to `sources/source-ledger.md`.

Record informative failures in `negative-results/`.

Do **not** silently promote a candidate into `mathematics/definitions.md`. Recommend canonicalization to Main Research/Controller; canonical project definitions should be integrated only after the specialist result is assessed.

## Success condition

Success does not require finding a perfect definition.

A successful specialist pass either:

- supplies a precise candidate that survives the stated adversarial tests under explicit assumptions; or
- proves/argues clearly why the current notion is underdetermined and identifies the minimal additional structure needed.

## End-of-pass report

Report:

1. files/branch/PR/commit state;
2. candidate criteria examined;
3. strongest surviving criterion, if any;
4. strongest counterexample;
5. assumptions needed;
6. whether the G1 maintenance/boundary blocker is resolved, narrowed, or unresolved;
7. what Main Research should do with the result.

Stop. Do not continue to G2 and do not perform an Independent Review.
