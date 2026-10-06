# G1 Specialist Pass — Endogenous Maintenance

**Role:** Specialist — stochastic processes / stochastic thermodynamics / open reaction-network modelling  
**Gate:** G1 — Mathematical Definition  
**Status:** specialist research artifact; recommendation only; no canonical definition is promoted here  
**Null programme:** `H_0 = known physics/chemistry`. No `Phi`, G2 bound, or scalar organization quantity is introduced.

## 1. Precise problem

**[OPEN]** Given a declared system/environment boundary `mathcal B`, declared exchange channels `mathcal J`, a path law `P_{0:T}`, and a specified viability region `V` in an admitted state representation, when is persistence over `[0,T]` produced by **endogenous maintenance** rather than by:

1. equilibrium/passive persistence;
2. externally imposed forcing or feedback;
3. external repair/replacement?

The required distinction is relational and boundary-relative. “Endogenous” cannot mean energetic isolation: a candidate system may import matter and free energy. The issue is instead **where the state-conditioned mediation that restores/renews the maintained variables is physically realized**.

**[CAND] Specialist working meaning.** Endogenous maintenance is path-level restoration/renewal of declared system variables, against specified loss/degradation channels, whose state-conditioned mediating transitions are realized by degrees of freedom inside `mathcal B`, while environmental channels provide admissible matter/energy supply but do not themselves encode the restorative policy.

This is not proposed as a definition of life or organization.

## 2. Established frameworks/results used

### 2.1 Stochastic trajectory thermodynamics

**[EST]** Chemical master-equation models admit trajectory-level reaction events and thermodynamic bookkeeping. Schmiedl & Seifert define energy, entropy and entropy production along single stochastic CRN trajectories. This supplies a rigorous path/event substrate but does not make entropy production a maintenance criterion (S017).

**[EST]** Open CRNs can be represented with chemostatted species/reservoirs and driven reaction currents. Rao & Esposito formulate nonequilibrium thermodynamics for deterministic open CRNs with time-dependent chemostats (S018), and later for stochastic open CRNs, separating time-dependent chemostat work from nonconservative forcing maintained by flows (S019). Thus environmental free-energy/matter supply is compatible with a system-level maintenance question; mere driven current is not sufficient.

### 2.2 External feedback versus autonomous coupling

**[EST]** Stochastic thermodynamics explicitly treats externally measured feedback control (S020). Therefore stable state regulation plus feedback cannot by itself identify endogenous maintenance.

**[EST]** Bipartite stochastic systems can also implement autonomous information-mediated operation with both subsystems included in a joint Markov description (S021). This is important for boundary discipline: “controller” is not intrinsically external. Whether control is endogenous depends on whether the controller degrees of freedom are inside the declared `mathcal B` and on their own maintenance/dependency relations.

### 2.3 Open CRNs, RAFs and boundaries

**[EST]** RAF theory gives a precise food-generated/reflexively autocatalytic relation but does not by itself require a generated boundary (S012–S013). Hordijk & Steel show how boundary participation can be represented in an extended RAF construction (S013). Hence RAF status is useful dependency structure but is not sufficient for endogenous maintenance.

### 2.4 Constraint closure/basic autonomy

**[EST literature framework]** Montévil & Mossio characterize biological organization through mutually dependent constraints acting on thermodynamically open processes (S014). Their framework motivates dependency closure but does not directly provide a stochastic path functional that resolves all MOB-LIFE counterexamples.

**[EST literature framework]** Ruiz-Mirazo & Moreno argue for basic autonomy in terms of materially/energetically grounded self-construction and explicitly emphasize construction of system boundaries and internally generated constraints (S022). They also state that basic autonomy is not sufficient for life. This supports treating maintenance as a narrower object than life.

## 3. Boundary and control semantics

For this pass, every model must refine the canonical `mathcal J` into typed channels. This is **[CAND] specialist notation**, not canonical notation:

- `J_sup`: environmental supply channels. Matter, chemical potential, photons, heat reservoirs, or other free-energy resources cross `mathcal B` without state-dependent instructions specifying which internal restorative action to execute.
- `J_forc`: environmental forcing channels. Externally prescribed protocols or boundary conditions alter rates/forces but need not depend on the instantaneous internal state.
- `J_ctrl`: external feedback/control channels. Signals/actions crossing `mathcal B` depend on measurements or state estimates of the system and select restorative actions.
- `J_rep`: external repair/replacement channels. Functional system components are replaced/repaired by an external agent or process across `mathcal B`.
- `R_int`: internal process-mediated transitions. Reactions, transports, switching events, assembly/disassembly or other transitions whose mediating degrees of freedom and state dependence are represented inside `mathcal B`.

The classification is physical/model-based, not semantic. A channel cannot be called “supply” merely because doing so makes a candidate pass. The model must state what crosses the boundary and whether its statistics/protocol depend on internal state.

### 3.1 Non-circular boundary rule

**[ASM]** `mathcal B` is fixed before evaluating maintenance, by an independently declared geometric, compartmental, graph-theoretic or observational partition. Candidate maintenance may be evaluated under several predeclared boundaries, but the winning boundary may not be selected after inspecting the maintenance score without reporting that selection procedure.

### 3.2 Controller relocation test

A feedback device outside `mathcal B` acts through `J_ctrl` and is external. If the same physical controller is moved inside an enlarged predeclared boundary, it becomes part of the candidate system; however, its own renewal/support dependencies then enter the maintenance test. This prevents “internal” from being synonymous with “biological” while making the criterion explicitly boundary-relative.

## 4. Candidate A — Restoration-current criterion (RCC)

### 4.1 Setup

Let `Y_t = y(x_t)` be declared maintenance-relevant variables and `V subseteq Y` a predeclared viability region. Let `D` be declared degradation/loss transitions that tend to move `Y` away from `V`, and partition restorative transitions into internal `R_int` and external `R_ext = J_ctrl union J_rep`.

For a jump process, let `N_r[0,T]` count occurrences of transition/reaction `r`. Choose a nonnegative restoration increment `g_r(y)` that is positive only when transition `r` moves the declared variable toward `V` under a predeclared distance or return functional. Define

```
R_int(T) = sum_{r in R_int} integral_0^T g_r(Y_{t-}) dN_r(t)
R_ext(T) = sum_{r in R_ext} integral_0^T g_r(Y_{t-}) dN_r(t).
```

Continuous-state diffusions may use the corresponding current/generator decomposition when physically identifiable.

Define turnover for a maintained component `k` by paired production/loss counts or fluxes, e.g.

```
Theta_k(T) = min{N_k^prod(T), N_k^loss(T)} / T,
```

with stoichiometric weighting when required.

### 4.2 RCC criterion

**[CAND-A]** A trajectory ensemble satisfies RCC on `[0,T]` if:

1. **nontrivial challenge:** declared degradation/loss has nonzero path activity or would drive exit from `V` on the comparison dynamics;
2. **internal restoration:** `E[R_int(T)] > 0` and restoration is state-coupled to departures/losses rather than a coincidental stationary flux;
3. **renewal:** at least one declared maintained material/constraint-bearing component has `E[Theta_k(T)] > 0`;
4. **viability effect:** suppressing the identified `R_int` transitions in the *same specified model* lowers a predeclared viability statistic, such as `P(tau_V > T)` or expected occupation time of `V`;
5. **external-control exclusion:** the same viability statistic is not predominantly restored by `J_ctrl` or `J_rep`.

Here `tau_V` is the first exit time from `V`. Condition 4 is a model intervention, not a claim of general philosophical causation.

### 4.3 Assumptions/domain

- transition/current decomposition is physically meaningful;
- `Y,V,D,R_int,R_ext` are declared before evaluation;
- intervention by suppressing a reaction/channel is mathematically defined and does not silently replace the whole model;
- sufficient path data/model access exists to estimate currents and first-passage/occupation statistics.

### 4.4 Strength and failure

RCC rejects passive crystals/frozen structures because turnover/restoration is absent, and rejects external repair when restoration crosses `J_rep`. It can reject externally feedback-controlled systems when the feedback action crosses `J_ctrl`.

**Failure:** RCC can accept a nonliving internally controlled machine whose controller, actuator and replacement stock all lie inside `mathcal B`. That is not logically wrong if the target is only “endogenous maintenance,” but it proves RCC cannot by itself define biological organization. It can also accept an open autocatalytic network that restores concentrations without maintaining a compartment.

## 5. Candidate B — Closed renewal-dependency criterion (CRDC)

### 5.1 Renewal/dependency graph

Let `K={K_1,...,K_m}` be declared constraint-bearing or maintenance-mediating components/processes inside `mathcal B`. Construct a directed graph `G_M` with edge

```
K_i -> K_j
```

iff, under the specified model and horizon:

1. activity/state of `K_i` materially contributes to production, repair, renewal or viability-support of `K_j`; and
2. suppressing the relevant mediation by `K_i`, while retaining environmental supply channels, measurably reduces a predeclared renewal/viability statistic for `K_j`.

This is a model-defined dependency graph; correlation or transfer entropy alone is insufficient.

### 5.2 CRDC criterion

**[CAND-B]** A system satisfies CRDC on `[0,T]` if there exists a nonempty internal set `K^* subseteq K` such that:

1. every `K_j in K^*` undergoes nonzero loss/turnover on the horizon or specified stationary ensemble;
2. every `K_j in K^*` has at least one incoming maintenance dependency from another member of `K^*`;
3. every `K_i in K^*` contributes to maintenance of at least one member of `K^*`;
4. the induced dependency graph on `K^*` is strongly connected, or a weaker closure structure is explicitly justified;
5. environmental `J_sup` may supply matter/free energy, but no indispensable state-conditioned repair/control dependency for members of `K^*` enters solely through `J_ctrl` or `J_rep`;
6. if a compartment/boundary component is claimed as part of the maintained organization, its production/repair and its effect on internal retention/transport must appear in `G_M`.

### 5.3 Assumptions/domain

- components `K_i` have an operational identity and turnover time scale;
- dependencies are interventionally definable inside the model;
- time-scale separation is adequate to distinguish a constraint-bearing component from the faster processes it modulates where that language is used;
- strong connectivity is a deliberately stringent candidate, not an established biological theorem.

### 5.4 Strength and failure

CRDC captures mutual renewal and makes external repair visible. It can distinguish a bare RAF from a compartment-maintaining network if the boundary component is included as a maintained node.

**Failure:** graph closure is representation-sensitive. Aggregating nodes can create apparent cycles; splitting a multifunctional component can destroy them. A fully internally automated engineered machine with reciprocal repair can satisfy CRDC. Thus CRDC is a candidate maintenance certificate, not a life criterion.

## 6. Candidate C — Endogenous Maintenance Certificate (EMC)

The strongest result of this specialist pass is a **conjunction**, not a new scalar.

**[CAND-C; recommended provisionally]** A model earns an **Endogenous Maintenance Certificate relative to `(mathcal B,mathcal J,Y,V,K^*,T)`** only if:

1. RCC conditions 1–5 hold;
2. CRDC conditions 1–6 hold for the maintenance-mediating set `K^*`;
3. **supply/control separation:** environmental matter/free-energy supply is allowed, but indispensable state-conditioned restorative selection is not imported solely through `J_ctrl` or `J_rep`;
4. **boundary audit:** the conclusion is reported as boundary-relative and repeated under any materially plausible predeclared alternative boundary;
5. **null comparison:** passive/no-renewal and externally maintained comparison models are evaluated with the same `Y,V,T` and observation convention.

This is best understood as a structured certificate/profile of evidence. It deliberately does not output one organization number.

## 7. Adversarial tests

| Case | RCC | CRDC | EMC | Diagnosis / false positive or negative risk |
|---|---|---|---|---|
| equilibrium crystal | fail | fail | fail | persistence/order without turnover/restorative currents |
| frozen passive structure | fail | fail | fail | persistence without active renewal |
| simple driven convection/pattern | usually fail | fail | fail | driven currents/pattern do not establish renewal-dependency closure; choice of bad `Y` can manufacture RCC-like restoration |
| externally thermostatted/feedback-controlled machine | fail when controller outside `mathcal B` | fail external-dependency clause | fail | `J_ctrl` carries state-conditioned restorative action |
| externally repaired machine | fail | fail | fail | repair/replacement enters through `J_rep` |
| simple oscillator | fail | fail | fail | recurrence is not material/constraint renewal |
| simple RAF without maintained compartment | may pass | partial/pass for catalytic nodes | fail if compartment maintenance is required in declared target | confirms RAF alone is insufficient |
| open autocatalytic network | may pass | may pass | may pass for **chemical endogenous maintenance**, not for compartmental autonomy | important scope warning: maintenance is weaker than life |
| boundary-coupled RAF / minimal reaction-compartment model of Hordijk–Steel type | plausible pass under explicit kinetics | plausible pass if boundary production/retention dependencies are represented | plausible pass, model-dependent | established RAF/boundary formalism supplies architecture, but quantitative path-level EMC requires specified kinetics |
| internally self-repairing engineered machine | pass | can pass | can pass | **strongest false-positive-for-life, but not for endogenous maintenance**; demonstrates EMC is not an organization/life definition |
| system with slow essential component turnover longer than `T` | possible fail | possible fail | possible fail | **false-negative risk** from finite horizon/time-scale choice |
| system whose maintenance is hidden by coarse-graining | possible fail | possible fail | possible fail | observation-map dependence must be reported |

## 8. Comparison

| Property | RCC | CRDC | EMC |
|---|---|---|---|
| path-level | strong | moderate; dependencies estimated from path/intervention data | strong |
| distinguishes passive persistence | yes under challenge/turnover assumptions | yes | yes |
| distinguishes external control | yes if channels typed correctly | yes if dependency provenance explicit | strongest |
| allows environmental energy/matter supply | yes | yes | yes |
| captures mutual maintenance | weak | strong | strong |
| compartment-sensitive | only if included in `Y` | explicit | explicit |
| representation dependence | medium | high | high but auditable |
| suitable as life definition | no | no | no |
| suitable G1 maintenance object | provisional | provisional | **best current candidate** |

## 9. Recommendation

**Recommendation: RETAIN PROVISIONALLY, do not canonicalize yet.**

The EMC is the strongest surviving specialist criterion because it combines:

- actual loss/turnover;
- path-level restorative currents;
- measurable effect on viability/return statistics;
- provenance of restorative control across `mathcal B`;
- mutual renewal/dependency;
- explicit allowance for raw environmental matter/free energy.

It survives the prescribed passive and externally maintained counterexamples under its stated modelling assumptions. It intentionally does **not** exclude a fully internally self-repairing engineered machine. That is a feature of scope: such a machine is endogenously maintained relative to the chosen boundary even if it is not alive. Additional organization/life components must do that later; this G1 specialist pass must not smuggle them into “maintenance.”

## 10. Exact unresolved obstruction

**[OPEN] Representation-and-boundary identifiability obstruction.** The EMC is not yet representation-independent. Its verdict depends on:

1. the predeclared boundary `mathcal B`;
2. classification of `J_sup,J_forc,J_ctrl,J_rep`;
3. the maintained variables `Y` and viability region `V`;
4. decomposition of transitions into internal mediators versus external actions;
5. the component granularity used to construct `G_M`;
6. horizon `T` relative to turnover time scales;
7. whether coarse-graining hides controller or renewal degrees of freedom.

No surveyed established theorem supplies a unique, model-independent choice of these objects. Therefore the G1 maintenance/boundary blocker is **narrowed, not resolved**.

### Minimal additional structure needed

Main Research should next define a narrower admissible system class in which:

- `mathcal B` induces an explicit state-factor or species/reaction partition;
- exchange channels are typed as physical flux, open-loop forcing, feedback signal/action, or repair/replacement;
- reaction/transition currents are identifiable;
- a viability observable and comparison dynamics are declared;
- intervention/removal of specified internal reactions/channels is mathematically well-defined;
- coarse-graining rules preserve the provenance labels needed by the certificate.

An open stochastic CRN with explicit chemostats, transport/boundary species and optional external controller channels is the most tractable first canonical test class.

## 11. End-of-pass report

1. **Files/branch/PR/commit state:** completed on branch `research/g1-specialist-endogenous-maintenance`; files changed are this specialist artifact, `sources/source-ledger.md`, `negative-results/G1_SPECIALIST_ENDOGENOUS_MAINTENANCE_FAILURES.md`, and `STATUS.md`. Pull request **#3** targets `main`. The pre-bookkeeping branch head was commit `1b634d17a48ee3603a8457b517c95aaed09fc148`; this end-of-pass bookkeeping update is the final Specialist commit.
2. **Candidate criteria examined:** RCC; CRDC; conjunctive EMC.
3. **Strongest surviving criterion:** EMC, provisionally and boundary-relative.
4. **Strongest counterexample:** a fully internally automated self-repairing engineered machine can satisfy EMC. It defeats any attempt to equate endogenous maintenance with life/organization, but not the maintenance criterion itself.
5. **Assumptions needed:** explicit boundary/channel typing; identifiable transitions/currents; predeclared viability variables/region; meaningful removal interventions; adequate observation horizon; explicit component granularity.
6. **Blocker status:** **NARROWED, NOT RESOLVED.**
7. **Main Research action:** instantiate EMC on a narrowly defined open stochastic CRN/reaction-compartment class; test boundary refinements and coarse-graining; only then decide whether any part merits canonical integration into `mathematics/definitions.md`.

## Sources

See `sources/source-ledger.md`, especially S004, S011–S014 and S017–S022.
