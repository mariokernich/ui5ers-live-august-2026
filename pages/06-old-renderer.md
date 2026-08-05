# The Old Way: Renderer API 😬

How we extended the shell before UI5 1.120

```ts
import ObjectPath from "sap/base/util/ObjectPath";

const oShellContainer = ObjectPath.get("sap.ushell.Container");
const oRenderer = oShellContainer.getRenderer();
oRenderer.addHeaderItem({
    id: "myCustomButton",
    icon: "sap-icon://action",
    text: "My Action",
    press: () => {
        // handle press
    },
}, true, false, ["begin"]); // 🤔 what do true & false mean again?
```

<div class="mt-3 grid grid-cols-2 gap-x-8 gap-y-1 text-sm">

- 😵 `controlType` and placement options **changed between releases**
- 🤯 Inconsistent header positions (`begin`, `end`, …)
- 📜 Verbose boilerplate just to add a single button
- 🔧 Hard to maintain across multiple UI5 versions

</div>

<div class="mt-3 text-lg">

It works — but it never felt clean. 🙈

</div>
