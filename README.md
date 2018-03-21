# Symlinked Markdown Auto-Rendering of README.md Test

This repo test a strange behavior, where it appears that a certain number of `%` symbols in a markdown link's target URL causes a rendering issue.

The issues is only apparent when GitHub automatically renders a `README.md` __symlink__ which points to a real markdown file.

The markdown file itself renders fine, it is only the rendering of the symlink which happens because the symlink is named `README.md`.

The dirs `foo1`, `bar1`, contain an example each. In `foo1` and `bar1` the target markdown files (`foo.md` and `bar.md`) each contain exatcly one `%` char in a single link target. The only difference is text padding. The `README.md` symlink in `foo1` renders automatically when viewing the dir in GitHub, the one in `bar1` does not.

This is repeated using a markdown link with 2 `%` chars, in `foo2` and `bar2` respectively. However, this time `foo.md` needs more padding to make it render, because it has more `%` chars in its link, than the previous example, weird.
