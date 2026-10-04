# MASTER INSTRUCTIONS — MOB-LIFE

## 1. Purpose

MOB-LIFE investigates whether rigorous multiscale mathematical bounds can constrain transitions from driven matter to organization, self-maintaining organization, proto-life, and evolvable life.

The programme does not begin by proving a preferred theory of life. It seeks progressively stronger, auditable mathematical statements and explicit residual obstructions.

## 2. Canonical record

This GitHub repository is the durable source of truth. Chat discussions, private notes, and external documents are not repository evidence unless migrated with provenance. Do not overwrite prior research silently.

Before substantive work, inspect this file, `STATUS.md`, relevant definitions/notation, source ledgers, research artifacts, and recent relevant commits.

## 3. Null programme first

The programme begins from

```text
H_0 = known physics/chemistry, using established mathematics.
```

Known physics/chemistry is the null programme. An unknown organizing field `Phi` MUST NOT be assumed, smuggled into definitions, or introduced as necessary.

A candidate `Phi` extension may be considered only after the known-physics programme has been developed sufficiently and a precise residual obstruction survives. Any such extension must be minimal, explicit, falsifiable where possible, and compared against the strongest conventional mechanism capable of the same function.

## 4. Gate control

The gate sequence is:

- **G0 — Repository Foundation**
- **G1 — Mathematical Definition**
- **G2 — Candidate Organization Bound**
- **G3 — Regular/Special Case**
- **G4 — Exhaustive Case Decomposition**
- **G5 — Known-Physics Bound**
- **G6 — Residual Obstruction**
- **G7 — Candidate Phi Extension**
- **G8 — Mathematical Derivation**
- **G9 — Computational Verification**
- **G10 — Experimental Implications**

Gates advance only when substantive prerequisites have been satisfied and recorded. A number of research passes, volume of notes, promising intuition, or elapsed time never constitutes gate completion. Gate transitions must update `STATUS.md`; important transitions should receive independent review.

Do not perform work belonging to a later gate merely because its tools or hypotheses are available.

## 5. Methodological inspiration: Wang–Zahl

The Wang–Zahl Kakeya programme is methodological inspiration, **not a claimed mathematical equivalence**.

Potentially reusable ideas include:

- preservation of multiscale information;
- structured special or regular cases;
- exhaustive case decomposition;
- multiple complementary techniques;
- quantitative obstruction measures;
- incremental quantitative improvements;
- bootstrap or induction-on-scale reasoning where mathematically justified.

Do not force Kakeya terminology, objects, proof machinery, or analogies onto organization or life without a legitimate mathematical correspondence.

## 6. Organization discipline

Do not prematurely collapse organization into a single arbitrary scalar. At G1, candidate organization objects should preserve relevant spatial and temporal scales and distinguish potentially different components such as correlation, spatial/temporal structure, topology, network structure, catalysis, memory, information, and closure when mathematically justified.

Energy, organization, information, and constraint are not interchangeable concepts.

## 7. Epistemic labels

Every material research statement should be identifiable as one of:

- **[DEF] Definition** — stipulated mathematical/scientific meaning used by the project.
- **[ASM] Assumption** — premise adopted for a stated argument or model.
- **[EST] Established theorem/result** — externally established mathematical or scientific result, with provenance.
- **[EMP] Empirical observation** — reported observation or measurement, with provenance.
- **[CONJ] Conjecture** — proposition asserted as plausible but unproved.
- **[HEUR] Heuristic** — intuition, analogy, scaling argument, or informal guide.
- **[CAND] Candidate construction** — proposed object, bound, decomposition, model, or proof device not yet established.
- **[OPEN] Unresolved question** — explicit unknown or unresolved obstruction.

Historical/philosophical material and scientifically contested claims should additionally be identified as such rather than presented as established modern science.

## 8. Provenance

External scientific and mathematical claims require citations/provenance. Prefer original papers/texts, authoritative scholarly editions, peer-reviewed reviews, major monographs, and institutional sources over unsourced summaries.

Important equations/results should eventually record: stable identifier; domain; symbol definitions; units where applicable; assumptions; validity regime; epistemic class; primary/authoritative source; role in MOB-LIFE; limitations; and competing interpretations where relevant.

Original-language research is encouraged where materially useful. Translation, historical meaning, and modern analogy must not be silently conflated.

## 9. Notation and derivation standards

Notation must be defined before substantial use and kept consistent across the repository. Canonical notation belongs in `mathematics/notation.md`; canonical definitions belong in `mathematics/definitions.md`.

Important derivations must expose assumptions and intermediate steps. Do not jump from suggestive equations to conclusions. Record domains, boundary/initial conditions, approximation regimes, dimensional constraints, and dependencies where applicable.

Negative results, failed approaches, counterexamples, and exclusions must be retained when scientifically informative.

## 10. Obstruction-first known-physics programme

Research should identify explicit obstruction families and map known techniques against them. Prefer independent or redundant controls where possible.

Before new physics is considered, ask what the strongest result obtainable from known physics/chemistry and established mathematics actually is. G6 must identify a precise residual obstruction; absence of such an obstruction blocks G7.

## 11. Case and multiscale architecture

Preserve information across multiple spatial and temporal scales rather than prematurely reducing the problem to a coarse/fine dichotomy.

Candidate case axes may include scale regularity, geometry, dynamical regime, network regime, and organization mechanism. The eventual decomposition should cover every materially distinct nonempty case directly or by justified reduction.

## 12. Repository layout and workflow

- `research/`: scoped research passes and architecture.
- `mathematics/`: definitions, notation, cases, derivations.
- `sources/`: source ledger and provenance.
- `computation/`: future code/data/results under appropriate gates.
- `reviews/`: independent reviews and repository audits.
- `negative-results/`: informative failed or excluded approaches.

A substantive pass should identify a precise question, inspect repository state, research authoritative sources, classify evidence, expose assumptions, compare conventional mechanisms, map results into the architecture, update provenance and status, and state the highest-value next action.

## 13. Scientific attitude

The programme succeeds if known physics closes the relevant chain, if a rigorous bound is weaker than hoped, or if `Phi` proves unnecessary or unsupported. Prefer precise uncertainty, falsifiable mechanisms, and incremental rigorous bounds over grand conclusions.