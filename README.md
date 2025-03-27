# M31 Neovim keymaps

This is my customized Neovim keymaps.

**Requirements:**
- [Neovim](https://neovim.io) v0.10.4 (LuaJIT 2.1.1731601260)
- [lazy.nvim](https://github.com/folke/lazy.nvim) v11.17.1
- [LazyVim](https://github.com/LazyVim/LazyVim) v14.14.0
- [snacks.nvim](https://github.com/folke/snacks.nvim) (main, [bc0630e](https://github.com/folke/snacks.nvim/commit/bc0630e))

Default keymaps set by LazyVim can be found [here](https://github.com/LazyVim/LazyVim/blob/main/lua/lazyvim/config/keymaps.lua) and customized by [@mitsuki31](https://github.com/mitsuki31).

---

## Key Mappings

### Buffers
| Keybinding | Mode | Description |
| ---------- | ---- | ----------- |
| <kbd>Alt-N</kbd> | Normal | Create a new buffer. |
| <kbd>Alt-D</kbd> | Normal | Delete the current buffer using `Snacks.bufdelete()`. |
| <kbd>Ctrl-S</kbd> | Insert | Save current buffer without changing to Normal mode. |

### Lines Formatting
| Keybinding | Mode | Description |
| ---------- | ---- | ----------- |
| <kbd>Ctrl-\\</kbd> | Insert, Normal, Visual | Toggle comment for the current line or selection. |
| <kbd>Ctrl-Z</kbd> | Insert, Normal | Undo the last change. |
| <kbd>Ctrl-Y</kbd> | Insert, Normal | Redo the last undone change. |

#### Moving Lines
| Keybinding | Mode | Description |
| ---------- | ---- | ----------- |
| <kbd>Alt-Down</kbd> | Normal | Move the current line below the cursor. |
| <kbd>Alt-Up</kbd> | Normal | Move the current line above the cursor. |
| <kbd>Alt-Down</kbd> | Insert | Move the current line down while staying in Insert mode. |
| <kbd>Alt-Up</kbd> | Insert | Move the current line up while staying in Insert mode. |
| <kbd>Alt-Down</kbd> | Visual | Move selected lines down. |
| <kbd>Alt-Up</kbd> | Visual | Move selected lines up. |

#### Deleting Lines
| Keybinding | Mode | Description |
| ---------- | ---- | ----------- |
| <kbd>Shift-D</kbd> | Visual | Delete selection without copying to clipboard (Void Delete). |

### Selection
| Keybinding | Mode | Description |
| ---------- | ---- | ----------- |
| <kbd>Ctrl-A</kbd> | Insert | Select all text in the buffer. |
| <kbd>Alt-A</kbd> | Normal | Select all text in the buffer (alternative to <kbd>Ctrl-A</kbd> to avoid overriding number increment functionality). |

---

## Notes
- <kbd>Ctrl-A</kbd> **Remapping Warning:**
  - <kbd>Ctrl-A</kbd> is normally used to increment numbers under the cursor. The alternative `<kbd>Alt-A</kbd> is provided for selecting all text in Normal mode.
- **Commenting Keymap ( <kbd>Ctrl-\\</kbd> )**:
  - This keybinding replaces the default comment toggling shortcut (`gcc`) with a more accessible key combination.

