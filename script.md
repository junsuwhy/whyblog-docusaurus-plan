### 寫 Issue 

```
claude -p -d --verbose --allowedTools="Edit,WriteFile,Bash,mcp__discord-webhook__discord-send-embed" --permission-mode=acceptEdits "請讀取 @prompts/003-create-each-task.txt 並執行裡面的動作"
```

### 執行 Issue

```
claude -p -d --verbose --allowedTools="Edit,WriteFile,Bash,mcp__discord-webhook__discord-send-embed" "請讀取 @prompts/004-execute-task.txt 並執行裡面的動作"
```

### 跳過 Issue

```
claude -p -d --allowedTools="Edit,WriteFile" "請讀取 @prompts/005-skip-task.txt 並執行裡面的動作"
```

### 提供手工測試方式說明

```
claude -p -d --allowedTools="Edit,WriteFile" "請讀取 @prompts/006-evaluate-intro-task.txt 並執行裡面的動作"
```