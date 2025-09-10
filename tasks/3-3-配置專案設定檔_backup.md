# 3-3. 配置專案設定檔

## 描述

配置 Docusaurus 專案的核心設定檔案，包含網站基本資訊、部署參數、內容路徑設定，以及側邊欄結構與依賴管理等設定，為後續的自動化部署和網站功能奠定基礎。

## 工項 tasks

- [ ] 3-3-1. 設定 `docusaurus.config.js`
  - [ ] 配置網站基本資訊 (title, tagline, url)
  - [ ] 設定 GitHub Pages 部署參數
  - [ ] 配置內容路徑指向 `./content/`
  - [ ] 啟用中英文搜尋功能
- [ ] 3-3-2. 設定 `sidebars.js` 側邊欄結構
- [ ] 3-3-3. 更新 `package.json` 腳本與依賴

## 測試方式

1. 驗證 `docusaurus.config.js` 設定檔語法正確且包含所有必要參數
2. 確認側邊欄設定檔 `sidebars.js` 結構完整
3. 檢查 `package.json` 包含正確的腳本命令
4. 執行 `npm run build` 確認專案能正常建置
5. 執行 `npm run start` 確認本地開發伺服器能正常運行

## 完成流程

請在 3.tasks.md 本項 task 的 [ ] 打上 [x] 記號表示完成，打上 [?] 記號表示尚有待處理、之後再檢查事項。
做記號完後在 task 的「目前任務」更新到下一個任務
清除執行記憶
讀取並執行 prompt-003-create-each-task.txt