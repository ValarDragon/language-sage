# Sage math language support in Atom
Adds syntax highlighting and snippets to Sage math files in Atom. Currently limited to basic python syntax. Work is currently being done to add more sage mathematics functions to the language specification, to be highlighted.

[This repository](https://github.com/ValarDragon/language-sage) is a fork from [Sage-language](https://github.com/nayrangnu/language-sage), which essentially took the [Python Language Bundle](https://github.com/atom/language-python) and replaced python everywhere with sage.

To fix `in,is,not,and,or` and parameters for functions being highlighted, add the following to your personal stylesheet (which can be found at Edit -> Stylesheet):
```
atom-text-editor::shadow {
  // Add Your Styles Here
  .keyword.operator.logical.sage { color: #c678dd; }
  .variable.parameter { color: hsl( 29, 54%, 61%); }
}
```
Customize those two colors according to your preferred theme, the given two colors are the colors for the one-dark-syntax theme by atom.

Contributions are greatly appreciated. Please fork this repository and open a
pull request to add snippets, make grammar tweaks, etc.
