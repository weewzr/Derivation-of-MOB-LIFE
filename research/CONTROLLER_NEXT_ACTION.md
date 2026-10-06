# Controller Assignment — G1 Main Research Pass 2: Canonical Test Class

**Role:** Main Research  
**Gate:** G1 — Mathematical Definition  
**Authorization:** ACTIVE  
**G1 remains IN PROGRESS. G2 is not authorized.**

Read `MASTER_INSTRUCTIONS.md`, `STATUS.md`, G1 Pass 1, and `research/G1_SPECIALIST_ENDOGENOUS_MAINTENANCE.md` before starting.

## Controller assessment

The Specialist result is accepted as substantive G1 input. The provisional Endogenous Maintenance Certificate (EMC), combining the Restoration-Current Criterion (RCC) and Closed Renewal-Dependency Criterion (CRDC), has **not** earned universal canonical status.

The remaining blocker is representation/boundary identifiability.

## Single objective

Define and analyze the **narrowest useful canonical test class** on which the provisional EMC becomes mathematically well-posed and auditable.

Start with the Specialist recommendation: an **open stochastic chemical reaction network / reaction-compartment class** with explicit chemostats, transport/boundary species, optional external controller/repair channels, identifiable reaction currents, viability variables, and declared observation maps.

Do not attempt to cover all physical systems in this pass.

## Required work

1. Give a precise mathematical definition of the proposed test class: species/state space, stochastic dynamics/generator or equivalent, reactions/stoichiometry, chemostats/reservoirs, system boundary, exchange channels, controller/repair channels, path law and observation horizon.

2. Define non-circular rules for typing channels as supply, forcing, external feedback/control, external repair/replacement, or internal process-mediated transitions.

3. Define a predeclared viability observable/region and degradation/loss transitions without defining them by the desired EMC outcome.

4. Instantiate RCC, CRDC and EMC explicitly on this class. State every assumption required for reaction removal/intervention and for dependency edges.

5. Construct at least a small family of explicit model cases representing:
   - passive/no-renewal persistence;
   - externally maintained/controlled persistence;
   - open autocatalytic chemistry without maintained compartment;
   - reaction-compartment/endogenous-maintenance candidate;
   - internally self-repairing engineered analogue where representable.

Analytical examples are preferred; computation may be used only as lightweight support if it does not constitute premature G9 work.

6. Test boundary refinement and at least one coarse-graining/observation change. Determine exactly which provenance labels and dependency relations must be preserved for an EMC verdict to remain meaningful.

7. Decide which parts, if any, have earned canonical status. Only promote definitions that survive these tests into `mathematics/definitions.md` and `mathematics/notation.md`. Keep EMC provisional if its remaining dependence is still scientifically material.

8. Update provenance and negative results.

## G1 completion audit

At the end, reassess all G1 prerequisites, not just maintenance:

- admissible system class;
- explicit system/environment boundary;
- dynamics/path law;
- spatial and temporal scales;
- observation/coarse-graining maps;
- canonical notation;
- candidate organization profile/components;
- endogenous-maintenance object;
- distinction from information, dissipation, correlation, persistence and externally maintained control;
- counterexample resistance.

Do not mark G1 complete merely because the test class works. If G1 remains incomplete, identify the **single precise remaining blocker**.

## Deliverable

Create `research/G1_PASS_2_CANONICAL_TEST_CLASS.md`, update relevant canonical files only where earned, update `STATUS.md`, source ledger and negative results, and use the repository branch/PR workflow.

## End-of-pass decision report

Report the canonical test class, EMC outcome, definitions promoted/rejected, strongest counterexample, coarse-graining/boundary result, whether G1 is genuinely complete, and the single highest-value next action.

Stop. Do not enter G2 and do not perform an Independent Review unless subsequently authorized by the Workflow Controller.
