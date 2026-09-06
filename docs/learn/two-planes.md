# The two planes

**Identity is shared; records and representations remain contextual.**

The **identity plane** is shared and durable: persistent IDs, aliases, relationships, resolution, and lifecycle events such as merge, split, and reconciliation.

The **data plane** is contextual: supplied state and time, provenance, coordinate/frame references, and representations selected for a purpose. Systems can disclose, cache, or serve different data while still referring to the same identity.

Both planes begin with observations or records supplied by upstream systems. 4D-ID does not detect or segment entities, localize them, perform SLAM/VPS or geometric registration, render content, navigate, or plan grasps.

This is the same separation that made the web work: everyone can resolve the same name, while each system controls the records and representations it stores, serves, or presents.
