# G1 Organization-Component Discrimination Matrix

**Scope:** G1 admitted/canonical test domains and accumulated counterexample family.  
**Status:** canonical G1 analysis artifact; entries are model-class expectations, not universal theorems.

## Retained profile axes

\[
\mathfrak O_{\mathcal S}(\ell,\tau)
=
\{O_{\rm maint},O_{\rm cat},O_{\rm dep},O_{\rm hered},O_{\rm spatial},O_{\rm robust},O_{\rm xscale}\}_{\ell,\tau}.
\]

Legend: **H** high/present is possible/characteristic; **L** low/absent in the clean model; **V** variable; **N/A** outside component domain.

| Counterexample/model | \(O_{\rm maint}\) | \(O_{\rm cat}\) | \(O_{\rm dep}\) | \(O_{\rm hered}\) | \(O_{\rm spatial}\) | \(O_{\rm robust}\) | \(O_{\rm xscale}\) |
|---|---:|---:|---:|---:|---:|---:|---:|
| equilibrium crystal/frozen order | L | L | L | N/A | H | H | V |
| random/high-entropy state | L | L | L | N/A | L | L | L |
| simple oscillator | L | L | V | N/A | L | H | L |
| convection/turbulence | L | L | V | N/A | H | V | H |
| passive correlated system | L | L | L/V | N/A | V | V | V |
| static information archive | L | L | L | N/A | V | H | L/V |
| externally controlled/repaired machine | L endogenous | L/V | V/H external | N/A/V | V | H | V |
| internally self-repairing engineered machine | H | L/V | H | N/A/V | V | H | V/H |
| bare/open autocatalytic network | V | H | H catalytic | N/A | L | V | V |
| compartment-maintaining reaction network | H | H/V | H | N/A/V | H | V/H | V/H |
| replicator/heritable system with weak self-maintenance | L/V | V | V | H | L/V | V | V |
| reaction-compartment with heredity | H | H/V | H | H | H | V/H | H/V |

## Removal audit

| Axis removed | Lost distinction | Result |
|---|---|---|
| maintenance | endogenous renewal vs passive/external persistence | retain |
| catalysis | chemical collective production vs noncatalytic maintenance/control | retain on chemical domain |
| dependency closure | intervention-backed mutual support vs correlation/catalytic membership alone | retain |
| heredity | cross-generation/transmission structure vs within-trajectory persistence | retain conditionally |
| spatial/compartment | bare autocatalysis vs maintained localization/boundary organization | retain |
| robustness | fragile vs perturbation-resistant realization at similar architecture | retain |
| cross-scale | matched single-scale profiles with different interscale dependence | retain |

No retained axis is sufficient for organization/life; each admits high-valued nonliving cases. Minimality is relative to this admitted model/counterexample class.
