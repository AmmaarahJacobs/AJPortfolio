# Project folders

Every folder in here is a project that lives outside GitHub. The portfolio page
lists them first in the **Selected work** grid, which is built from the
`LOCAL_PROJECTS` array at the bottom of `index.html`.

## Adding a project

1. Create a folder named after the project, e.g. `projects/openvision/`.
2. Drop in a cover image: `cover.jpg` (or `.png`), roughly 1600×1200 — a 4:3
   screenshot or mockup works best. Without one, the card shows the project's
   initials instead, so an image is optional.
3. Add an object to `LOCAL_PROJECTS` in `index.html`:

```js
{
  title: "OpenVision",
  status: "In progress",        // "In progress", "Case study", "2025" …
  year: "2026",
  category: "Web · AI",         // short label next to the status
  summary: "Two or three sentences on the problem and what you built.",
  stack: ["Java", "MySQL"],     // rendered as "Java · MySQL"
  cover: "projects/openvision/cover.jpg",
  links: [
    { label: "Case study", href: "" },          // empty href = hidden
    { label: "Live site", href: "https://…" }
  ]
}
```

The section hides itself automatically if the list is empty, and any entry
without a `title` is skipped.

## What to keep in each folder

Suggested contents, so the folder is a complete case study rather than just
assets:

```
projects/openvision/
  cover.jpg        main card / hero image
  README.md        what it is, the problem, the stack, what you learned
  screens/         additional screenshots, referenced from the README
```

Keep an image under about 500 KB so the page stays quick on mobile.
