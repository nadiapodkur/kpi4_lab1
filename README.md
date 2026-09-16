# UI Elements — Lab 1
# Nadiia Podkur IP-41

A single reference page that catalogs ten common UI elements. For each one there's a plain-language explanation of what it is and when to use it, plus a working live example.

## Files

| File | Purpose |
|---|---|
| `index.html` | Page structure and content — one section per UI element |
| `style.css` | All styling |

## Elements covered

1. Radiobutton
2. Checkbox
3. Text input
4. Tabs
5. Buttons
6. Text label
7. Link
8. Tooltip
9. Dropdown list
10. Data grid

## Running it

No build step or dependencies — it's plain HTML/CSS/JS.

- **Quickest:** double-click `task.html` to open it in any modern browser.
- **In VS Code:** install the **Live Server** extension, right-click `task.html`, choose "Open with Live Server". This is the better option here, since the page loads fonts from Google Fonts over the network.

## Publishing

To submit a link as the assignment asks:

1. Create a public GitHub repository and push `task.html` and `style.css` to it (keep them in the same folder, since `task.html` links to `style.css` by relative path).
2. In the repo settings, enable **GitHub Pages** (Settings → Pages → Deploy from branch → `main`, root folder).
3. GitHub will generate a link like `https://<username>.github.io/<repo-name>/` — submit that link.

## Notes on implementation

- **Tabs** (#4) use a small vanilla JavaScript snippet at the bottom of `task.html`: clicking a tab button toggles an `active` class on itself and on the matching panel, and CSS shows only `.tab-panel.active`.
- **Tooltip** (#8) shows two approaches: a custom CSS tooltip (`.has-tooltip` / `.tooltip-bubble`, shown on hover *and* keyboard focus for accessibility) and the native browser tooltip via the `title` attribute.
- **Data grid** (#10) is a plain HTML `<table>` — enough to demonstrate the concept without pulling in a grid library.
- Every input has a properly associated `<label for>`, and interactive elements have a visible focus outline, for basic keyboard accessibility.
