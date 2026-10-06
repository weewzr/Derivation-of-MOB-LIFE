# Mathematical Definitions

**Gate:** G1 — IN PROGRESS.
Only definitions that have earned canonical status appear here. No final organization bound is defined.

## D1. Admitted state space
**[DEF]** \(X\) denotes the finest state space admitted by a specified MOB-LIFE model, equipped with the structure required by that model. No universal choice of \(X\) is imposed across all model families.

## D2. Trajectory and path law
**[DEF]** \(x_{0:T}\) denotes a trajectory over \([0,T]\). \(P_{0:T}\) denotes a probability law on the relevant path space when stochastic/ensemble treatment is required. MOB-LIFE does not assume a coarse-grained observed process remains Markovian.

## D3. System/environment boundary
**[DEF]** \(\mathcal B\) is an explicit modelling rule partitioning/identifying system degrees of freedom relative to an environment. Boundary type must be declared and not inferred circularly from a claimed organization score.

## D4. Exchange channels
**[DEF]** \(\mathcal J\) denotes specified matter/energy exchange channels across \(\mathcal B\), including direction/type and units where applicable. Openness does not imply organization.

## D5. Observation scales
**[DEF]** \(\ell\) and \(\tau\) are spatial and temporal observation/coarse-graining scales. They are resolution parameters, not organization values.

## D6. Observation/coarse-graining map
**[DEF]** \(C_{\ell,\tau}\) is a declared measurable observation/coarse-graining map from fine trajectories (or states where appropriate) to an observed representation at scales \((\ell,\tau)\). Retained variables, spatial/temporal aggregation and relevant boundary-flux treatment must be specified. No universal organization monotonicity is assumed.

## D7. Organization profile type
**[DEF: type only]** \(\mathfrak O_{\mathcal S}(\ell,\tau)\) is a scale-indexed family/profile placeholder for mathematically distinct organization-component observables. No weighting or scalar aggregation rule is canonical.

## D8. Canonical G1 stochastic reaction-compartment test class
**[DEF: restricted domain]** A canonical test-class model is a finite-species continuous-time Markov jump reaction system with:
1. species partition \(\mathsf S=\mathsf S_{\rm int}\sqcup\mathsf S_{\rm bnd}\sqcup\mathsf S_{\rm env}\sqcup\mathsf S_{\rm ctrl}\);
2. system-side count state \(X_t\in\mathbb N_0^d\) for internal/boundary species;
3. finite typed reaction set \(\mathsf R\), stoichiometric jumps \(\nu_r\), and propensities \(a_r(x,t)\);
4. generator \((\mathcal L_t f)(x)=\sum_r a_r(x,t)[f(x+\nu_r)-f(x)]\);
5. explicit boundary induced by the declared partition and cross-boundary channels;
6. declared horizon and event record sufficient to identify typed currents.

This is a canonical **test class**, not the universal MOB-LIFE admissible class.

## D9. Test-class channel provenance
**[DEF: restricted domain]** Before maintenance evaluation, each channel is typed exactly once as: internal process-mediated; supply/removal; external open-loop forcing; external feedback/control; or external repair/replacement.

Typing is determined by physical mechanism location and conditional dependence, not by the desired verdict. Raw environmental matter/free-energy supply may feed internal processes without becoming an internal restorative policy.

## D10. Predeclared viability audit
**[DEF: restricted domain]** A maintenance audit predeclares measurable viability observable \(V\), admissible region \(K\), maintained variables \(Y\), loss/degradation channels, horizon \(T\), and comparison statistic before evaluating maintenance interventions.

\[
\mathcal V_T=\{V(X_t)\in K\ \text{for all }t\in[0,T]\}.
\]

Choices may be question-dependent; predeclaration prevents post-hoc construction of a favorable certificate.

## D11. Reaction-removal intervention
**[DEF: restricted domain]** For \(A\subseteq\mathsf R\), \(\mathcal M^{-A}\) sets \(a_r=0\) for \(r\in A\) while retaining the initial law, external protocols and structural forms of nonremoved propensities.

**[ASM]** Causal interpretation requires modularity: disabling the mechanism must not silently change other mechanism laws. Otherwise simple reaction removal is not an admissible causal test.

## D12. EMC-admissible observation map
**[DEF: restricted domain]** For the canonical test class, an observation map is EMC-admissible only if it preserves: (i) maintained variables and viability event; (ii) loss/restoration event identity or sufficient current statistics; (iii) channel provenance; (iv) intervention mappings for dependency edges; and (v) boundary membership of mediating degrees of freedom.

Aggregations mixing internal and external provenance are not EMC-admissible.

## Explicit non-definitions
Entropy, entropy production, mutual information, correlation length, graph complexity, topology, dynamical stability, RAF membership, persistence, predictive information, RCC, CRDC, EMC, or closure individually are **not** canonical definitions of organization.

RCC, CRDC and EMC remain provisional maintenance criteria. See \`research/G1_SPECIALIST_ENDOGENOUS_MAINTENANCE.md\` and \`research/G1_PASS_2_CANONICAL_TEST_CLASS.md\`.

## D13. Canonical organization-profile component basis

**[DEF: profile-axis basis, G1 domain-relative]** On the admitted G1 domains, the organization profile retains the following mathematically distinct component axes:
\[
\mathfrak O_{\mathcal S}(\ell,\tau)
=
\{
O_{\rm maint},
O_{\rm cat},
O_{\rm dep},
O_{\rm hered},
O_{\rm spatial},
O_{\rm robust},
O_{\rm xscale}
\}_{\ell,\tau}.
\]

These are **axis/type definitions**, not scalar scores, sufficient conditions for organization, or criteria for life. Exact observables may be families and must declare their domain, units and observation map.

### D13a. Endogenous-maintenance axis \(O_{\rm maint}\)
Records boundary-relative evidence of internally mediated renewal against declared loss/degradation, including restoration currents, intervention effects and provenance/dependency information where applicable. RCC/CRDC/EMC remain provisional implementations, not universal definitions.

### D13b. Catalytic-organization axis \(O_{\rm cat}\)
Records catalytic/reaction-network organization, such as RAF/subRAF structure and, where required, kinetic catalytic currents on a declared chemical reaction representation. It is domain-specific and depends on species/reaction/food resolution.

### D13c. Intervention-backed dependency axis \(O_{\rm dep}\)
Records mechanistic support/dependency relations admitted by declared interventions under explicit modularity assumptions. Correlation or transfer entropy alone does not establish an edge.

### D13d. Heredity axis \(O_{\rm hered}\)
Where a transmission/reproduction map and heritable variables are declared, records persistence/transmission of state across those events using fidelity/error kernels, parent-descendant information or equivalent mathematically specified observables. For systems without such a map the axis is **not applicable (N/A)**, not zero.

### D13e. Spatial/compartment axis \(O_{\rm spatial}\)
Records physically declared spatial localization, interfaces, compartment membership, segregation or maintained boundary organization. It is explicitly spatial-scale dependent; topology may appear as a subdescriptor only when physically justified.

### D13f. Dynamical-robustness axis \(O_{\rm robust}\)
Records response, survival or return under a predeclared perturbation class, using model-appropriate quantities such as exit/return probabilities or times, spectral stability or Lyapunov-type measures where defined.

### D13g. Cross-scale axis \(O_{\rm xscale}\)
Records dependence/coupling between explicitly declared scale representations, using information-, response-, dependency- or mechanism-preservation observables appropriate to a declared pair/family of observation maps. No single universal cross-scale statistic or monotonicity law is assumed.

**[SCOPE]** This seven-axis basis is minimal/nonredundant only relative to the current admitted G1 model and counterexample class. Universal logical necessity is not claimed.

## D14. Descriptor versus profile axis

**[DEF]** A **profile axis** is retained when removing it loses a mathematically relevant distinction on the admitted model/counterexample class that the remaining axes do not represent.

**[DEF]** A **descriptor** is a valid observable that may characterize a system but has not earned independent-axis status under the current adversarial removal test.

At G1 Pass 3, generic memory, predictive information, directed statistical dependence/transfer entropy, generic topology, generic correlation, information content and dissipation remain descriptors/diagnostics or subcomponents rather than independent canonical profile axes.
