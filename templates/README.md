# Community Templates

This directory contains PDFDog templates contributed by the community.


## How to contribute

Create your template with the **PDFDog desktop app**, then export it as a **Folder**.

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
    └── template.pdfdog
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

| File              | Description                                           |
| ----------------- | ----------------------------------------------------- |
| `meta.json`       | Template name, description, author, and contact email |
| `cover.png`       | Template preview image                                |
| `template.pdfdog` | Exported PDFDog template                              |

> **Important:** Use **Export → Folder**, not **Export → Template**. The single `.pdfdog` file is not the format used in this directory.

## Submit a Pull Request

1. Fork this repository.
2. Add your exported template folder under `templates/`.
3. Commit and push your changes.
4. Open a pull request against `main`.

Before submitting, make sure the template imports and previews correctly in PDFDog and that you have permission to share any included fonts, images, or other assets.

All submissions are reviewed before being added to the app gallery.

For questions, open a [GitHub issue](https://github.com/PDF-Dog/pdfdog/issues) or email [support@getpdfdog.com](mailto:support@getpdfdog.com).
