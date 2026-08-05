# Deployment & Activation 🚀

It deploys like any UI5 app — plus one manifest flag

```json
"sap.flp": {
  "type": "plugin"
}
```

<div class="two-col mt-4">

<div>

### 🏢 On-Premise (ABAP FLP)

<div class="text-sm mt-2">

Deploy as BSP / UI5 application, then either:

- **Global**: `/UI2/FLP_CONF_DEF` + `/UI2/FLP_CUS_CONF` → every user gets the plugin
- **Role-based**: target mapping `Shell-plugin` in a catalog + PFCG role → only authorized users

</div>

</div>

<div>

### ☁️ SAP Build Work Zone

<div class="text-sm mt-2">

- Deploy as HTML5 app (MTA → BTP)
- Refresh the HTML5 Apps content channel
- Add via Content Explorer & assign to a role

</div>

<div class="mt-3 p-3 bg-blue-500 bg-opacity-10 rounded-lg border-l-4 border-blue-500 text-sm">

No tile required — the plugin loads automatically when users open the launchpad. 🪄

</div>

</div>

</div>

<div class="mt-4 text-center opacity-80">

**Cross-app requirement? A plugin is very likely the right tool for the job.**

</div>
