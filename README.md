# Qt support for vim

Simple Qt support for Qt-based projects.

## Installation:

# vim-plug
  Plug 'cpiger/vim-qt'

## Filetypes:

* C++
* qmake
* qml
* qbs
* qrc -- xml
* ui -- xml
* ts -- xml

## Status:

| Language | File Type Detection | File Type Plugin |       Syntax       |     Indent    | Compiler | Plugin |
| :------- | :-----------------: | :--------------: | :----------------: | :-----------: | :------: | :----: |
|  Qt C++  |  **+** (extend cpp) |                  | **+** (extend cpp) |               |          |        |
|  qmake   |        **+**        |      **+**       |        **+**       |               |          |        |
|   qml    |        **+**        |                  |        **+**       |     **+**     |          |        |
|   qbs    |        **+**        |      **+**       |        **+**       |               |          |        |
|   qrc    |     **+** (xml)     |                  |                    |               |          |        |
|    ui    |     **+** (xml)     |                  |                    |               |          |        |
|    ts    |     **+** (xml)     |                  |                    |               |          |        |


## vim-qt-assistant

Search and display the document of the word under the current cursor in qt assistant.

# Usage
just call `GetDocFromAssistant()` function in vim.

```
:call GetDocFromAssistant()

# or map a key to do this:

map <F1> :call GetDocFromAssistant()<CR>
```

## Related works:

* https://github.com/vim-scripts/cpp.vim
* https://github.com/Townk/vim-qt
* https://github.com/kosl90/qt-highlight-vim
* https://github.com/vim-scripts/Qt.vim
* https://github.com/edlanglois/vim-qrc
* https://github.com/vim-scripts/qt2vimsyntax
* https://github.com/pavel-belikov/vim-qtcreator-tasks
* https://github.com/vim-scripts/qmake--syntax.vim
* https://github.com/pavel-belikov/vim-qmake
* https://github.com/artoj/qmake-syntax-vim
* https://github.com/suy/vim-qmake
* https://bitbucket.org/JohnKaul/qbs.vim
* https://github.com/tiamat18/vim-qmake
* https://github.com/listenerri/vim-qt-assistant

## TODO:

* Add supported syntaxes to Syntax menu
* QtDoc

## C++ Completion for Qt

1. Generate compile_commands.json (for example: https://github.com/rizsotto/Bear)
2. Set up LSP server (for example: https://github.com/cquery-project/cquery)
3. Install & use LSP client for Vim
   (https://github.com/autozimu/LanguageClient-neovim or
   https://github.com/prabirshrestha/vim-lsp)
   
