貪吃蛇遊戲（Snake Game）

一個使用 HTML5 Canvas + 原生 JavaScript 實作的經典貪吃蛇遊戲，包含深色現代風 UI、難度選擇、蛇樣式切換、本地最高分紀錄與暫停功能。



功能介紹





單一檔案執行：所有 HTML / CSS / JS 都在 index.html 中，開啟即可玩。



鍵盤操作：方向鍵 ↑ ↓ ← → 控制蛇的移動。



暫停 / 繼續：按下按鈕或鍵盤空白鍵 / P 來暫停與繼續。



難度選擇：





初級：速度較慢、無障礙物。



中級：速度中等，吃水果後逐漸生成隨機石頭，最多 25 顆。



高級：速度較快，石頭生成更快且最多 40 顆。



蛇樣式切換：提供 15 種配色，可即時切換。



水果種類：多種不同色系的小水果方塊。



分數與最高分：當前分數與最高分會顯示在頂部，最高分保存在瀏覽器 localStorage。



本機執行方式





確認專案結構類似：

 貪吃蛇遊戲/
 ├─ index.html
 └─ README.md



直接用瀏覽器開啟：





在 Finder 中雙擊 index.html，或



右鍵 index.html → 用瀏覽器開啟（例如 Chrome / Safari / Edge）。



建議使用桌機 / 筆電瀏覽器執行，以方便使用鍵盤方向鍵操作。



專案初始化（本機 Git 設定）

如果目前資料夾還不是 Git 專案，可以依照以下步驟在終端機中執行（目錄需在 貪吃蛇遊戲）：

cd "貪吃蛇遊戲"

# 初始化 git
git init

# 將檔案加入版本控制
git add index.html README.md

# 建立第一次提交
git commit -m "Initial commit: Snake game"



發佈到 GitHub 的步驟

1. 在 GitHub 建立新的 Repository





登入 GitHub。



右上角點選 「+」 → New repository。



輸入：





Repository name：例如 snake-game（或你喜歡的名稱）



其他選項保持預設（先不用勾選初始化 README 等）。



按 Create repository 建立。

建立後，GitHub 會顯示一段「把現有專案推上來」的指令說明，類似：

git remote add origin https://github.com/<你的帳號>/<repo-name>.git
git branch -M main
git push -u origin main

2. 在本機專案中連結到 GitHub

在終端機中、並確保目前目錄是 貪吃蛇遊戲 專案根目錄：

cd "貪吃蛇遊戲"

# 新增遠端 repository（請把網址換成你自己 repo 的 URL）
git remote add origin https://github.com/<你的帳號>/<repo-name>.git

# 確保使用 main 分支（若已是 main 可略過）
git branch -M main

# 將本機 commit 推送到 GitHub
git push -u origin main

完成後，到 GitHub 上的 repo 頁面，就可以看到 index.html 和 README.md。



使用 GitHub Pages 發佈為靜態網站

由於這個遊戲是純前端靜態頁面，非常適合用 GitHub Pages 直接發佈。

步驟





打開你的 GitHub 專案頁面，例如：





https://github.com/<你的帳號>/<repo-name>



點選上方的 Settings。



左側選單找到 Pages（有時在「Code and automation」區塊底下）。



在 Build and deployment 區塊中：





Source 選擇 Deploy from a branch。



Branch 選擇 main，並保持資料夾為 / (root)。



按 Save。



等待數十秒到一兩分鐘，GitHub Pages 會在同一頁顯示：





Your site is live at https://<你的帳號>.github.io/<repo-name>/

之後你就可以用這個網址分享你的貪吃蛇遊戲給其他人玩。



開發與修改建議





如需修改遊戲行為（速度、障礙物生成規則、蛇樣式等），可以直接編輯 index.html 裡的 <script> 區塊。



修改後建議流程：





在瀏覽器重新整理測試。



在終端機執行：

 git status        # 查看變更
 git add index.html
 git commit -m "調整 xxx 功能"
 git push          # 推到 GitHub



一般情況下，GitHub Pages 會在 push 之後自動重新部署，稍等片刻即可在網頁上看到最新版本。



授權（可自行修改）

預設未指定授權，你可以依照需求：





將此專案設為 Private 僅自用；或



新增一個 LICENSE 檔案（例如 MIT License），開放他人學習與使用。

