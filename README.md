# The Physics Archive — V1 Shell

A GitHub Pages-ready prototype of the Physics Archive platform shell.

## What is included

- Public navigation: Home, Learn, Explore, Solve, Practice, My Archive, About, Search
- AP Physics 1 → Kinematics course hierarchy
- Four lesson shells
- Modular lesson blocks
- Working 2D Vector Laboratory with live symbolic/spatial sync
- Motion Laboratory placeholder
- Guided Problem Decoder example
- Practice shell
- Creator/Admin dashboard
- Browser-based lesson editor with Draft / Published / Coming Soon states
- Responsive desktop/tablet/mobile styling
- Physics Archive palette and Montserrat typography

## Important: admin security

The `/admin` area in this prototype is **not production security**. It stores edits in the current browser using `localStorage`. This is deliberate: it lets us test the content workflow before connecting a real backend.

For real private creator access and cross-device publishing, the next build should connect the same UI to a backend with authentication (for example Supabase/Postgres or another CMS/API).

## Run locally

You can open `index.html` directly, but a local server is better:

```bash
python -m http.server 8000
```

Then open `http://localhost:8000`.

## GitHub Pages

Upload `index.html`, `styles.css`, and `app.js` to a repository root and enable GitHub Pages from the main branch. The app uses hash routes, so it works on GitHub Pages without server-side route configuration.

## Creator route

Open:

`#/admin`

The lesson editor saves to browser storage immediately. Use **Reset demo data** from Admin → Lessons to restore the original prototype content.
