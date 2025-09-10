# 1-4. 確認 GitHub Pages 功能可用性

## 描述

驗證 GitHub 帳戶是否具備 GitHub Pages 功能，並確認相關設定正確。這是建置雙 Repository 架構的必要前置條件，需要確保應用程式倉庫能夠透過 GitHub Pages 正常部署和提供網站服務。

## 工項 tasks

- [ ] 檢查 GitHub 帳戶的 Pages 功能權限
- [ ] 確認應用程式倉庫 (whyblog-docusaurus) 的 Pages 設定
- [ ] 驗證 GitHub Actions 部署至 Pages 的權限配置
- [ ] 測試基本的 Pages 部署流程
- [ ] 檢查自訂網域設定選項 (如有需要)
- [ ] 確認 HTTPS 強制執行設定

## 測試方式

1. 前往 GitHub 倉庫設定頁面的 Pages 選項卡
2. 確認能看到 Pages 設定選項且無權限限制警告
3. 測試能夠選擇 "GitHub Actions" 作為 Source
4. 建立簡單的測試 HTML 檔案並成功透過 Pages 訪問
5. 驗證 Actions 工作流程具備部署至 Pages 的必要權限

## 完成流程

請在 3.tasks.md 本項 task 的 [ ] 打上 [x] 記號表示完成，打上 [?] 記號表示尚有待處理、之後再檢查事項。
做記號完後在 task 的「目前任務」更新到下一個任務
清除執行記憶
讀取並執行 prompt-003-create-each-task.txt