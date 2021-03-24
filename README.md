![](https://img.shields.io/badge/Stability-Experimental-red.svg)
[![Build Status](http://104.196.136.37/api/badges/ronggur/tinkerbell-docs/status.svg)](http://104.196.136.37/ronggur/tinkerbell-docs)

# Tinkerbell Docs

This is the source repo for the Tinkerbell docs. They are build using static-site generator [`mkdocs`](https://www.mkdocs.org/) and using the [`mkdocs-material`](https://squidfunk.github.io/mkdocs-material/) theme, then served by netlify to [docs.tinkerbell.org](https://docs.tinkerbell.org/). 

## mkdocs

If you wish, you can install `mkdocs` and `mkdocs-material` to build the docs locally. Prerequisite: You need to have Python installed.

To [install `mkdocs`](https://www.mkdocs.org/#installation):

`pip install mkdocs`

Next you'll need to [install the `mkdocs-material` theme](https://squidfunk.github.io/mkdocs-material/getting-started/#installation):

`pip install mkdocs-material`

To build locally, clone the repo and from `tinkerbell-docs`, run:

`mkdocs serve`

## Contributing to the Tinkerbell Docs

All the markdown source files for the documentation are in the `docs/` folder. Find the file that you want to update and edit it. Then open a Pull Request with your changes. Make sure that the build passes, and take a look at the netlify preview to see your changes staged on the website.

### Page metadata

Currently the metadata for the page is yaml formatted, with two fields: title and date. If you edit a doc, update the date to when you made your edits. 

### Adding Images

All the images for the docs are in the `images/` folder. To pull the image into your doc, use a relative link to the image file. Example:

```
![Architecture](/images/architecture-diagram.png)
```

### Adding a page

If you would like to submit a new page to the documentation, be sure to add it to the `nav` section in mkdocs.yml. This will ensure that the page appears in the table of contents.
