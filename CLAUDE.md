# Student Names

Flashcards for learning students' names from their photos, one tab per class. A teaching tool
Ross uses himself — not a student-facing activity.
Live at <https://rossdavilla.github.io/Names/>.

## Layout

```
index.html           the whole app — one self-contained file, no build step
classes.js           the class list: one entry per class, pointing at a photo folder
photos/<class-id>/   that class's photos, one per student
```

See `README.md` for the keyboard and swipe controls and how the Learning/Learned bins work.

## Adding a class

Resize the photos, put them in `photos/<class-id>/`, and add an entry to `classes.js`. Nothing
else is generated, so that is the whole change.

## ⚠️ Student photos — this repo is public

Every photo here is a real student's face, and GitHub Pages serves the whole repository
publicly. That is already true of what is committed, but it means:

- **Never add student names, emails, IDs or grades** to `classes.js` or anywhere else in the
  repo beyond the first names the flashcards need.
- Keep this app out of any public listing. It is already in the
  [`rossdavilla.github.io`](https://github.com/rossdavilla/rossdavilla.github.io) directory under
  the `tools` tag with **`"shot": { "none": true }`** so the screenshotter never captures a
  student's face. Leave that flag in place, and set the same flag on any new app whose screen
  would show student photos or data.
- If Ross asks to publish or share a page from this repo, point the risk out before doing it.

## Publishing

GitHub Pages serves `main` from the repository root, so a push to `main` is the deploy.
