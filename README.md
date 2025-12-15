# n8nAIDemo-RAG
使用n8n + Webhook + Zeabur + RAG架構佈署一個workflow，實作出一個可以上傳菜單並根據使用者需求推薦菜單菜色的Line bot。
* n8n + RAG 工作流模板

# workflow
<img width="1658" height="452" alt="image" src="https://github.com/user-attachments/assets/19e1bb55-8ce3-4738-b114-b30199829052" />
流程分為兩大部分:
1. 使用者上傳菜單(XLSX檔) -> 接收XLSX檔 -> 菜單轉換成json資料並儲存至全域變數 -> 回傳 "菜單上傳成功"
2. 使用者在聊天室輸入需求 -> 把菜單與使用者需求傳給LLM -> LLM將使用者需求轉換成限制條件 -> 篩選出符合條件的菜色 -> LLM結合候選菜色資訊與使用者需求產生推薦菜色 -> 輸出至Line聊天室

# Demo
<img width="1109" height="240" alt="image" src="https://github.com/user-attachments/assets/31338dce-fb38-45d4-a256-2d415afb0e58" />
<img width="1102" height="521" alt="image" src="https://github.com/user-attachments/assets/a03c0b3e-8948-49fb-a393-d8f53fb54ad4" />

# 教學影片
[n8n + Line bot + RAG教學影片](https://youtu.be/DTT2rzW2zNo)
