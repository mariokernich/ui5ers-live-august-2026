# New Generator for Fiori Launchpad Plugins

> Building Fiori Launchpad Plugins with TypeScript & the Extension API
>
> **UI5ers live · August 2026**

This repository contains the presentation for the UI5ers live session on the new
**`generator-ui5-ts-flp-plugin`** — an [Easy-UI5](https://github.com/ui5-community/generator-easy-ui5)
generator for scaffolding **Fiori Launchpad plugins** with **TypeScript**, built as
a [Slidev](https://sli.dev/) slide deck.

---

## 📑 What the talk covers

1. **What are Fiori Launchpad Plugins?** — the overlooked third option in UI5 development
2. **Plugin Architecture** — a component without views, powered by shell services
3. **Old vs. New** — from the legacy Renderer to the modern Extension API (UI5 1.120+)
4. **The Generator** — `generator-ui5-ts-flp-plugin` in the UI5 community
5. **Live Demo** — scaffold, run & extend a plugin locally
6. **Deployment & Wrap-up** — getting your plugin into ABAP FLP / Build Work Zone

---

## ▶️ Run the presentation locally

The deck lives in [`slides.md`](./slides.md), which stitches together the
individual slides stored in [`pages/`](./pages). Reusable assets are in
[`components/`](./components) and [`images/`](./images).

```bash
npm install      # or: pnpm install
npm run dev      # starts Slidev and opens http://localhost:3030
```

### Scripts

| Command          | Description                                  |
| ---------------- | -------------------------------------------- |
| `npm run dev`    | Start the live presentation server           |
| `npm run build`  | Build a static version of the deck (`dist/`) |
| `npm run export` | Export the slides to PDF                     |

Learn more about Slidev in the [documentation](https://sli.dev/).

---

## 📁 Repository structure

```
├── slides.md            # Slidev entry point (imports pages/*)
├── pages/               # Individual slides (01-title.md … 99-thank-you.md)
├── components/          # Vue components used in slides
├── images/              # Slide images / logos
├── style.css            # Global slide styles
└── package.json         # Slidev scripts & dependencies
```

---

## 🔗 Links

- Slidev — https://sli.dev/
- Easy-UI5 — https://github.com/ui5-community/generator-easy-ui5
- SWAN GmbH — https://swan.de
