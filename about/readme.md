# 🌐 Amanda Wu - 數位設計師個人作品集網站 (Digital Designer Portfolio)

![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![Tech Stack](https://img.shields.io/badge/stack-HTML5%20%7C%20TailwindCSS%20%7C%20JS%20%7C%20GAS-purple.svg)

本專案為 **吳文瑜 (Amanda Wu)** 的個人數位作品集網站源碼。採用現代深色宇宙風格與霓虹燈光視覺效果設計，展示 13 年數位設計與 Web 前端開發經驗，並包含跨網域串接 Google Apps Script (GAS) 的動態聯絡表單功能。

---

## ✨ 網站亮點 (Features)

- **🌌 現代科技感 UI/UX**：採用 Dark Space 主題，搭配動態 Glow 光暈與磨砂玻璃質感 (Glassmorphism)。
- **📱 全響應式設計 (RWD)**：完美適應 Desktop、Tablet 與 Mobile 等各式螢幕尺寸，具備滑順的選單切換與錨點滾動。
- **⚡ 高效能與極簡架構**：使用 Single Page Application (SPA) 概念，利用 CDN 引入 Tailwind CSS 與 Font Awesome 實現輕量化與快速載入。
- **📩 Google 試算表表單串接**：聯絡表單採用 **JSONP / Google Apps Script** 技術，繞過跨網域 (CORS) 限制，直接將訪客留言寫入後端 Google Sheet。

---

## 🛠️ 技術棧 (Tech Stack)

* **UI / Front-End:** HTML5, CSS3, JavaScript (ES6+)
* **Styling Framework:** [Tailwind CSS (v3)](https://tailwindcss.com/)
* **Icon Library:** [Font Awesome (v6)](https://fontawesome.com/)
* **Typography:** Google Fonts (Inter, Noto Sans TC)
* **Backend Automation:** Google Apps Script (GAS) + Google Sheets API

---

## 📂 檔案結構 (File Structure)

```text
.
├── index.html        # 作品集主要網頁檔 (包含 UI 佈局、樣式設定與前端邏輯)
└── README.md         # 專案說明文件
```

---

## ⚙️ Google Apps Script (GAS) 聯絡表單後端設定指南

若您欲使用自己的 Google 試算表接收聯絡表單訊息，請參考以下步驟設定：

### 1. 建立 Google 試算表 (Google Sheet)
1. 新增一個 Google 試算表。
2. 在第一列（Row 1）依序填入欄位名稱：`Timestamp` | `Name` | `Email` | `Type` | `Message`。

### 2. 設定 Google Apps Script (GAS)
1. 在試算表上方選單點選 **擴充功能 (Extensions) > Apps Script**。
2. 將以下程式碼貼入 `Code.gs`：

```javascript
function doGet(e) {
  var params = e.parameter;
  var sheet = SpreadsheetApp.getActiveSpreadsheet().getActiveSheet();
  
  // 寫入資料
  sheet.appendRow([
    new Date(),
    params.name,
    params.email,
    params.type,
    params.message
  ]);

  // 以 JSONP 格式回傳
  var callback = params.callback;
  var result = JSON.stringify({ result: 'success' });
  var output = callback + '(' + result + ')';

  return ContentService.createTextOutput(output)
    .setMimeType(ContentService.MimeType.JAVASCRIPT);
}
```

### 3. 部署 Web 應用程式 (Deploy)
1. 點擊右上角 **部署 (Deploy) > 新增部署 (New deployment)**。
2. 種類選擇 **Web 應用程式 (Web app)**。
3. 設定：
   - **執行者 (Execute as)**：`Me (我自己)`
   - **誰有存取權限 (Who has access)**：`Anyone (所有人)`
4. 點擊 **部署**，並複製發布後的 **Web App URL**。
5. 開啟 `index.html`，尋找 `<input type="hidden" id="gas-url" value="...">`，將 `value` 替換為您的 Web App URL 即可。

---

## 🚀 快速上手 (Quick Start)

1. **Clone 本專案：**
   ```bash
   git clone https://github.com/your-username/amanda-wu-portfolio.git
   ```
2. **運行專案：**
   本專案為純前端網頁，無需繁瑣安裝步驟。只需在瀏覽器中直接開啟 `index.html` 或搭配 VS Code 的 `Live Server` 套件即可運行。

---

## 📄 授權條款 (License)

本專案基於 [MIT License](LICENSE) 條款開源發布。
