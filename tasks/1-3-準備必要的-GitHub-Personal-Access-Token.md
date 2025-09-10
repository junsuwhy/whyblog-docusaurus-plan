# 1-3. 準備必要的 GitHub Personal Access Token

## 描述

為了實現雙 Repository 架構中的 repository_dispatch 觸發機制，需要準備具有適當權限的 GitHub Personal Access Token。此 token 將用於內容倉庫觸發應用程式倉庫的部署流程，以及應用程式倉庫讀取內容倉庫的內容。

## 工項 tasks

- [ ] 建立內容倉庫使用的 `REPO_DISPATCH_TOKEN`
  - [ ] 登入 GitHub，進入 Settings > Developer settings > Personal access tokens > Tokens (classic)
  - [ ] 建立新 token，命名為 "whyblog-repo-dispatch"
  - [ ] 設定權限：勾選 `public_repo` (Access public repositories)
  - [ ] 複製並安全存儲 token 值
- [ ] 建立應用程式倉庫使用的 `CONTENT_REPO_TOKEN`
  - [ ] 建立另一個新 token，命名為 "whyblog-content-read"  
  - [ ] 設定權限：勾選 `public_repo` (Read access to public repositories)
  - [ ] 複製並安全存儲 token 值
- [ ] 驗證 token 有效性
  - [ ] 測試 `REPO_DISPATCH_TOKEN` 能否觸發 repository_dispatch 事件
  - [ ] 測試 `CONTENT_REPO_TOKEN` 能否讀取內容倉庫

## 測試方式

AI 可以透過以下方式驗證任務成功：
1. 確認用戶已建立兩個 Personal Access Token
2. 確認 token 已正確設定權限 (public_repo)
3. 驗證 token 能夠成功存取目標倉庫
4. 確認用戶已安全存儲 token 值，準備用於後續的 GitHub Actions 配置

## 完成流程

請在 3.tasks.md 本項 task 的 [ ] 打上 [x] 記號表示完成，打上 [?] 記號表示尚有待處理、之後再檢查事項。
做記號完後在 task 的「目前任務」更新到下一個任務
清除執行記憶
重新讀取並執行 prompt-003-create-each-task.txt