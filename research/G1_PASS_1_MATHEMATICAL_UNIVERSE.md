# G1 Pass 1 — Mathematical Universe for Organization

**Gate:** G1 — Mathematical Definition  
**Status:** research artifact; not a bound and not a G1 completion claim  
**Null programme:** `H_0 = known physics/chemistry` using established mathematics. No `Phi` term is introduced.

## 1. Question and conclusion

**[OPEN]** What mathematical objects must exist before organization can be a well-posed object suitable for later bounds?

**Pass-1 conclusion.** MOB-LIFE should begin from an open, possibly stochastic, spatially resolved dynamical system observed through an explicitly indexed family of coarse-graining maps. Organization should initially be represented by a **profile/family of observables**, not a scalar. No surveyed established framework supplies a universal "organization" quantity that distinguishes living/self-maintaining organization from all prescribed nonliving counterexamples.

The minimal canonical substrate earned in this pass is: a measurable state space, trajectory/path law, system/environment partition, exchange channels, spatial/temporal observation scales, and observation maps. Candidate organization components remain provisional.

## 2. Established frameworks: inherit, adapt, distinguish

### 2.1 Dynamical systems
**[EST]** Deterministic evolution supplies state spaces, flows/maps, invariant sets, stability, attractors, bifurcations and correlation/recurrence concepts.  
**Inherit:** state/evolution language and stability tools.  
**Distinguish:** dynamical stability is not organization; a fixed point or limit cycle can be stable with negligible self-maintaining structure.

### 2.2 Stochastic/Markov processes
**[EST]** Markov processes supply transition kernels/generators, stationary measures, hitting/recurrence concepts and path probabilities.  
**Inherit:** path-space description `P[x_{0:T}]` as a general stochastic representation.  
**Adapt:** do not require the observed/coarse system to remain Markovian. Mori–Zwanzig reduction shows unresolved degrees of freedom can appear as memory and noise.

### 2.3 Nonequilibrium statistical mechanics and stochastic thermodynamics
**[EST]** Stochastic thermodynamics defines work, heat and entropy production at trajectory level for well-defined nonequilibrium ensembles; fluctuation relations constrain path probabilities.  
**Inherit:** open-system bookkeeping, driving protocols, reservoirs, currents, trajectory ensembles and entropy production where assumptions apply.  
**Reject as identification:** dissipation/entropy production is not organization. Driven turbulent or convective systems dissipate strongly without satisfying self-maintenance/closure criteria.

### 2.4 Information theory
**[EST]** Entropy, mutual information, conditional information and the data-processing inequality rigorously quantify statistical dependence/information. Predictive information can be defined as past–future mutual information. Transfer entropy detects directed statistical dependence after conditioning on history.  
**Inherit:** dimensionless dependence observables at specified variables/scales.  
**Reject as identification:** information is not organization. High mutual/predictive information occurs in passive periodic, frozen, copied, or externally controlled systems.

### 2.5 Network/graph descriptions
**[EST]** Graph theory and complex-network methods quantify degree, clustering, paths, components, spectra and dynamical processes on networks.  
**Inherit:** typed directed graphs/hypergraphs for reaction, catalytic, constraint or dependency relations.  
**Reject as identification:** topology alone does not encode material realization, rates, energetic feasibility, maintenance or causal direction.

### 2.6 Correlation and spatiotemporal structure
**[EST]** Correlation functions, spectra and correlation lengths characterize spatial/temporal dependence and patterning. Nonequilibrium pattern formation includes convection, hydrodynamic instabilities, chemical oscillations and other nonliving systems.  
**Inherit:** scale-dependent correlation observables.  
**Reject as identification:** long-range order/pattern is not life or self-maintenance.

### 2.7 Coarse-graining / multiscale reduction
**[EST]** Projection/coarse-graining can transform fully resolved Markovian dynamics into reduced dynamics with drift, memory and fluctuating terms.  
**Inherit:** observation maps must be explicit and indexed by resolution.  
**Critical consequence:** organization observables cannot be assumed invariant or monotone under coarse-graining. Information-theoretic dependence can decrease under processing, while apparent memory can increase when hidden variables are eliminated. Therefore transformation laws must be proved observable-by-observable.

### 2.8 Topology
**[EST]** Topological data analysis can extract persistent qualitative structure from high-dimensional/noisy data.  
**Inherit cautiously:** topological summaries are candidate descriptors when the physical object/filtration is justified.  
**Reject as generic organization:** nontrivial topology can occur in passive matter and arbitrary data clouds.

### 2.9 Chemical reaction networks
**[EST]** CRN theory separates species, complexes, reactions, stoichiometric subspaces and kinetics; deficiency theory gives structural/dynamical results under explicit assumptions.  
**Inherit:** typed reaction networks, stoichiometry, kinetics, compatibility classes, open inflow/outflow descriptions.  
**Distinguish:** network structure and even stable reaction dynamics do not alone establish organization.

### 2.10 RAF autocatalytic sets
**[EST]** RAF theory gives a combinatorial criterion/algorithm for reaction subsets that are reflexively autocatalytic and food-generated/self-sustaining relative to a specified food set.  
**Inherit:** a rigorous candidate component for catalytic organization.  
**Limitation:** RAF status depends on the catalytic reaction system and food set and does not by itself impose a generated boundary/compartment. Hordijk and Steel explicitly distinguish RAF theory from models where a maintained/generated boundary is essential.

### 2.11 Constraint/closure approaches
**[EST about the literature; CAND for MOB-LIFE adoption]** Montévil and Mossio formalize biological organization as closure among constraints defined at relevant time scales, with constraints mutually dependent and generative.  
**Use:** this is a serious candidate for a closure component and for system-boundary reasoning.  
**Caution:** it is a theoretical framework, not a theorem that all life or only life satisfies one unique mathematical closure functional. MOB-LIFE must operationalize dependency and maintenance before canonical adoption.

## 3. Candidate admissible system class

### 3.1 Core object
**[CAND]** A system instance over horizon ([0,T]) is provisionally
[
mathcal S=(X,Sigma,mathcal E,mathcal D,mathbb P,mathcal B,mathcal J),
]
where:

- (X): microscopic/finest admitted state space;
- (Sigma): sigma-algebra (or corresponding measurable structure);
- (mathcal E): evolution law (flow/map, stochastic kernel/generator, SDE/SPDE, or reaction dynamics);
- (mathcal D): driving protocol/reservoir specification;
- (mathbb P): induced probability law on trajectories when stochastic or ensemble treatment is required;
- (mathcal B): explicit system/environment boundary or partition rule;
- (mathcal J): admissible matter/energy exchange channels across that boundary.

This tuple is intentionally broad enough to include deterministic dynamics by degenerate path measures.

**[OPEN]** It is not yet canonical because the correct category encompassing PDE fields, particle systems, stochastic processes and CRNs without excessive generality remains unresolved.

### 3.2 Trajectories
**[DEF]** For an admitted state space (X), a trajectory on ([0,T]) is denoted (x_{0:T}) (or (x(t)) in continuous time).  
**[DEF]** (P_{0:T}) denotes a probability law on the relevant path space when an ensemble is required. It is not assumed Markovian.

### 3.3 Boundary and openness
**[CAND]** A MOB-LIFE system boundary must be an explicit modelling object, not inferred from organization after the fact. The boundary may be geometric, compartmental, graph-theoretic, or an observation partition, but its type and exchange channels must be declared.

**[OPEN]** Whether self-generated/maintained boundaries become necessary for later organization levels is not settled at G1.

## 4. Multiscale architecture

**[DEF]** (ell) denotes a spatial observation/coarse-graining scale and (	au) a temporal observation/coarse-graining scale; they are resolution parameters, not organization values.

**[CAND]** Use a family of measurable observation maps
[
C_{ell,	au}:X^{[0,T]}ightarrow X_{ell,	au}^{[0,T']}
]
(or state-level maps where appropriate). This path-level form is preferred over forcing (C_{ell,	au}:X	o X_{ell,	au}), because temporal aggregation generally acts on trajectory segments.

Each map must specify what variables are retained, spatial averaging/partition, temporal sampling/averaging, and treatment of boundary fluxes.

**[REJECTED ASSUMPTION]** Universal monotonicity of "organization" under coarse-graining. Different components transform differently; some information is destroyed, while hidden-variable elimination can induce memory.

**[CAND]** A future organization object should therefore initially be a scale-indexed profile
[
mathfrak O_{mathcal S}(ell,	au)={O_a(mathcal S;ell,	au)}_{ain A},
]
where (A) indexes mathematically distinct components. No aggregation rule or bound is asserted.

## 5. Candidate component audit

| Component | Candidate mathematical object | Units | Scale dependence | Status | Captures | Primary insufficiency |
|---|---|---:|---|---|---|---|
| spatial correlation | connected (n)-point correlations / correlation length / structure factor | variable-dependent; normalized versions dimensionless | explicit (ell) | [CAND] | spatial dependence/order | crystals, convection, turbulence |
| temporal persistence | autocorrelation / survival or recurrence times | time or dimensionless | explicit (	au) | [CAND] | persistence | frozen disorder, oscillators |
| memory | conditional dependence on history; memory kernel where model supports it | model-dependent | strongly scale-dependent | [CAND] | history dependence | coarse-graining itself can induce memory |
| mutual information | (I(U;V)) | bits/nats | variables and coarse-graining dependent | [EST measure], [CAND component] | statistical dependence | passive correlated systems |
| predictive information | (I(	ext{past};	ext{future})) | bits/nats | window/resolution dependent | [EST measure], [CAND component] | predictable structure | periodic oscillator |
| directed dependence | conditional information / transfer entropy | bits/nats | lag/resolution dependent | [EST measure], [CAND component] | directional statistical dependence | common-driver/confounding and control |
| network organization | typed graph/hypergraph invariants, spectra, motifs | mostly dimensionless | representation-dependent | [CAND] | relational architecture | passive engineered/random networks |
| topology | persistent homology or physically defined topological invariants | often scale-indexed | filtration/coarse-graining dependent | [CAND] | robust shape/connectivity | crystals/material defects/data geometry |
| catalytic organization | RAF membership/sub-RAF structure; CRN kinetics | combinatorial plus kinetic units | network/chemical scale | [EST framework], [CAND component] | collective catalysis/food generation | RAF need not include boundary or heredity |
| constraint structure | dependency graph among operational constraints | representation-dependent | time-scale dependent | [CAND] | maintained restrictions on processes | operationalization unresolved |
| dynamical stability | Lyapunov/spectral/return-time quantities | model-dependent | resolution-dependent | [CAND] | robustness/persistence | stable nonliving attractors |
| closure | closed dependency among maintained constraints | initially relational | multiscale | [CAND] | mutual maintenance | needs measurable dependency/maintenance criterion |
| multiscale dependence | spectrum/profile across ((ell,	au)) | component-dependent | intrinsic | [CAND] | cross-scale structure | scale richness alone not life |

## 6. Counterexample programme

### CE1 equilibrium crystal
High spatial order, correlations, low configurational entropy and nontrivial symmetry. **Defeats:** correlation/order as organization sufficient condition.

### CE2 random noise
High Shannon entropy but negligible reproducible structure/predictive information. **Defeats:** entropy/information-content language as organization.

### CE3 frozen disorder
Can store many bits and persist indefinitely while doing no active maintenance. **Defeats:** memory/persistence/information storage alone.

### CE4 turbulent flow
Strong multiscale correlations, fluxes, intermittency and entropy production. **Defeats:** multiscale structure + dissipation as sufficient.

### CE5 convection pattern
Driven nonequilibrium matter forms coherent persistent spatial patterns. **Defeats:** self-organization/pattern formation alone.

### CE6 externally controlled machine
Can show feedback, memory, high mutual information, stable function and complex networks while maintenance/control resources originate externally. **Defeats:** control/function/information without autonomy or endogenous maintenance.

### CE7 simple oscillator
Perfectly persistent and highly predictable temporal structure. **Defeats:** temporal persistence/predictive information alone.

### CE8 highly correlated passive system
Mutual information can be large under equilibrium/common-cause coupling. **Defeats:** correlation/MI as causal organization.

### CE9 high-information archive
A static archive can contain enormous Shannon information and structured dependencies without metabolism or self-maintenance. **Defeats:** stored information/complexity alone.

### CE10 simple RAF
A reaction system may satisfy a rigorous RAF criterion relative to a food set while lacking compartmentalization, heredity or autonomous boundary maintenance. **Defeats:** autocatalysis alone as life/complete organization.

## 7. Distinctions that must survive G1

1. energy throughput != organization;
2. entropy production != organization;
3. Shannon information != organization;
4. correlation != causal dependence;
5. persistence != active maintenance;
6. pattern formation != closure;
7. network complexity != catalytic/constraint closure;
8. autocatalysis != compartmentalized autonomous life;
9. coarse-grained memory != necessarily microscopic memory;
10. externally maintained function != endogenous self-maintenance.

## 8. What earned canonical status

Canonical in this pass: path/trajectory notation; path law; explicit system/environment boundary requirement; explicit exchange channels; spatial and temporal observation scales; explicit coarse-graining/observation maps; no-Markov-under-coarse-graining assumption; organization profile as a *type signature* only (not a numerical definition).

Not canonical: a universal scalar organization number; a universal closure functional; a fixed admissible-system tuple; any monotonicity law under coarse-graining; any claim that RAF, information, entropy production, topology, stability or correlation alone defines organization.

## 9. Unresolved G1 questions

1. What is the narrowest admissible system category that still covers spatial stochastic matter, CRNs and deterministic field models?
2. What boundary semantics allow fair comparison between endogenous maintenance and externally controlled systems?
3. Which component observables admit representation-independent or covariant transformation rules under (C_{ell,	au})?
4. How should "maintenance" be operationalized as a path property rather than mere persistence?
5. Can constraint closure be converted into a measurable dependency/renewal graph without circularly defining organization?
6. Which minimum subset of components is necessary before a future bound can exclude the counterexamples above?
7. How should cross-scale coupling be represented without arbitrary weighting?

## 10. Recommendation

**G1 remains IN PROGRESS.** The single highest-value next question is:

> **What operational, path-level definition of endogenous maintenance can distinguish persistence caused by internal renewal/constraint closure from persistence imposed by equilibrium structure or external control, while remaining well-defined under explicit system/environment boundaries?**

A narrow specialist in stochastic processes/stochastic thermodynamics plus reaction-network/open-system modelling would be useful for that question. Independent Review is premature until this ambiguity is resolved and a smaller canonical system class is proposed.

## Sources

See `sources/source-ledger.md`, entries S001–S014.