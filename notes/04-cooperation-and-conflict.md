# 04. Cooperation and Conflict

ODD chooses cooperation as a value, but biology does not divide neatly into
competitive cells and cooperative genes. Cooperation and conflict occur at
multiple levels. The formation of multicellular individuality required mechanisms
that aligned lower-level behavior and mediated internal conflict.

This distinction matters for software. Adding more agents does not create an
organism. A coherent system also needs boundaries, shared signals, division of
labor, resource allocation, and mechanisms that prevent local success from
damaging the whole.

## Engineering translation

| Biological problem | Software question |
| --- | --- |
| Uncontrolled proliferation | Can an agent create work or consume resources without limits? |
| Failure of differentiation | Are agent responsibilities distinct and enforceable? |
| Resource conflict | Who allocates tokens, compute, time, and human attention? |
| Signal corruption | Can observations and reports be traced and verified? |
| Immune overreaction | Can recovery automation cause more damage than the incident? |
| Organism-level fitness | What prevents a local metric from harming users or the system? |

## Conflict mediation mechanisms

- scoped authority and resource budgets;
- shared health objectives with explicit tradeoffs;
- independent verification for consequential proposals;
- isolation, rollback, and termination;
- human arbitration for value conflicts;
- memory of failed changes and their context.

Competition may still be useful for generating alternative hypotheses or designs.
Selection should occur in a safe evaluation environment, while production behavior
remains cooperative and governed.

## Biological grounding

- Michod and Roze describe conflict mediation as necessary for the emergence and
  continued health of multicellular individuality:
  <https://pubmed.ncbi.nlm.nih.gov/11298810/>
- Ratcliff and colleagues experimentally observed multicellular clustering,
  division of labor, and group-beneficial programmed cell death in yeast:
  <https://pubmed.ncbi.nlm.nih.gov/22307617/>
- Traulsen and Nowak model how cooperation can be favored through multilevel
  selection:
  <https://pmc.ncbi.nlm.nih.gov/articles/PMC1544155/>
