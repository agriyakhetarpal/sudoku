# `pygame-ce` exhibit: running in the browser

This is a minimal showcase of a Sudoku game running in the browser
via [Pyodide v0.27.0a2](https://github.com/pyodide/pyodide/releases/tag/0.27.0a2), i.e., the latest (alpha) version of Pyodide available at the time
of writing, through a recipe for [`pygame-ce`](https://github.com/pyodide/pyodide/tree/c11a1f35782cd2bd95ef2051c05c46fd2558dcaa/packages/pygame-ce),
enabling SDL2 support in a web browser.

## Sudoku

Not all features of the Sudoku specification currently work. This code hopes to
display a working example of not only how easy it is to write games with `pygame-ce`,
but also to present how one can play them with WebAssembly-generated code in the browser.
In this case, there are many missing features: no undo buttons, no highlights or hints,
I couldn't get the fonts' anti-aliasing to work properly, the number generation is
sometimes too easy – with no adjustable difficulty settings or solve (im)possibility
guarantees, and there are no interactive UI elements besides the Sudoku grid itself.

However, this is all a "yet". :) I do not intend to work on adding support for these at
this time. Please feel free to open a PR for any of these, if you'd like to, and I'll
happily accept them as they come along!
