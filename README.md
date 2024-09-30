# hw2.md

## PERT/CPM 圖視覺化

```mermaid
graph TD;
    A[研擬計畫<br/>1天] --> B[任務分配<br/>4天];
    A --> C[取得硬體<br/>17天];
    B --> D[程式開發<br/>70天];
    C --> E[安裝硬體<br/>10天];
    D --> F[程式測試<br/>30天];
    E --> G[撰寫使用手冊<br/>25天];
    E --> H[轉換檔案<br/>20天];
    F --> I[系統測試<br/>25天];
    G --> J[使用者訓練<br/>20天];
    H --> J;
    I --> K[使用者測試<br/>25天];
    J --> K;


```

---




## 甘特圖視覺化
```mermaid
gantt
    dateFormat  YYYY-MM-DD
    title gantt

    section 研擬階段
    研擬計畫      :done, des1, 2024-10-01, 1d

    section 分配階段
    任務分配      :active, des2, 2024-10-02, 4d
    取得硬體      :done, des3, 2024-10-02, 17d

    section 開發階段
    程式開發      :active, des4, 2024-10-06, 70d
    安裝硬體      :done, des5, 2024-10-19, 10d

    section 測試階段
    程式測試      :active, des6, 2024-12-15, 30d
    撰寫使用手冊  :active, des7, 2024-10-29, 25d
    轉換檔案      :done, des8, 2024-10-29, 20d
    系統測試      :des9, 2025-01-14, 25d
    使用者訓練    :des10, 2024-11-23, 20d
    使用者測試    :des11, 2025-02-08, 25d


