### Navigate this page:
1. [Introduction](#intro)
1. [Using subpages](#subpages)
1. [Page sanitization (security note)](#page-sanitization)
1. [Gollum tag reference](#tags)
1. [Gollum code block reference](#code-blocks)
1. [Gollum macro reference](#macros)
1. [Gollum diagram reference](#diagrams)
1. [Integrating mathematics](#mathematics)
1. [Authentication](#authentication)

# Introduction

By default, a page's title will be its file path, relative to repository root (or page file dir), without extension (e.g. `/mordor/Sauron`).

### Custom titles via CLI

If you start Gollum with the `--h1-title` option, then the first `<h1>` header on the page will be used. So, for example, this markdown page:

```markdown
# This is my title
# This is the first h1 that will be displayed
```

will be rendered with the `This is my title` page title. The first header rendered in the page's text will be `This is the first h1 that will be displayed`.

This option overrides the metadata syntax.

### Custom titles via the metadata syntax

The syntax:
```
<!-- --- title: My page title -->
```

Note that the metadata must be the first piece of text on the page.

# SUBPAGES

Gollum allows you to add a header, sidebar and footer to pages. They will most probably be shared among several pages. Subpages affect all pages in their directory and any subdirectories that do not have a subpage of their own.


