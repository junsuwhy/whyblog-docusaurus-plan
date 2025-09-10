# 3-2. 初始化 Docusaurus 專案

## 描述

在應用程式倉庫中初始化 Docusaurus 專案，建立完整的 Docusaurus 應用程式結構和配置。
此步驟將：

1. 執行 Docusaurus 專案初始化，建立基本的專案結構
2. 安裝中文搜尋功能套件，支援繁體中文內容搜尋
3. 配置基本的專案設定，為後續的客製化配置做準備
4. 確保專案能正常執行本地開發伺服器

這是雙倉庫架構中應用程式端的核心建置步驟。

## 工項 tasks

注意：應用程式倉庫是本資料夾下的 `docusaurus` 資料夾下，下列工作都請在 `docusaurus` 資料夾下執行。

- [ ] 執行 `npx create-docusaurus@latest . classic --typescript` 初始化專案
- [ ] 安裝中文搜尋套件 `@easyops-cn/docusaurus-search-local`
- [ ] 驗證專案結構已正確建立 (src/, content/static/, content/docs/, content/blog/ 等目錄)
- [ ] 檢查 package.json 的 scripts 和依賴項設定
- [ ] 測試本地開發伺服器啟動 (`npm run start`)
- [ ] 測試建置流程 (`npm run build`) 
- [ ] 清理不需要的範例檔案，準備客製化配置
- [ ] 確保與現有 content/ 目錄不衝突

## 測試方式

請在 `docusaurus` 資料夾下驗證以下項目確認任務完成：
1. 執行 `ls -la` 確認 Docusaurus 專案目錄結構已建立
2. 檢查 `package.json` 包含必要的 Docusaurus 依賴和 scripts
3. 確認 `docusaurus.config.js` 和 `sidebars.js` 檔案存在
4. 執行 `npm install` 確保依賴安裝成功
5. 執行 `npm run start` 測試開發伺服器能正常啟動 (port 3000)
6. 執行 `npm run build` 測試建置流程成功，產生 `build/` 目錄
7. 檢查中文搜尋套件是否已正確安裝在 `package.json` 依賴中
8. 確認現有的 `content/` 目錄和 `README.md` 不受影響

## 完成流程

請在 3.tasks.md 本項 task 的 [ ] 打上 [x] 記號表示完成，打上 [?] 記號表示尚有待處理、之後再檢查事項。
做記號完後在 task 的「目前任務」更新到下一個任務
清除執行記憶
讀取並執行 prompt-003-create-each-task.txt
