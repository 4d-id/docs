# Use the JS SDK

The SDK works with identities and records already observed or registered by another system. It does not perform detection, segmentation, SLAM, VPS, localization, geometric registration, rendering, navigation, or grasp planning.

```bash
npm install @4d-id/js
```

```js
import { Client } from "@4d-id/js";

const api = new Client("http://localhost:4141");
const { id } = await api.resolve({
  registry: "asset.register",
  external_id: "TB-WH-01",
});
const state = await api.state(id);
const relations = await api.relations(id);
const representations = await api.representations(id, "rendering");
```

Client-side minting is also available for identities derived from caller-supplied data; minting does not detect or localize an entity. `representations` returns available/ranked representations; the SDK does not render them.

Full API in the [js-sdk README](https://github.com/4d-id/js-sdk).
