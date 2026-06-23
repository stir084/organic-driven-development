# 05. Software Vital Signs

Vital signs are observable proxies for a system's ability to remain viable. They
are not a mystical “life score,” and they should not be collapsed into one number
before their meaning and tradeoffs are understood.

## Candidate dimensions

| Dimension | Question | Example signals |
| --- | --- | --- |
| Function | Is the system fulfilling its promises? | success rate, correctness, SLOs |
| Stress | How much pressure is it absorbing? | saturation, queue growth, error bursts |
| Recovery | Can it return to a viable range? | MTTR, rollback success, recovery slope |
| Adaptability | Can it respond safely to change? | lead time, change failure rate, reversibility |
| Coherence | Do the parts still honor shared intent? | contract violations, policy drift, contradictions |
| Memory | Does it retain operational learning? | repeated incidents, retrieval quality, decision provenance |
| Cooperation | Do local actions improve the whole? | handoff failures, resource conflict, global side effects |
| Trust | Are behavior and change accountable? | unexplained actions, approval coverage, audit completeness |

Each system needs a viable range rather than a universal target. Extremely low
change frequency may indicate stability or inability to adapt; high redundancy may
increase resilience or unsustainable cost. Interpretation requires context.

## From signals to diagnosis

1. Observe raw evidence without an LLM rewriting it.
2. Derive transparent metrics and trends.
3. Let an agent form a diagnosis with cited evidence and uncertainty.
4. Compare the diagnosis with baselines and alternative explanations.
5. recommend a reversible intervention.
6. measure whether the system returned to its viable range.

AI can combine heterogeneous signals and generate hypotheses. It does not make a
signal valid by naming it “vitality.” Validity comes from operational definitions,
predictive or explanatory evidence, and repeatable outcomes.

## Initial research question

Can a connected set of vital signs detect degradation and recommend a successful
recovery earlier than conventional threshold alerts, without increasing harmful
or noisy interventions?
