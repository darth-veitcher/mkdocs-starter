# Embedding draw.io

The template for this project has a modified `footer` which can be found at [docs_src/theme/partials/footer.html](https://github.com/darth-veitcher/mkdocs-starter/blob/master/docs_src/theme/partials/footer.html). This draws on the excellent work by [sakumikko](https://github.com/sakumikko/mkdocs-drawio) and loads a javascript viewer for interactively rendering any linked draw.io xml file in the browser. No need to export or convert diagrams to svg/png.

To use draw.io diagrams inside the documentation use the following syntax.

```html
<div class="dynamic-graph" data-mxgraph-path="mydiagram.drawio"></div>
```

It will show up as per below.

<div class="dynamic-graph" data-mxgraph-path="diagrams/gcp.drawio"></div>

## File locations

The `.drawio` file is passed in as `data-mxgraph-path` relative to the documentation root. For example a simple, flat structure like this results in `data-mxgraph-path="gcp.drawio"` (because it is at the root of the site with the index).

```null
docs_src
├── drawio.md
├── gcp.drawio
├── index.md
└── theme
    └── partials
        └── footer.html
```

If you structure the documentation (like me) with folders associated with resources then this becomes `data-mxgraph-path="diagrams/gcp.drawio"`

```null
docs_src
├── diagrams
│   └── gcp.drawio
├── drawio.md
├── index.md
└── theme
    └── partials
        └── footer.html
```
