# Markdown Auto-Rendering of Symlinked README.md Test

This repo test a strange behavior, where it appears that a certain character change causes a rendering issue.

The issues is only apparent when GitHub automatically renders a `README.md` __symlink__ which points to a real markdown file.

The markdown file itself renders fine, it is only the rendering of the symlink which happens because the symlink is named `README.md`.

The dirs `foo`, and `bar`, contain an example each. In `foo` and `bar` the target markdown files (`foo.md` and `bar.md`) each contain a heading line and a single character `a`, or `A` respectively. The `README.md` symlink in `foo` pointing to `foo.md` renders automatically when viewing the dir in GitHub, the one in `bar` pointing to `bar.md` does not.

Why? It seems like something to do with character encoding...

