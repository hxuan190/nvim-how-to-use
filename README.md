# Neovim Keybindings Documentation

## Leader Key
- **Leader key**: Space (`SPC`)

---

## Key Mappings

### Insert Mode
- `jk`: Exit insert mode and switch to normal mode.

---

### Normal Mode

#### Search Highlights
- `nh`: Clear search highlights (after searching with `/pattern`).

#### Window Management
- `sv`: Split window vertically.
- `sh`: Split window horizontally.
- `se`: Equalize split window sizes.
- `sx`: Close the current split window.

#### Tab Management
- `to`: Open a new tab.
- `tx`: Close the current tab.
- `tn`: Next tab.
- `tp`: Previous tab.
- `tf`: Open the current buffer in a new tab.

---

### File and Explorer Commands
- `e`: Create a new file (`:ene`).
- `SPC ee`: Toggle file explorer (`:NvimTreeToggle`).

---

### Search Commands (Telescope)
- `SPC ff`: Find file (`:Telescope find_files`).
- `SPC fs`: Search word (`:Telescope live_grep`).

---

### Session Management
- `SPC wr`: Restore session for current directory (`:SessionRestore`).
- `SPC ws`: Save session for current directory (`:SessionSave`).

---

### Quit & Format
- `q`: Quit Neovim (`:qa`).
- `mp`: Format file or selected range.

---

## Gitsigns Plugin

### Navigation
- `]h`: Next hunk.
- `[h`: Previous hunk.

### Actions
- `hs`: Stage current hunk.
- `hr`: Reset current hunk.
- `hu`: Undo stage hunk.
- `hp`: Preview hunk.
- `hb`: Blame current line.
- `hB`: Toggle line blame.
- `hd`: Diff current file.
- `hS`: Stage entire buffer.
- `hR`: Reset entire buffer.

### Text Objects
- `ih`: Select current hunk in operator/visual mode.

---

## Lazygit Plugin
- `lg`: Open Lazygit in a floating window.

---

## Manual Linting
- `l`: Trigger linting for the current file.

---

## Additional LSP Key Mappings
- `gR`: Show references.
- `gD`: Go to declaration.
- `gd`: Go to definition.
- `ca`: Show code actions.
- `rn`: Rename symbol.
- `rs`: Restart LSP server.

---

## Completion Navigation
- `<C-k>`: Select previous completion item.
- `<C-j>`: Select next completion item.
- `<C-u>`: Scroll documentation up.
- `<C-d>`: Scroll documentation down.
