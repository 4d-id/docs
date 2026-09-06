# Quickstart

4D-ID consumes an existing external identifier or record. It does not observe, detect, segment, localize, register geometry, render, navigate, or plan grasps.

The first access operations against a running resolver:

```bash
resolve(registry, external_id) -> 4did plus aliases
get_state(4did)                -> supplied state/time and provenance
get_relations(4did)            -> related entities
get_representations(4did)      -> representations available for a purpose
watch(4did)                    -> identity and record changes as they happen
```

Run the resolver locally, then resolve an identifier that is already registered:

```bash
git clone https://github.com/4d-id/reference-resolver
cd reference-resolver && npm install && npm start
curl "localhost:4141/resolve?registry=asset.register&external_id=TB-WH-01"
```

`resolve` is lookup, not perception: the resolver maps a supplied registry/external ID to a persistent identity. Merge, split, history, reconciliation, and provenance are part of the identity record and its lifecycle; see the specification for their normative semantics.
