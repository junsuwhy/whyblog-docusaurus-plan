# 3-3. 配置 Docusaurus 核心設定檔案：設定檔 `docusaurus.config.js`

## 描述

配置 Docusaurus 的核心設定檔案 `docusaurus.config.js`，以建立完整的部落格與知識庫功能。根據雙 Repository + repository_dispatch 架構，需要設定正確的 GitHub Pages 部署參數、內容來源路徑、搜尋功能整合以及主題配置。

本任務將建立一個完整的 Docusaurus 配置，支援：
- 網站基本資訊與 SEO 設定
- GitHub Pages 部署設定
- 內容倉庫的 docs 和 blog 路徑對應
- 中英文搜尋功能整合
- 主題與自訂樣式載入

## 工項 tasks

- [ ] 設定網站基本資訊 (title: "My Blog & Knowledge Base", tagline, favicon)
- [ ] 配置 GitHub Pages 部署參數 (organizationName: "junsuwhy", projectName: "whyblog-docusaurus", baseUrl)
- [ ] 設定正確的 URL 結構 (`https://junsuwhy.github.io/whyblog-docusaurus/`)
- [ ] 配置內容來源路徑 (docs: './content/docs', blog: './content/blog')
- [ ] 整合中英文搜尋功能 (@easyops-cn/docusaurus-search-local)
- [ ] 設定主題與 preset 配置 (classic preset)
- [ ] 啟用 MDX 支援與自訂 CSS 載入 (./src/css/custom.css)
- [ ] 配置本地開發伺服器參數 (host: 'localhost')
- [ ] 設定導航欄與頁腳基本結構
- [ ] 驗證設定檔案語法正確性

## 測試方式

### TDD 驗證方法

1. **配置檔案語法驗證**：
   ```bash
   cd docusaurus
   npm run build --dry-run
   ```

2. **本地開發伺服器啟動測試**：
   ```bash
   cd docusaurus
   npm run start -- --host localhost --port 3000
   ```
   驗證能否在 `http://localhost:3000` 存取網站

3. **搜尋功能測試**：
   - 本地伺服器啟動後，檢查頁面是否有搜尋框
   - 嘗試搜尋中英文內容並驗證結果

4. **靜態建置測試**：
   ```bash
   cd docusaurus
   npm run build
   ```
   驗證建置成功且 `build` 資料夾生成

5. **設定檔案內容驗證**：
   ```bash
   cd docusaurus
   node -e "const config = require('./docusaurus.config.js'); console.log(JSON.stringify(config, null, 2));"
   ```
   檢查設定是否正確載入

## 環境與目錄配置

- **工作目錄**：`/home/debian/whyblog-docusaurus/docusaurus/`
- **設定檔案位置**：`./docusaurus.config.js`
- **內容來源路徑**：`./content/docs` 和 `./content/blog`
- **本地測試 IP**：`localhost` (VM 環境)
- **部署目標**：`https://junsuwhy.github.io/whyblog-docusaurus/`

## 完成流程

請在 3.plan.md 本項 task 的 [ ] 打上 [x] 記號表示完成，打上 [?] 記號表示尚有待處理、之後再檢查事項。
做記號完後在 task 的「目前任務」更新到下一個任務
清除執行記憶
讀取並執行 prompt-003-create-each-task.txt