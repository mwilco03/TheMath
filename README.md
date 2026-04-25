# TheMath — Quick Tip

A single static page that demonstrates the **mirror &amp; slide** trick for
calculating a tip in your head.

Live page: served from `main` via GitHub Pages → `index.html`.

## The trick

1. **Write the bill** into a row of digit cells.
2. **Mirror** that row onto the line below.
3. **Slide** the mirrored row one cell to the right — that's `× 0.1`, i.e. **10%** of the bill.
4. **Mirror** the 10% row once more.
5. **Add** the two 10% rows column by column → **20% tip**.
6. Want **15%**? Take the midpoint of the bill row and the 20% row (or halve 10% and add).

The page renders the math symbols (`·`, `+`, `=`) inline with the grid so the
operation is visible, not hidden behind a calculator.

## Run it

It's a single file. Open it directly:

```sh
open index.html        # macOS
xdg-open index.html    # Linux
start index.html       # Windows
```

…or serve the folder:

```sh
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deploy

GitHub Pages → **Settings → Pages → Source: `main` / `(root)`**. No build step.

## Files

- `index.html` — the whole app (HTML + CSS + JS, no dependencies).
