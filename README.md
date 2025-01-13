# Neovim Keybindings Documentation

## Leader Key
- **Leader key**: `Space`  
  The leader key serves as a prefix for custom shortcuts. Replace `<leader>` in the key combinations below with `Space`.

---

## Key Mappings

### 1. **Insert Mode**
- **`jk`**: Exit insert mode and switch to normal mode.  
  Press `jk` quickly while in insert mode.

---

### 2. **Normal Mode**

#### **Search Highlights**
- **`<leader>nh`**: Clear search highlights.  
  Usage: After searching (e.g., `/pattern`), use this shortcut to remove the highlighted search results.

---

#### **Number Increment/Decrement**
- **`<leader>+`**: Increment the number under the cursor.  
- **`<leader>-`**: Decrement the number under the cursor.  
  Usage: Place the cursor over a number and use these shortcuts to adjust its value.

---

#### **Window Management**
- **`<leader>sv`**: Split the window vertically.  
- **`<leader>sh`**: Split the window horizontally.  
- **`<leader>se`**: Make all split windows equal size.  
- **`<leader>sx`**: Close the current split window.  
  Usage: Use these to manage multiple splits in your workspace.

---

#### **Tab Management**
- **`<leader>to`**: Open a new tab.  
- **`<leader>tx`**: Close the current tab.  
- **`<leader>tn`**: Go to the next tab.  
- **`<leader>tp`**: Go to the previous tab.  
- **`<leader>tf`**: Open the current buffer in a new tab.  
  Usage: Tabs act as separate workspaces. Use these shortcuts to manage them.

---

### Notes
1. **Remap Explanation**:  
   This configuration uses `vim.keymap.set()` for defining mappings.  
   Each mapping includes a `desc` (description) for clarity, making it easy to reference when exploring keybindings in Neovim tools like Telescope.

2. **How to Enable This Configuration**:  
   Save the configuration in your `init.lua` or a separate Lua file (e.g., `keymaps.lua`).  
   If stored separately, ensure to source it in your `init.lua`:
   ```lua
   require("keymaps")
