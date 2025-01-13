# Neovim Keybindings Documentation

## Leader Key
- **Leader key**: `Space`  
---

## Key Mappings

### 1. **Insert Mode**
- **`jk`**: Exit insert mode and switch to normal mode.  
---

### 2. **Normal Mode**

#### **Search Highlights**
- **`<leader>nh`**: Clear search highlights.  
  Usage: After searching (e.g., `/pattern`), use this shortcut to remove the highlighted search results.

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

### 1. **`e`: New File**
- **Description:** Create a new, empty file.
- **Command:** `<cmd>ene<CR>`
- **When to Use:** When you need to start editing a new file from scratch.
- **How to Use:** From the dashboard, press `e`.

---

### 2. **`SPC ee`: Toggle File Explorer**
- **Description:** Open or close the file explorer (`NvimTree`).
- **Command:** `<cmd>NvimTreeToggle<CR>`
- **When to Use:** When you need to browse files and directories in your project.
- **How to Use:** Press `Space` followed by `ee`.

---

### 3. **`SPC ff`: Find File**
- **Description:** Search for and open a file within the project using `Telescope`.
- **Command:** `<cmd>Telescope find_files<CR>`
- **When to Use:** When you need to quickly locate and open a file in your project.
- **How to Use:** Press `Space` followed by `ff`, then type the file name.

---

### 4. **`SPC fs`: Find Word**
- **Description:** Search for a word or phrase across the entire project using `Telescope`.
- **Command:** `<cmd>Telescope live_grep<CR>`
- **When to Use:** When you need to search for a word, function, or any piece of code across the project.
- **How to Use:** Press `Space` followed by `fs`, then type the search term.

---

### 5. **`SPC wr`: Restore Session For Current Directory**
- **Description:** Restore the session (files and window layout) from the previous session in the current directory.
- **Command:** `<cmd>SessionRestore<CR>`
- **When to Use:** When you need to pick up where you left off and restore your previous working environment.
- **How to Use:** Press `Space` followed by `wr`.

---

### 6. **`q`: Quit NVIM**
- **Description:** Quit Neovim and close the editor.
- **Command:** `<cmd>qa<CR>`
- **When to Use:** When you are finished working and want to exit Neovim.
- **How to Use:** From the dashboard, press `q`.

---

## Summary of Key Mappings

| **Key Mapping**  | **Function**                              | **When to Use**                               |
|------------------|------------------------------------------|----------------------------------------------|
| `e`              | Create a new file                        | When starting a new file                     |
| `SPC ee`         | Toggle file explorer (`NvimTree`)        | When browsing files and directories          |
| `SPC ff`         | Find and open a file                     | When searching for a specific file           |
| `SPC fs`         | Find a word or phrase                    | When searching for text across the project   |
| `SPC wr`         | Restore session for current directory    | When resuming work from the previous session |
| `q`              | Quit Neovim                              | When you're finished and want to exit Neovim  |

By using these key mappings, you can quickly access the most common functionalities in Neovim and boost your productivity!

