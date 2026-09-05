# What 4D-ID is

Spatial computing runs on frames that do not line up: maps, headsets, robots, game engines, and 3D scans each track space their own way, and none of them agree. The fix is not a new coordinate system on top. It is a shared **name**, so all of them can point at the same thing while keeping their own coordinates.

Four concepts carry the whole standard:

- **Identity** — a persistent, opaque name for a thing, unchanged as it moves or is re-observed.
- **Hierarchy** — a strict tree of frames from a domain root through local coordinate systems.
- **Pose** — position and orientation relative to the parent, as GeoPose, with uncertainty.
- **Time** — source, publish, and receive timestamps with an uncertainty bound.

Everything else in the standard is a rule about how those four behave under a named pressure, or a binding to a standard that already exists.
