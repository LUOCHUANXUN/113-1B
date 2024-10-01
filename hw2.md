# PERT/CPM 圖
```mermaid
graph TD;
    A[研擬計畫] --> B[任務分配];
    A --> C[取得硬體];
    B --> D[程式開發];
    C --> E[安裝硬體];
    D --> F[程式測試];
    D --> G[撰寫使用手冊];
    E --> H[轉換檔案];
    F --> I[系統測試];
    G --> J[使用者訓練];
    H --> J;
    I --> K[使用者測試];
    J --> K;
```markdown
# 甘特圖
```mermaid
gantt
    dateFormat  YYYY-MM-DD
    title 任務甘特圖
    section 任務
    研擬計畫 :done, 2024-10-01, 1d
    任務分配 :active, after A, 4d
    取得硬體 :done, after A, 17d
    程式開發 :active, after B, 70d
    安裝硬體 :done, after C, 10d
    程式測試 :done, after D, 30d
    撰寫使用手冊 :done, after D, 25d
    轉換檔案 :done, after E, 5d
    系統測試 :done, after F, 20d
    使用者訓練 :done, after G, 20d
    使用者測試 :done, after H, 25d

```markdown
# 關鍵路徑

關鍵路徑為：`1 -> 2 -> 4 -> 6 -> 9 -> 11`，總耗時為 146 天。
