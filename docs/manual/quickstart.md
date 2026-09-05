# Quickstart

The first four calls against a running resolver:

```bash
resolve(registry, id)      -> 4did:…
context(4did)              -> a compact, agent-ready description
get_representations(4did)  -> the right model for the job
watch(4did)                -> changes as they happen
```

Run the resolver locally, then hit it:

```bash
git clone https://github.com/4d-id/reference-resolver
cd reference-resolver && npm install && npm start
curl "localhost:4141/resolve?registry=asset.register&external_id=TB-WH-01"
```
