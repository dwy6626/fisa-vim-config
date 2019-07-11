fisa-vim-config
===============

A vim configuration for the modern pythonista (plus some other goodies)

Installation instructions and docs `here <http://fisadev.github.io/fisa-vim-config/>`_.

## In this fork

- Fix `range() + range()` error
- Add some customized configuration
- Activated Powerline

### To patch "Monaco" font in MacOS (for Powerline)

- Get the font from system

```bash
cp /System/Library/Fonts/Monaco.dfont Monaco.dfont
```

- Generate the .tff file (`brew install fondu` if you don't get command not found error)

```bash
fondu Monaco.dfont
```

- Do `fontforge`:

```bash
fontforge -script fontpatcher/fontpatcher Monaco.ttf
```

- Install the new font `Monaco-Powerline.tff` to system

- Apply the iTerm2 config: [zsh.json](./zsh.json), refer to [this issue](https://gitlab.com/gnachman/iterm2/issues/7533)

Please also refer to the original [readme file](./fontpatcher/README.rst)
