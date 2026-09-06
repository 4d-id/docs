# Conformance

4D-ID is a candidate standard until adopted. The current reference data runner reports **15 schema-level checks passing**. The endpoint CLI executes a smaller implemented subset and reports all other manifest entries as not run; it is a diagnostic, not a certification or full-conformance verdict.

**15 schema-level checks passing. Functional conformance work continues.** The manifest of every target test is in the [spec repo](https://github.com/4d-id/spec/blob/main/conformance/manifest.json); the partial endpoint CLI is in the [conformance repo](https://github.com/4d-id/conformance).

The 15 checks validate schema/data-level behavior only. Functional work continues, including fuller resolution, relationships, representations, provenance, merge/split/history/reconciliation, propagation, security, and domain behavior. Passing current checks is not evidence that an implementation performs perception, detection, segmentation, SLAM, VPS, localization, geometric registration, rendering, navigation, or grasp planning; those are outside 4D-ID.
