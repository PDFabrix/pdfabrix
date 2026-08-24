# Community Templates

This directory contains PDFabrix templates contributed by the community.


## How to contribute

Create your template with the **PDFabrix desktop app**, then export it as a **Folder**.

In **Workspace → Templates**:

1. Design or open your template.
2. Click **Export → Folder**.
3. Choose a unique **Folder ID** and fill in the template metadata.
4. Export the folder.

Each template must have this structure:

```text
templates/
└── your-template-id/
    ├── meta.json
    ├── cover.png
    └── template.pdfabrix
```

### Folder ID

Use a short, unique ID:

* lowercase letters, numbers, `-`, and `_` only
* must start with a letter or number
* maximum 60 characters

Examples:

```text
invoice-simple-a4
shipping-label
certificate-a4
```

### Required files

| File               | Description                                           |
| ------------------ | ----------------------------------------------------- |
| `meta.json`        | Template name, description, author, and contact email |
| `cover.png`        | Template preview image                                |
| `template.pdfabrix` | Exported PDFabrix template                           |

> **Important:** Use **Export → Folder**, not **Export → Template**. The single `.pdfabrix` file is not the format used in this directory.

## Submit a Pull Request

1. Fork this repository.
2. Add your exported template folder under `templates/`.
3. Commit and push your changes.
4. Open a pull request against `main`.

Before submitting, make sure the template imports and previews correctly in PDFabrix and that you have permission to share any included fonts, images, or other assets.

All submissions are reviewed before being added to the community gallery.

Maintainers: after merging template changes, run `npm run gallery` at the repository root to refresh the gallery in [README.md](../README.md).

For questions, open a [GitHub issue](https://github.com/PDFabrix/pdfabrix/issues) or email [support@pdfabrix.com](mailto:support@pdfabrix.com).
