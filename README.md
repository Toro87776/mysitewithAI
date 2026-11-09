# 🌐 My Web Portfolio — 吳文瑜 (Amanda Wu)

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-Ready-blue.svg)](https://toro87776.github.io/mysitewithAI/)
[![Stack: HTML5 | TailwindCSS | JS ES6+](https://img.shields.io/badge/Stack-HTML5%20%7C%20TailwindCSS%20%7C%20JS-purple.svg)](#-tech-stack--apis)
[![Responsive: Mobile First](https://img.shields.io/badge/Design-Mobile--First-cyan.svg)](#-features)

歡迎來到 **吳文瑜 (Amanda Wu)** 的個人數位作品集網站源碼庫。  
本專案採現代深色宇宙風格與動態霓虹光暈（Glassmorphism）設計，具備極致滑順的**行動端優先（Mobile-First）**體驗。專案完整匯整了 13 年跨足數位設計、UI/UX 原型規劃、全響應式前端切版、商業數據儀表板，以及 AI 輔助開發的實戰作品。

---

## 🚀 專案線上即時演示 (Live Demo)

* **主要入口網站**：`index.html` (My Web Portfolio)
* **設計師個人簡歷**：`about/index.html`
* **GitHub Pages 部署網址**：[https://toro87776.github.io/mysitewithAI/](https://toro87776.github.io/mysitewithAI/)

---

## ✨ 網站亮點 (Features)

- **📱 行動端優先 (Mobile-First Architecture)**：專為手機螢幕設計拇指熱區導航列（Home、Catalog、Projects、About、Music），適配各式螢幕尺寸與安全邊距 (`viewport-fit=cover`)。
- **📂 互動專案目錄 (Interactive Catalog)**：支援即時關鍵字模糊搜尋，以及「全部」、「互動 Web Apps」、「數據與企業系統」、「視覺與架構」等快速分類標籤切換。
- **💳 深度專案卡片 (Detailed Project Cards)**：每個專案皆附有 100 字核心介紹、使用的 API 與技術清單、實際應用場景（Use Cases），以及一鍵啟動按鈕。
- **🎵 背景音頻控制器 (Audio Bar)**：具備動態音波視覺化動畫、播放/暫停與音量調控。
- **🖼️ 藍圖燈箱預覽 (Modal Preview)**：支援點擊直接放大檢視系統架構圖與資訊圖表大圖。
- **📩 Google 試算表表單串接**：聯絡表單採用 **JSONP / Google Apps Script (GAS)** 技術，繞過跨網域 CORS 限制，直接將訪客留言寫入後端 Google Sheet。

---

## 📦 收錄專案與互動 Web 應用 (Included Projects)

### 1. 🌤️ 台灣即時天氣觀測站 (`apps/weather.html`)
* **介紹**：採用 Bento Grid（便當盒風格）模組化介面設計，即時整合中央氣象署觀測站數據，提供每小時即時氣溫、降雨機率預警、紫外線強度、體感溫差及空氣品質指標（AQI），搭配動態溫差趨勢圖與風速風向圖表。
* **技術/API**：中央氣象署觀測資料 API、Browser Geolocation API、Chart.js Canvas API、Fetch RESTful JSON API。
* **應用場景**：通勤穿著決策、戶外活動預警、旅行者隨身氣候助理。

### 2. 📊 鼎盛銷售經營診斷儀表板 (`apps/DingSangCo. Pseudonymized sales analyze Dashboard .html`)
* **介紹**：專為企業高階決策者與業務主管打造的商業診斷儀表板。內建超過 820 筆 B2B 擬真銷售訂單分析引擎，支援即時拖曳上傳外部 Excel 與 CSV 檔案。涵蓋 Pareto 虧損原因深度歸因、業務員折扣越權偵測、大客戶集中度風險評估及退貨成本損耗分析。
* **技術/API**：SheetJS (XLSX.js) API、Chart.js Multi-Axis / Bubble API、HTML5 Drag & Drop API、FileReader API。
* **應用場景**：企業月度董事會營運健檢、通路毛利稽核、業務經理業績與折扣核定。

### 3. 🌿 森語塔羅・心靈占卜 (`apps/Taro forest style.html`)
* **介紹**：深翠森林風格之沉浸式 Web 應用程式。內建完整 78 張偉特塔羅牌（22 張大阿爾克那與 56 張小阿爾克那），支援正逆位解讀、真實物理洗牌動態與流暢 3D 卡牌翻轉動畫。提供單張啟示、過去現在未來以及身心靈三角牌陣，占卜紀錄自動同步本機。
* **技術/API**：Web Storage API (localStorage)、CSS 3D Transforms / Perspective Engine、DOM Events & Audio Feedback。
* **應用場景**：個人每日冥想指引、工作轉折自我對話、心理諮商破冰小工具。

### 4. 🏢 部門階層架構與人員異動系統 (`apps/department_organizational_hierarchy_personnel_transfer_system.html`)
* **介紹**：專為中大型企業設計的人資組織架構與人員調動平台。透過直觀的樹狀圖層級視覺化，即時呈現企業跨事業群、部門及團隊的從屬關係與各層級員額編制，具備組織階層靈活調整、員工職等薪級設定與完整的人事調動歷程稽核紀錄。
* **技術/API**：DOM Tree Traversal & Hierarchical Mutation API、Modal & Event Delegation API、JSON State Persistence Engine。
* **應用場景**：組織重整、年度員額編制規劃 (Headcount Budgeting)、跨專案小組人員借調。

### 5. 💼 吳文瑜 個人數位設計作品集 (`about/index.html`)
* **介紹**：數位設計師吳文瑜的個人品牌主頁。匯聚 13 年跨足品牌 CIS 識別、UI/UX 產品原型、活動行銷素材切版（如國泰雲門隨行吧、膳魔師、泰安產險、美津濃）之實戰成果，頁尾整合 Google Apps Script 動態表單。
* **技術/API**：Google Apps Script (GAS) Web App API、JSONP 跨網域傳輸、Google Sheets API、Tailwind CSS。

### 6. 🎨 視覺設計與專案資產 (`assets/`)
* **🏪 巷仔內文具行智慧營銷系統** (`assets/Sationary store notion application.png`)：Notion 進銷存與日常營運管理系統架構。
* **🐶 YongGO 幼犬問卷洞察資訊圖** (`assets/YongGo project Inforgraphic.png`)：寵物飼主需求調研與視覺化資訊圖表。
* **📐 網站整體資訊架構規劃圖** (`assets/website-infographic.png`)：大型數位平台 IA 階層、線框原型與 User Flow 藍圖。

---

## 🛠️ 技術棧 (Tech Stack & APIs)

| 領域 | 使用技術 / 工具 |
| :--- | :--- |
| **前端核心** | HTML5, CSS3, JavaScript (ES6+), Modern DOM APIs |
| **UI 與樣式** | [Tailwind CSS (v3)](https://tailwindcss.com/), Glassmorphism, 3D CSS Transforms |
| **圖標與字型** | [Font Awesome (v6)](https://fontawesome.com/), Google Fonts (Inter, Noto Sans TC) |
| **數據圖表** | [Chart.js (v4)](https://www.chartjs.org/) (Line, Bar, Bubble, Pareto, Doughnut) |
| **檔案解析** | [SheetJS (xlsx.full.min.js)](https://sheetjs.com/) (Excel / CSV 前端即時解析) |
| **本機儲存與狀態** | HTML5 Web Storage API (localStorage), Drag & Drop API, FileReader API |
| **後端自動化** | Google Apps Script (GAS) + Google Sheets API (無伺服器表單接收) |

---

## 📂 檔案目錄結構 (Directory Structure)

```text
mysite_ai/
├── index.html         # 核心入口網站 (My Web Portfolio 主頁，包含專案目錄、卡片展示與 About Me)
├── README.md          # 專案完整說明文件
├── .gitignore         # Git 忽略配置檔
│
├── about/             # 設計師個人主頁與後端說明
│   ├── index.html     # 吳文瑜 Amanda Wu 詳細簡歷、重要專案與 GAS 聯絡表單
│   └── readme.md      # Google Apps Script (GAS) 部署指引
│
├── apps/              # 獨立互動 Web 應用程式
│   ├── weather.html                                                # 台灣即時天氣觀測站
│   ├── DingSangCo. Pseudonymized sales analyze Dashboard .html     # 鼎盛銷售經營診斷儀表板
│   ├── Taro forest style.html                                      # 森語塔羅・心靈占卜
│   └── department_organizational_hierarchy_personnel_transfer_system.html # 部門組織與人員調動系統
│
├── assets/            # 設計資產、系統藍圖與肖像
│   ├── Sationary store notion application.png                      # 文具行 Notion 系統圖
│   ├── YongGo project Inforgraphic.png                             # 幼犬調研資訊圖
│   ├── website-infographic.png                                     # 網站 IA 架構圖
│   └── selfie.png                                                  # 個人形象肖像照
│
└── music/             # 品牌音效資產
    └── intro.mp3      # 品牌前導環境音樂
```

---

## 🚀 本地運行 (Local Development)

本專案為輕量純靜態 Web 架構，無需任何 Node.js 依賴或編譯打包步驟：

1. **Clone 本專案：**
   ```bash
   git clone https://github.com/Toro87776/mysitewithAI.git
   cd mysitewithAI
   ```

2. **直接開啟：**
   在瀏覽器中雙擊開啟 `index.html`，或使用 VS Code 套件 **Live Server** 運行即可享受完整功能。

---

## 🌍 GitHub Pages 免費公開部署步驟

若欲啟用 GitHub Pages 將作品集公開上線：
1. 進入本儲存庫的 **Settings** > **Pages**。
2. 在 **Branch** 處選擇 `main` 分支，資料夾選擇 `/ (root)`。
3. 點選 **Save**，約 1~2 分鐘後即可透過 `https://toro87776.github.io/mysitewithAI/` 訪問公開網站！

---

## 👤 作者資訊 (Author)

* **設計師**：吳文瑜 (Amanda Wu)
* **GitHub**：[@Toro87776](https://github.com/Toro87776)
* **聯絡信箱**：bmandawu@gmail.com
* **專長領域**：UI / UX 設計、RWD 響應式前端、品牌視覺 CIS、商業數據儀表板

---

## 📄 授權條款 (License)

本專案基於 [MIT License](LICENSE) 條款開源發布。
