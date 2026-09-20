# Mini Projects — HTML, CSS, and JavaScript

Small, single-purpose front-end exercises. Each project is three files — `main.html`, `main.css`, `main.js` — with no dependencies, no build step, and no framework.

## Why this exists

Each project isolates one browser technique so it can be learned without anything else in the way:

| Project | Technique |
| --- | --- |
| **Blurry Loading** | Mapping scroll or load progress onto a CSS `filter: blur()` value, driven by JavaScript |
| **Expanding Cards** | CSS `flex-grow` transitions toggled by class, with click handlers managing the active state |

The constraint is the point: no libraries, no bundler, nothing to install. Open the file and it runs.

## Running them

Open the HTML file in a browser:

```bash
cd "Blurry Loading" && start main.html      # Windows
cd "Blurry Loading" && open main.html       # macOS
cd "Blurry Loading" && xdg-open main.html   # Linux
```

Or serve the repository over HTTP if you would rather browse it:

```bash
python -m http.server 8000
```

Folder names contain spaces, so quote them in the shell.

## Structure

```
Blurry Loading/
  main.html    markup
  main.css     styles and transitions
  main.js      behaviour
Expanding Cards/
  ...same three files
```

Same shape every time, so the diff between two projects is only the technique being practised.

## Notes

- Pure static files. No `npm install`, no build, no server required.
- Images are loaded from external URLs, so the pages need an internet connection to render fully.
- These are practice exercises rather than components meant to be dropped into a real project — though the CSS in both is worth borrowing.
