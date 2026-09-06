# Access API

The access operations (specification Clause 10) expose identity and record data supplied to a resolver. They are one semantic API with many bindings. The REST binding is described in [openapi.yaml](https://github.com/4d-id/spec/blob/main/openapi/openapi.yaml).

- `resolve` maps a supplied registry/external identifier or alias to a persistent identity.
- `get_entity`, `get_state`, `get_relations`, and `query` expose entity records, state/time, relationships, and searchable data.
- `query_events`, `get_snapshot`, `list`, and `watch` expose provenance, history, snapshots, and changes.
- `get_representations` returns representations available for a purpose; it does not render them.
- `transform` exposes/applies declared transforms supplied by participating systems; it does not perform localization or geometric registration.
- `context` returns a bounded, agent-ready description.

These operations support aliases, resolution, relationships, representations, state/time, provenance, and lifecycle operations such as merge, split, and reconciliation. They do not perform detection, segmentation, SLAM, VPS, navigation, or grasp planning.
