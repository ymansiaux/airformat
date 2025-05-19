# airformat
Demo of the Air code formatter:

- using a pre commit hook
- using Github Actions (format + devtools::check() of an R package)

# Requirements

- Air installed
- Depending on your IDE, you may also need to install some extensions (as as VSCode user I had to install the [Air - R Language Support extension](https://marketplace.visualstudio.com/items?itemName=Posit.air-vscode).

Please read the following ressources before starting:

- https://posit-dev.github.io/air/formatter.html
- https://www.tidyverse.org/blog/2025/02/air/

**Warning for VSCode users**

Before using Air I was using the REditorSupport formatter provided with the [R extension for VSCode](https://github.com/REditorSupport/vscode-R). Air was not working, because I forgot to edit correctly my `settings.json` file.

If you wish Air to be used as your default formatter, please comment or remove the line `"editor.defaultFormatter": "REditorSupport.r"` in your `settings.json` file.

```
  "[r]": {
    // "editor.defaultFormatter": "REditorSupport.r",
    "editor.formatOnSave": true,
    "editor.wordSeparators": "`~!@#%$^&*()-=+[{]}\\|;:'\",<>/?"
  }
```

