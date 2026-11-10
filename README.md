# 課程讀書筆記站｜C++ 講義

課程講義與讀書筆記的靜態網站，目前主題為 C++（第 1–7 講）。純 HTML + CSS，無需建置工具，可直接部署於 GitHub Pages。

- 維運規範：[`AGENTS.md`](AGENTS.md)
- 新增講義：複製 `notes/_lecture-template.html`，命名為 `cpp-NN-主題.html`，並在 `index.html` 依講次加入卡片。
- 新增閱讀筆記：複製 `notes/_template.html`。

## 本機預覽

直接用瀏覽器開啟 `index.html` 即可。

## 部署到 GitHub Pages

1. 在 GitHub 建立新的 repository（例如 `cpp-lecture-notes`）。
2. 在本資料夾執行：
   ```bash
   git init
   git add .
   git commit -m "Add C++ lecture notes"
   git branch -M main
   git remote add origin https://github.com/<你的帳號>/cpp-lecture-notes.git
   git push -u origin main
   ```
3. 到 repository 的 **Settings → Pages**，Source 選 **Deploy from a branch**，Branch 選 **main**，資料夾選 **/ (root)**，儲存。
4. 約一兩分鐘後，網址為 `https://<你的帳號>.github.io/cpp-lecture-notes/`。

## 更新紀錄

- 2026-11-10：主題改為 C++，新增第 1–7 講講義與講義範本；AGENTS.md 新增講義結構規則。
- 2026-11-10：建立網站骨架、`AGENTS.md`、閱讀筆記範本。

## 待辦

- 講義中的程式碼尚未實際編譯驗證，建議在本機以 `g++ -std=c++20 -Wall -Wextra` 逐講測試。
- 講義內容依 cppreference 與標準行為撰寫，正式用於教學前請對照最新標準再確認。
