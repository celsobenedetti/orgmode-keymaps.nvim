# orgmode-keymaps.nvim

Neovim plugin for org-mode that adds useful visual-mode keymaps.

## Keymaps

| Keymap | Action |
|--------|--------|
| `<C-b>` | Toggle bold: `*bold*` |
| `<C-i>` | Toggle italic: `/italic/` |
| `<C-e>` | Toggle inline code: `=code=` (visual mode) or multiline code block (V-LINE mode) |
| `<C-k>` | Add link: `[[https://url][selected text]]` |

## Setup

Using lazy.nvim:

```lua
{ 'celsobenedetti/orgmode-keymaps.nvim', config = true }
```

### Options

```lua
require('orgmode-keymaps').setup({
  filetypes = {'org'}, -- default filetypes to enable keymaps
})
```

## Usage

1. Visually select text (v or V mode)
2. Use the keymap to transform the selection
3. For `<C-k>`, you'll be prompted to enter the URL

## References

- This was based of [markdowny.nvim](https://github.com/antonk52/markdowny.nvim) (thanks antonk52!)
