# 2-3. 設定 GitHub Actions 工作流程

## 描述

在內容倉庫中建立 GitHub Actions 工作流程檔案，設定當內容更新時自動觸發部署流程。透過 repository_dispatch 機制與應用程式倉庫進行通訊，實現跨倉庫的自動化部署流程。目錄在 `whyblog-docusaurus/content`

## 工項 tasks

- [ ] 建立 `.github/workflows/trigger-deploy.yml`
- [ ] 配置 repository_dispatch 觸發機制
- [ ] 測試 push 與 PR 合併觸發條件

## 測試方式

請透過以下方式驗證任務已成功：
1. 確認 `.github/workflows/trigger-deploy.yml` 檔案存在且格式正確
2. 驗證 repository_dispatch 設定正確，包含正確的 token 與目標倉庫
3. 測試工作流程在 push 事件時能正確觸發
4. 測試工作流程在 PR 合併時能正確觸發
5. 確認工作流程能成功發送 repository_dispatch 事件

## 完成流程

請在 3.tasks.md 本項 task 的 [ ] 打上 [x] 記號表示完成，打上 [?] 記號表示尚有待處理、之後再檢查事項。
做記號完後在 task 的「目前任務」更新到下一個任務
清除執行記憶
讀取並執行 prompt-003-create-each-task.txt
