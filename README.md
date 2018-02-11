lsp-css
==============

CSS, LESS, and SASS support for lsp-mode using [vscode-css-languageserver-bin](https://github.com/vscode-langservers/vscode-css-languageserver-bin)

## Installation

### From source

Clone this repository and [lsp-mode](https://github.com/emacs-lsp/lsp-mode) to
suitable paths, and add them to your load path:

```emacs-lisp
(add-to-list 'load-path "<path to lsp-mode>")
(add-to-list 'load-path "<path to lsp-css>")
```

### From MELPA

Install one of the available packages:
- `lsp-css`

## Usage
### Enabling `lsp-css`

```emacs-lisp
(require 'lsp-css)
(add-hook 'css-mode-hook #'lsp-css-enable)
(add-hook 'less-mode-hook #'lsp-css-enable)
(add-hook 'sass-mode-hook #'lsp-css-enable)
(add-hook 'scss-mode-hook #'lsp-css-enable)
```

You also need
[vscode-css-languageserver-bin](https://github.com/vscode-langservers/vscode-css-languageserver-bin)
installed and on your PATH.

```bash
npm i -g vscode-css-languageserver-bin
```

(`sudo` may be necessary depending on how you have
[npm](https://www.npmjs.com/) setup)
