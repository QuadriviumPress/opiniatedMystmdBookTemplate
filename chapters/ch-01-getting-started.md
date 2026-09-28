---
title: Getting started
---

# Getting started

Organize each chapter as a Markdown file in `chapters/` using the
`ch-NN-slug.md` naming pattern. Add it to the `toc` in `myst.yml`, and MyST will
include it in the book navigation.

```{note}
State what the reader should be able to do after the chapter. Keep each source
file small enough to review. One file per chapter is the default.
```

## Write with MyST

MyST supports familiar Markdown plus roles and directives for technical
publishing. Give equations an `eq:` label and figures a `fig:` label.

```{math}
:label: eq:starter:energy

E = mc^2
```

You can refer back to {eq}`eq:starter:energy` without manually maintaining its number.

```{important}
A labeled equation is part of the book's shared notation. Do not repeat the
same relation later with a second label.
```

```{figure} ../images/logo.svg
:label: fig:starter:logo
:alt: Open book logo used by this starter
:align: center
:width: 20%

The starter logo. Replace it before publishing a real book.
```

```{tip}
Cross-reference the figure with {ref}`fig:starter:logo` rather than typing its number.
```

```{warning}
A figure without alternative text is a failed accessibility check. Write the
`:alt:` text for the image, and put the caption after the options.
```
