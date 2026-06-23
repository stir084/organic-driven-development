# Experiment 001: Vital Loop

## Objective

Build a small service that detects its own degraded state, explains the evidence,
recalls relevant past incidents, and recommends a reversible recovery action to a
human.

The first version must not modify production automatically. The purpose is to test
whether the ODD model improves diagnosis and recovery, not to demonstrate maximum
autonomy.

## Loop

```text
observe -> detect -> diagnose -> remember -> propose -> human decision
   ^                                                        |
   |                                                        v
   +------------------- verify <- act or simulate <---------+
```

## Minimal system

Use one deliberately small HTTP service with:

- request latency, error rate, throughput, saturation, and dependency health;
- structured logs and a small incident-memory store;
- reproducible fault injection such as latency, dependency failure, or resource
  exhaustion;
- a diagnostic agent that can read only the supplied evidence;
- a verifier that checks claims against raw observations;
- a human-readable report containing uncertainty and a reversible action.

## Safety boundary

The agent may observe, retrieve memory, diagnose, and propose. It may run approved
tests in an isolated environment. It may not deploy, modify production data,
change its constraints, or suppress evidence.

## Hypotheses

H1. A diagnosis using connected vital dimensions and incident memory identifies
the injected fault more accurately than a threshold alert alone.

H2. Independent evidence verification reduces unsupported diagnostic claims.

H3. A structured recovery proposal reduces human time to choose a safe action.

## Measurements

- fault identification accuracy;
- time to useful diagnosis;
- unsupported-claim rate;
- correct evidence citation rate;
- recovery-action acceptance rate;
- time to restore the viable range;
- false-positive and unnecessary-intervention rates;
- human review time.

## Baselines

Compare at least:

1. conventional metric thresholds;
2. a single diagnostic agent without memory or verification;
3. the complete Vital Loop.

## Success criterion

The experiment supports further work only if the complete loop improves recovery
quality or review time without materially increasing false interventions. If it
does not, record the result and revise or reject the relevant ODD claim.

## Deferred work

- automatic production repair;
- agents that rewrite their own governance;
- a universal vitality score;
- multi-service and multi-agent ecosystems;
- financial-market vitality models.

These are later experiments, not prerequisites for testing the first claim.
