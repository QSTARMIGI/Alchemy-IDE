# Alchemy IDE

**Alchemy IDE** is an experimental MIGI satellite project for authoring explainable, permission-aware workflows.

Its intended role is to help developers and creators design workflows that connect symbolic intent, typed schemas, policy checks, tools, models, receipts, and user interfaces.

> This repository is a development workspace. It does not claim that every planned capability is implemented or production-ready.

## Relationship to MIGI Core

MIGI Core defines the authority and provenance boundaries:

```text
Original → Observation → Authority → Execution → Receipt
```

Alchemy IDE is intended to make those workflows visible and editable:

```text
Symbolic intent
  ↓
Typed workflow graph
  ↓
Policy validation
  ↓
Tool / model / service execution
  ↓
MUEF event + MIGIReceipt
```

## Intended Building Blocks

- visual workflow authoring;
- Emoji A++ or symbolic command parsing;
- typed event and receipt schemas;
- policy linting before execution;
- tool and model capability registry;
- replayable execution graphs;
- debugging views for authority and provenance;
- adapters that keep external services behind explicit permission boundaries.

## Engineering Rules

- Do not represent simulations as verified observations.
- Keep policy evaluation separate from model inference.
- Require explicit authority for consequential actions.
- Preserve third-party licenses and attribution for dependencies or borrowed code.
- Link durable execution changes to MUEF events and MIGIReceipt records where applicable.

## Status Labels

Use these labels in documentation and issues:

```text
implemented
prototype
planned
research
upstream dependency
```

## Canonical Reference

Architecture, shared trust primitives, and the MIRROR SEED MVP backlog live in [QSTARMIGI/MIGI](https://github.com/QSTARMIGI/MIGI).
