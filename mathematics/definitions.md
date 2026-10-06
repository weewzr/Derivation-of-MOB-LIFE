# Mathematical Definitions

**Gate:** G1 — IN PROGRESS.  
Only definitions that earned canonical status in G1 Pass 1 appear here. They define the mathematical substrate; they do **not** define a final organization bound.

## D1. Admitted state space

**[DEF]** (X) denotes the finest state space admitted by a specified MOB-LIFE model, equipped with the measurable/topological/geometric structure required by that model.

No universal choice of (X) is yet imposed across particle, field, stochastic and reaction-network models.

## D2. Trajectory and path law

**[DEF]** (x_{0:T}) denotes a trajectory of the admitted system over observation horizon ([0,T]) (with (x(t)) used when convenient in continuous time).

**[DEF]** (P_{0:T}) denotes a probability law on the relevant trajectory/path space when stochastic or ensemble treatment is required. Deterministic dynamics may be represented by a degenerate path law when useful.

**[DEF]** MOB-LIFE does not assume that a coarse-grained observed process is Markovian.

## D3. System/environment boundary

**[DEF]** (mathcal B) is an explicit modelling rule that partitions or identifies system degrees of freedom relative to an environment for the question under study.

The boundary type must be declared (for example geometric, compartmental, graph-theoretic, or observational). It must not be inferred circularly from a claimed organization score.

## D4. Exchange channels

**[DEF]** (mathcal J) denotes the specified matter/energy exchange channels permitted across (mathcal B), including their direction/type and physical units where applicable.

This definition records openness; it does not imply that large flux is high organization.

## D5. Observation scales

**[DEF]** (ell) is a spatial observation/coarse-graining scale and (	au) is a temporal observation/coarse-graining scale. They are resolution parameters, not organization values.

## D6. Observation/coarse-graining map

**[DEF]** (C_{ell,	au}) denotes a declared measurable observation/coarse-graining map from fine trajectories (or states when temporal aggregation is absent) to an observed representation at spatial scale (ell) and temporal scale (	au).

Every use must specify retained variables, spatial partition/averaging, temporal sampling/averaging, and treatment of boundary fluxes relevant to the calculation.

No universal invariance, covariance, or monotonicity of organization under (C_{ell,	au}) is assumed.

## D7. Organization profile type

**[DEF: type only]** (mathfrak O_{mathcal S}(ell,	au)) denotes a **scale-indexed family/profile placeholder** for mathematically distinct organization-component observables of a specified system (mathcal S).

This is a type signature, not a scalar definition and not a claim that any current candidate component is necessary or sufficient. No weighting or aggregation rule is canonical.

## Explicit non-definitions

The following are **not** canonical definitions of organization: entropy; entropy production; mutual information; correlation length; graph complexity; topology; dynamical stability; RAF membership; persistence; predictive information; or closure taken individually.

See `research/G1_PASS_1_MATHEMATICAL_UNIVERSE.md` and `negative-results/G1_PASS_1_COUNTEREXAMPLES.md`.