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

### 5. **`SPC wr`: Restore Session for Current Working Directory**
- **Description:** Restore the last session for the current working directory, including open files and window layout.
- **Command:** `<cmd>SessionRestore<CR>`
- **When to Use:** When you want to resume your work in the same directory with the exact same workspace state as when you last worked in it.
- **How to Use:** Press `Space` followed by `wr` to restore the session for the current directory.

---

### 6. **`SPC ws`: Save Session for Current Working Directory**
- **Description:** Save the current session for the current working directory, including open files and window layout.
- **Command:** `<cmd>SessionSave<CR>`
- **When to Use:** When you want to save the current workspace state to come back to it later.
- **How to Use:** Press `Space` followed by `ws` to save the session for the current directory.

---
### 7. **`<leader>mp`: Format File or Range (in Visual Mode)**
# Gitsigns Plugin Key Mappings

## **Navigation**
- **`]h`**: Move to the next hunk (code change) in the current file.
- **`[h`**: Move to the previous hunk (code change) in the current file.

## **Actions**
- **`<leader>hs`**: Stage the current hunk (mark the change for commit).
- **`<leader>hr`**: Reset the current hunk (undo the changes in the hunk).
- **`<leader>hs`** (in Visual Mode): Stage the selected hunk (select a range of text in Visual Mode and stage it).
- **`<leader>hr`** (in Visual Mode): Reset the selected hunk (select a range of text in Visual Mode and undo the changes).
- **`<leader>hS`**: Stage the entire buffer (all changes in the file).
- **`<leader>hR`**: Reset the entire buffer (undo all changes in the file).
- **`<leader>hu`**: Undo stage the current hunk (unstage it).
- **`<leader>hp`**: Preview the current hunk (view the changes in the hunk).
- **`<leader>hb`**: Blame the current line (shows who made the last change and the commit message).
- **`<leader>hB`**: Toggle line blame (turns the line blame information on or off).
- **`<leader>hd`**: Diff the current file (shows the diff for the current file).
- **`<leader>hD`**: Diff the current file against its previous version (`~`).

## **Text Object**
- **`ih`** (in Operator or Visual Mode): Select the current hunk.
  - After selecting a hunk with `ih`, you can stage it by pressing `<leader>hs` or reset it by pressing `<leader>hr`.
# Lazygit Plugin Key Mapping Documentation

## Key Mapping

- **`<leader>lg`**: Open the Lazygit interface in a floating window.

## How to Use

1. **Open Lazygit**:
   - Press the key combination `<leader>lg` (where `<leader>` is typically the space key by default).
   - This will trigger the `LazyGit` command and open the Lazygit interface in a floating window.

2. **Navigate and Use Lazygit**:
   - Once the Lazygit window is open, you can use its interactive interface to perform git operations like staging, committing, viewing logs, checking branches, and more.
   - The floating window will provide a full git interface, allowing you to interact with your repository without leaving Neovim.

### Example:
- Pressing `<leader>lg` opens the Lazygit interface for the current git repository.
- You can use the Lazygit interface just like you would use a terminal git client, but all within Neovim.

# Manual Linting Key Mapping Documentation

## Key Mapping

- **`<leader>l`**: Trigger linting for the current file.

## How to Use

1. **Trigger Linting**:
   - Press the key combination `<leader>l` (where `<leader>` is typically the space key by default).
   - This will manually trigger linting for the current file. The linting tool (e.g., `lint` or a configured linter) will scan the file for issues and display the results.

2. **Linting Process**:
   - After pressing `<leader>l`, the linting results will be shown, indicating any syntax errors or code quality issues in the current file.
   - You can navigate through the issues to fix them, depending on the linting tool you have configured.

**Triggering Key Mappings**:
   - **`gR`**: Show references of the symbol under the cursor.
   - **`gD`**: Go to the declaration of the symbol.
   - **`gd`**: Open the symbol's definition using `Telescope`.
   - **`<leader>ca`**: Open code action options (like fix suggestions, refactoring, etc.).
   - **`<leader>rn`**: Trigger renaming of the symbol under the cursor.
   - **`<leader>rs`**: Restart the LSP server for the current project.

### Cách sử dụng các Key Mappings:

- **`<C-k>` - Chọn mục hoàn tất trước**:
  
  - **Khi nào sử dụng**: Khi bạn đang sử dụng menu hoàn tất và muốn di chuyển lên để chọn gợi ý hoàn tất trước đó.
  - **Cách sử dụng**: Sau khi menu hoàn tất hiện ra, nhấn `<C-k>` để chọn mục hoàn tất phía trên trong danh sách gợi ý. Ví dụ: Bạn muốn chọn một biến đã khai báo trước đó và menu hiện ra các lựa chọn, nhấn `<C-k>` để di chuyển lên.

- **`<C-j>` - Chọn mục hoàn tất tiếp theo**:
  
  - **Khi nào sử dụng**: Khi bạn muốn di chuyển xuống và chọn mục hoàn tất tiếp theo trong danh sách gợi ý.
  - **Cách sử dụng**: Khi menu hoàn tất hiển thị, nhấn `<C-j>` để di chuyển xuống mục tiếp theo trong danh sách. Ví dụ: Bạn đang gõ mã và muốn chọn một hàm từ gợi ý, nhấn `<C-j>` để chọn hàm tiếp theo.

- **`<C-b>` - Cuộn tài liệu lên**:
  
  - **Khi nào sử dụng**: Khi mô tả của gợi ý hoàn tất quá dài và bạn muốn cuộn lên để xem phần trên.
  - **Cách sử dụng**: Trong menu hoàn tất hoặc khi đang xem mô tả gợi ý, nhấn `<C-b>` để cuộn tài liệu lên. Ví dụ: Khi đang chọn một gợi ý từ LSP và phần mô tả bị cắt bớt, nhấn `<C-b>` để cuộn lên xem chi tiết hơn.

- **`<C-f>` - Cuộn tài liệu xuống**:
  
  - **Khi nào sử dụng**: Khi mô tả của gợi ý quá dài và bạn muốn cuộn xuống để xem phần tiếp theo.
  - **Cách sử dụng**: Trong menu hoàn tất, nhấn `<C-f>` để cuộn tài liệu xuống. Ví dụ: Khi mô tả của một gợi ý chiếm nhiều không gian, nhấn `<C-f>` để cuộn xuống và đọc phần tiếp theo.

- **`<C-Space>` - Hiển thị menu hoàn tất**:
  
  - **Khi nào sử dụng**: Khi bạn muốn hiển thị menu hoàn tất và xem các gợi ý như hàm, biến, hoặc đường dẫn tệp.
  - **Cách sử dụng**: Khi bạn đang gõ mã và muốn thấy các gợi ý từ LSP, snippets, hoặc buffer, nhấn `<C-Space>` để hiển thị menu hoàn tất. Ví dụ: Bạn đang nhập tên hàm và muốn chọn từ danh sách gợi ý, nhấn `<C-Space>` để mở menu hoàn tất.

- **`<C-e>` - Đóng cửa sổ hoàn tất**:
  
  - **Khi nào sử dụng**: Khi bạn không muốn chọn bất kỳ gợi ý nào và muốn đóng cửa sổ hoàn tất.
  - **Cách sử dụng**: Khi menu hoàn tất hiển thị và bạn không muốn chọn gợi ý nào, nhấn `<C-e>` để đóng cửa sổ hoàn tất. Ví dụ: Menu hoàn tất hiện ra nhưng bạn quyết định không chọn gợi ý nào, chỉ cần nhấn `<C-e>` để đóng cửa sổ.

- **`<CR>` - Xác nhận lựa chọn gợi ý**:
  
  - **Khi nào sử dụng**: Khi bạn đã chọn một gợi ý trong menu hoàn tất và muốn xác nhận lựa chọn đó.
  - **Cách sử dụng**: Sau khi di chuyển đến một gợi ý trong menu hoàn tất, nhấn `Enter` (hoặc `<CR>`) để chọn gợi ý đó. Ví dụ: Khi bạn chọn một tên hàm từ danh sách gợi ý, nhấn `Enter` để hoàn tất và tiếp tục viết mã.
### Cách sử dụng các Key Mappings:

- **`<leader>ee` - Toggle file explorer**:
  
  - **Khi nào sử dụng**: Khi bạn muốn mở hoặc đóng file explorer trong Neovim.
  - **Cách sử dụng**: Nhấn `<leader>ee` để chuyển đổi giữa việc mở hoặc đóng file explorer. Ví dụ: Bạn đang làm việc trong một tệp và muốn mở file explorer để dễ dàng truy cập các tệp khác trong dự án.

- **`<leader>ef` - Toggle file explorer on current file**:
  
  - **Khi nào sử dụng**: Khi bạn muốn mở hoặc đóng file explorer và tự động điều hướng đến tệp hiện tại trong explorer.
  - **Cách sử dụng**: Nhấn `<leader>ef` để mở file explorer và tự động làm nổi bật tệp bạn đang làm việc trong đó. Ví dụ: Bạn muốn dễ dàng tìm và mở tệp hiện tại trong dự án từ file explorer.

- **`<leader>ec` - Collapse file explorer**:
  
  - **Khi nào sử dụng**: Khi bạn muốn thu gọn file explorer để làm sạch không gian làm việc.
  - **Cách sử dụng**: Nhấn `<leader>ec` để thu gọn file explorer. Ví dụ: Bạn muốn tạm thời đóng file explorer để tập trung vào mã của mình mà không làm phiền không gian màn hình.

- **`<leader>er` - Refresh file explorer**:
  
  - **Khi nào sử dụng**: Khi bạn muốn làm mới file explorer để cập nhật danh sách tệp trong trường hợp có thay đổi ngoài Neovim.
  - **Cách sử dụng**: Nhấn `<leader>er` để làm mới file explorer và cập nhật các thay đổi tệp mới nhất. Ví dụ: Bạn vừa thêm, xóa hoặc thay đổi một tệp trong dự án bên ngoài Neovim và muốn làm mới explorer để phản ánh sự thay đổi.
### Cách sử dụng các Key Mappings:

- **`s` - Substitute with motion**:

  - **Khi nào sử dụng**: Khi bạn muốn thay thế văn bản từ vị trí con trỏ đến một vị trí xác định theo chuyển động con trỏ.
  - **Cách sử dụng**: Di chuyển con trỏ đến vị trí bắt đầu, sau đó nhấn `s` và tiếp tục với một chuyển động (ví dụ: `w`, `e`, `t`, ...) để thay thế phần văn bản được chỉ định. Ví dụ: `s` + `w` sẽ thay thế từ vị trí con trỏ đến đầu từ tiếp theo.

- **`ss` - Substitute line**:

  - **Khi nào sử dụng**: Khi bạn muốn thay thế toàn bộ nội dung của một dòng.
  - **Cách sử dụng**: Đặt con trỏ vào bất kỳ vị trí nào trên dòng bạn muốn thay thế, nhấn `ss`, và bạn sẽ được yêu cầu nhập văn bản thay thế cho toàn bộ dòng. Ví dụ: Bạn muốn thay thế nội dung của một dòng mà không cần di chuyển con trỏ ra khỏi nó.

- **`S` - Substitute to end of line**:

  - **Khi nào sử dụng**: Khi bạn muốn thay thế văn bản từ vị trí con trỏ cho đến hết dòng.
  - **Cách sử dụng**: Đặt con trỏ vào vị trí bạn muốn bắt đầu thay thế, sau đó nhấn `S`. Văn bản từ vị trí con trỏ đến cuối dòng sẽ được thay thế.

- **`s` (Visual Mode) - Substitute in visual mode**:

  - **Khi nào sử dụng**: Khi bạn muốn thay thế văn bản đã được chọn trong chế độ visual.
  - **Cách sử dụng**: Vào chế độ visual (nhấn `v` để chọn văn bản), sau đó nhấn `s` để thay thế phần văn bản đã chọn. Ví dụ: Bạn có thể chọn một phần của văn bản và thay thế nó bằng văn bản mới mà không làm thay đổi các phần khác.
### Cách sử dụng các Key Mappings:

- **`<leader>ff` - Fuzzy find files in cwd**:

  - **Khi nào sử dụng**: Khi bạn muốn tìm kiếm và mở một tệp trong thư mục làm việc hiện tại bằng cách sử dụng tìm kiếm mờ (fuzzy search).
  - **Cách sử dụng**: Nhấn `<leader>ff`, và một cửa sổ tìm kiếm sẽ xuất hiện cho phép bạn nhập tên tệp để tìm kiếm trong thư mục hiện tại. Gõ tên tệp và chọn tệp bạn muốn mở.

- **`<leader>fr` - Fuzzy find recent files**:

  - **Khi nào sử dụng**: Khi bạn muốn tìm kiếm và mở một tệp gần đây mà bạn đã làm việc.
  - **Cách sử dụng**: Nhấn `<leader>fr`, và một danh sách các tệp gần đây sẽ xuất hiện. Bạn có thể chọn tệp bạn muốn mở từ danh sách này.

- **`<leader>fs` - Find string in cwd**:

  - **Khi nào sử dụng**: Khi bạn muốn tìm kiếm một chuỗi trong tất cả các tệp trong thư mục làm việc hiện tại.
  - **Cách sử dụng**: Nhấn `<leader>fs` và nhập chuỗi mà bạn muốn tìm. Tìm kiếm sẽ được thực hiện trên toàn bộ thư mục, và bạn sẽ nhận được một danh sách các kết quả tìm kiếm.

- **`<leader>fc` - Find string under cursor in cwd**:

  - **Khi nào sử dụng**: Khi bạn muốn tìm kiếm chuỗi văn bản mà con trỏ hiện tại đang chỉ vào trong thư mục làm việc hiện tại.
  - **Cách sử dụng**: Đặt con trỏ vào chuỗi bạn muốn tìm và nhấn `<leader>fc`. Tìm kiếm sẽ được thực hiện cho chuỗi văn bản đó trong toàn bộ thư mục làm việc.

- **`<leader>ft` - Find todos**:

  - **Khi nào sử dụng**: Khi bạn muốn tìm tất cả các TODOs trong mã nguồn của bạn.
  - **Cách sử dụng**: Nhấn `<leader>ft` để mở cửa sổ tìm kiếm và tìm tất cả các mục TODO trong dự án của bạn. Bạn có thể dễ dàng xem các mục TODO đã được ghi chú.

### Cách sử dụng các Key Mappings:

- **`<leader>xw` - Open trouble workspace diagnostics**:

  - **Khi nào sử dụng**: Khi bạn muốn mở bảng chẩn đoán của toàn bộ workspace, để kiểm tra các lỗi hoặc vấn đề trong mã nguồn của toàn bộ dự án.
  - **Cách sử dụng**: Nhấn `<leader>xw`, và cửa sổ Trouble sẽ mở ra, hiển thị tất cả các cảnh báo, lỗi và vấn đề trong workspace của bạn.

- **`<leader>xd` - Open trouble document diagnostics**:

  - **Khi nào sử dụng**: Khi bạn muốn xem chẩn đoán lỗi hoặc vấn đề trong tài liệu (file) hiện tại.
  - **Cách sử dụng**: Nhấn `<leader>xd`, và cửa sổ Trouble sẽ chỉ hiển thị các lỗi hoặc vấn đề trong tệp mà bạn đang làm việc.

- **`<leader>xq` - Open trouble quickfix list**:

  - **Khi nào sử dụng**: Khi bạn muốn xem danh sách các quickfixes (ví dụ: sửa lỗi hoặc sửa mã nhanh chóng) trong dự án.
  - **Cách sử dụng**: Nhấn `<leader>xq`, và Trouble sẽ mở ra danh sách các quickfixes có thể áp dụng vào mã nguồn của bạn.

- **`<leader>xl` - Open trouble location list**:

  - **Khi nào sử dụng**: Khi bạn muốn xem danh sách các vị trí có lỗi hoặc cảnh báo trong mã nguồn của bạn.
  - **Cách sử dụng**: Nhấn `<leader>xl`, và Trouble sẽ hiển thị một danh sách các vị trí trong mã mà có vấn đề cần chú ý.

- **`<leader>xt` - Open todos in trouble**:

  - **Khi nào sử dụng**: Khi bạn muốn tìm và xem các mục TODO trong mã của bạn.
  - **Cách sử dụng**: Nhấn `<leader>xt`, và Trouble sẽ hiển thị tất cả các mục TODO mà bạn đã ghi chú trong mã nguồn của mình, giúp bạn theo dõi công việc cần làm.
### Cách sử dụng các Key Mappings:

- **`<leader>sm` - Maximize/Minimize a Split**:

  - **Khi nào sử dụng**: Khi bạn muốn tối đa hóa hoặc thu nhỏ một cửa sổ chia (split) trong Neovim.
  - **Cách sử dụng**: Nhấn `<leader>sm` để chuyển đổi trạng thái của cửa sổ chia hiện tại. Nếu cửa sổ đó đang được chia nhỏ, nó sẽ được tối đa hóa. Nếu cửa sổ đã tối đa hóa, nó sẽ trở lại trạng thái chia nhỏ.

