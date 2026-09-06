# What 4D-ID is

## Where it starts

4D-ID starts after perception or an existing data system has produced an observation or record. In the pipeline **OBSERVE → GROUND → IDENTIFY → RESOLVE → INTEROPERATE**, observation and grounding are upstream inputs; 4D-ID provides the persistent identity, resolution, and interoperability layer. Grounding determines the referent; localization estimates where it is; 4D-ID preserves which thing that referent is across records and systems.

An observation is evidence or a record about something; it is not the persistent identity itself.

- **OBSERVE** — upstream sensors, applications, or data systems produce observations.
- **GROUND** — an upstream system associates an observation with supplied coordinates, frames, or external records. 4D-ID can carry those references; it does not estimate them.
- **IDENTIFY** — assign a persistent identity and preserve aliases for the same entity.
- **RESOLVE** — resolve aliases and external identifiers, expose relationships and state, and reconcile identity claims.
- **INTEROPERATE** — share representations, time/state, provenance, and lifecycle history across systems.

## What it provides

- persistent identity and aliases;
- resolution across registries and vendor boundaries;
- relationships between entities;
- representations selected for a purpose;
- state and time, with provenance;
- merge, split, history, and reconciliation semantics.

4D-ID is not a perception or robotics stack. It does **not** perform detection, segmentation, SLAM, VPS, localization, geometric registration, rendering, navigation, or grasp planning. SEGS is adjacent, not core.

Spatial coordinates, poses, and transforms may be represented when supplied by another system; 4D-ID does not compute localization or geometric registration.

## Adjacent grounding services

A **Spatial Entity Grounding Service (SEGS)** is an implementation pattern that turns observations into grounded entity hypotheses: detect or segment → classify → track or re-identify → localize in 3D → match known entities → propose an existing or candidate 4D-ID. SEGS is adjacent to 4D-ID, not part of the core candidate standard; 4D-ID records and resolves the accepted identity and its evidence.
