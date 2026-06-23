# 03. Agent as Cell

An AI agent can be modeled as a cell when it is a bounded runtime unit that senses
signals, uses specialized capabilities, consumes resources, produces effects, and
communicates with other units.

The analogy breaks if every agent is treated as a miniature person with an
unbounded objective. Biological cells are constrained by position, signaling,
resource availability, differentiation, and mechanisms that suppress behavior
harmful to the organism.

## Agent requirements

A cell-like agent should have:

- a narrow role and declared capability set;
- explicit inputs, outputs, and resource limits;
- a local objective connected to system-level health;
- identity and provenance for every action;
- communication through observable pathways;
- a safe failure and termination mechanism;
- no implicit authority to modify production or its own constraints.

Skills are closer to reusable expressed capabilities than to neurons. Connections
between agents and skills form a capability and signaling graph; calling it a
neural network would imply learning dynamics that may not actually exist.

## Working hypothesis

Specialization plus explicit coordination will produce more reliable adaptation
than a single general agent or a collection of agents optimized only for local
task completion.
