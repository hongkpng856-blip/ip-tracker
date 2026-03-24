# IP 追蹤器 | Visitor IP Tracker

## 📖 功能說明

這是一個部署在 GitHub Pages 上的 IP 追蹤網站，可以：

- ✅ **自動獲取訪客 IP 地址**
- ✅ **顯示 IP 詳細資訊**（國家、城市、ISP、時區、經緯度）
- ✅ **統計訪問數據**（總訪問次數、獨立 IP 數、今日訪問、國家數）
- ✅ **記錄訪問歷史**（最近 50 筆）
- ✅ **匯出 JSON 資料**
- ✅ **清除記錄功能**

## 🌐 線上網站

部署完成後，網站將位於：
```
https://hongkpng856-blip.github.io/ip-tracker/
```

## 🔧 技術說明

### 前端技術
- **純 HTML + CSS + JavaScript**（無需後端）
- **響應式設計**（支援手機、平板、桌面）
- **現代化 UI**（漸層背景、毛玻璃效果）

### API 使用
- **主要 API**: [ipapi.co](https://ipapi.co)（免費，每月 1000 次請求）
- **備用 API**: [ipify.org](https://www.ipify.org)

### 資料儲存
- 使用瀏覽器 **localStorage** 儲存記錄
- 最多保存 500 筆記錄
- 資料僅存在使用者裝置上，不會上傳到伺服器

## 📊 統計功能

| 統計項目 | 說明 |
|----------|------|
| 總訪問次數 | 所有時間的訪問總數 |
| 獨立 IP 數 | 不同 IP 地址的數量 |
| 今日訪問 | 當天的訪問次數 |
| 國家/地區 | 訪問者來自的不同國家數量 |

## 🚀 部署步驟

1. 建立 GitHub Repository
2. 上傳 `index.html` 和 `README.md`
3. 在 Repository Settings → Pages 啟用 GitHub Pages
4. 選擇 Branch: `main`, Folder: `/ (root)`
5. 等待部署完成（約 1-2 分鐘）

## 📝 注意事項

### GitHub Pages 的限制
- **靜態託管**：無法執行後端代碼（如 Flask/Python）
- **客戶端儲存**：記錄存在使用者瀏覽器，不同裝置/瀏覽器會有不同記錄
- **API 限制**：ipapi.co 免費版每月 1000 次請求

### 如需後端追蹤
如果需要跨裝置、跨瀏覽器共享記錄，需要：
1. 部署後端服務（如 PythonAnywhere、Render）
2. 使用資料庫儲存記錄
3. 詳見 `memory/2026-03-24.md` 中的部署說明

## 📁 檔案結構

```
ip-tracker-github/
├── index.html    # 主頁面（包含 HTML/CSS/JS）
└── README.md     # 說明文件
```

## 🔗 相關連結

- [ipapi.co API 文件](https://ipapi.co/api/)
- [GitHub Pages 文件](https://docs.github.com/zh/pages)

---
*建立時間：2026-03-24 10:15 GMT+8*
