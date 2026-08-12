# pradeepsuryad.github.io

Personal portfolio site — **Pradeep Surya Dadi, Surgical & Humanoid Robotics Engineer**.

**Live:** <https://pradeepsuryad.github.io/>

## Stack

| | |
|---|---|
| **Languages** | HTML, CSS, JavaScript (ES6) — all inline |
| **3D** | [Three.js](https://threejs.org) r128 via cdnjs |
| **Build step** | none |
| **Dependencies** | none to install — no npm, no bundler, no framework |
| **Hosting** | GitHub Pages, legacy source: `main` branch, root (`/`) |

The entire site is a single self-contained [index.html](index.html) (~110 KB):
markup, styles, animation, and the Three.js scene all live in one file. That's
deliberate — it makes the site trivially portable and means a deploy is just a
`git push`, with no build output to reconcile.

## Sections

`#top` · `#work` · `#research` · `#thesis` · `#journey` · `#lab` · `#stack` · `#contact`

Plus interactive bits: `#scene` (the Three.js canvas), `#ikhint` (an inverse-kinematics
demo hint), `#progress` (scroll progress bar), and a responsive nav (`#nav`,
`#navtoggle`, `#navlinks`).

## Local preview

No tooling required — open the file directly:

```powershell
start index.html
```

Or serve it, if you want correct relative-path and CORS behaviour:

```bash
python -m http.server 8000   # then open http://localhost:8000
```

## Deploy

```bash
git add index.html
git commit -m "Update portfolio"
git push origin main
```

GitHub Pages rebuilds automatically; the change is usually live within a minute.

## Related

- [ramudu3339.github.io](https://github.com/Ramudu3339/Ramudu3339.github.io) — a
  sibling single-file Pages site, hosted under a separate account.
