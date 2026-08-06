# What are Fiori Launchpad Plugins?

When people talk about UI5 development, they usually mean...

<div class="two-col mt-4">

<div>

- 📱 **UI5 Applications** — everybody knows them
- 📚 **UI5 Libraries** — reusable controls & helpers
- 🧩 **FLP Plugins** — the overlooked third option

<div class="mt-6 p-4 bg-blue-500 bg-opacity-10 rounded-lg border-l-4 border-blue-500">

**A plugin runs inside the Fiori shell** — activated once, it can apply to
<b>all</b> apps and the FLP home page itself: your own, SAP standard, even third-party UI5 apps.

</div>

<div class="mt-4 text-sm opacity-70">
⚠️ SAPUI5 only — <code>sap.ushell</code> is not part of OpenUI5
</div>

</div>

<div>

```mermaid { scale: 0.5 }
graph TD
    FLP["🚀 Fiori Launchpad Shell"]
    P["🧩 Your Plugin<br/>(loaded once at startup)"]
    A1["📱 SAP Standard App"]
    A2["📱 Your Custom App"]
    A3["📱 Third-Party App"]

    P -. extends .-> FLP
    FLP --> A1
    FLP --> A2
    FLP --> A3

    style P fill:#3b82f6,color:#fff
    style FLP fill:#1e293b,color:#fff
```

</div>

</div>
