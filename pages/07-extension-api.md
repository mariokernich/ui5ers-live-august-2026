# The New Way: Extension API ✨

Dedicated shell service since **UI5 1.120**

<div class="two-col mt-2">

<div>

```ts
const extension =
  await Container.getServiceAsync<Extension>("Extension");

const headerItem = await extension.createHeaderItem({
    id: "myHeaderAction",
    icon: "sap-icon://action",
    text: "My Action",
    press: () => { /* ... */ },
});
headerItem.showForAllApps();
```

</div>

<div class="text-sm">

- ✅ Fully async, properly typed — great with TypeScript
- ✅ `createHeaderItem()` / `createUserAction()`
- ✅ `showForAllApps()` / `showOnHome()`
- ✅ Documented, stable, dedicated service

<div class="mt-3 p-3 bg-blue-500 bg-opacity-10 rounded-lg border-l-4 border-blue-500">

**UI5 1.124+**: `FrameBoundExtension` adds footer, side pane,
sub-header, tool area & user settings entries.

</div>

</div>

</div>

<div class="mt-2 text-sm">

| | Old Renderer | Extension API |
|---|---|---|
| API stability | changed across versions 🎲 | dedicated, documented ✅ |
| Boilerplate | lots 📜 | minimal ✨ |
| Recommended for | legacy < 1.120 | everything else |

</div>
