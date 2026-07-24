# 階梯渠底水理分析與靜水池設計檢算系統 (Stepped Spillway Hydraulics & Stilling Basin Design Tool)

這是一個專為土木、水利與水土保持工程設計人員開發的網頁端計算工具。本系統旨在簡化階梯式渠道（Stepped Spillway / Stepped Chute）的水理計算，並針對下游靜水池（Stilling Basin）進行幾何與水理檢算，提供直觀、即時的分析與視覺化回饋。

---

## 🌟 系統特色

*   **直觀的參數輸入**：支援設計流量 ($Q$)、渠道寬度 ($B$)、階高 ($h$)、階長 ($l$)、總落差 ($H_{total}$) 等關鍵幾何與水理參數輸入。
*   **坡度防呆警示**：系統自動檢算坡度比值 ($h/l$)。若坡度角過陡（大於 45°），將自動觸發警告，防止不切實際的設計。
*   **下游靜水池檢算**：輸入設計池長 ($L_d$)，系統將自動進行水躍（Hydraulic Jump）計算，檢算靜水池長度與流速是否滿足最大容許流速 ($v_{allow}$) 等規範要求。
*   **動態視覺化示意**：提供即時的渠道與水理狀態示意圖，幫助設計人員快速評估水理表現。
*   **現代化 UI/UX**：採用精美、流暢的現代網頁設計，支援深色模式（Dark Mode）切換，適應不同工作環境。

---

## 🚀 如何在 GitHub 上使用（GitHub Pages 部署）

本系統為純前端應用（HTML5 + Tailwind CSS + JavaScript），**無須任何後端伺服器或資料庫**，極度適合直接託管於 GitHub Pages 免費網頁空間。

### 部署步驟

1.  **建立 Repository**：在您的 GitHub 帳號下建立一個新的儲存庫（Repository，例如命名為 `stepflow-calc`）。
2.  **上傳檔案**：將此專案的所有檔案（包括 `index.html`）上傳至該儲存庫。
3.  **啟用 GitHub Pages**：
    *   進入該儲存庫的 **Settings**（設定）。
    *   在左側選單點擊 **Pages**。
    *   在 **Build and deployment** 下的 **Branch**，將分支選擇為 `main`（或 `master`），目錄選擇 `/ (root)`，然後點擊 **Save**。
4.  **開始使用**：等待約 1~2 分鐘，GitHub 會提供給您一個專屬網址（例如：`https://<您的帳號>.github.io/stepflow-calc/`），您就可以直接在瀏覽器上使用這個系統了！

---

## 💻 本地執行方式

本專案完全不需要安裝任何相依套件，您可以透過以下兩種方式在本地電腦執行：

1.  **直接開啟**：雙擊 `index.html` 即可在瀏覽器中運行。
2.  **使用開發伺服器（推薦）**：
    *   如果您使用 Visual Studio Code，推薦安裝 **Live Server** 擴充套件，並右鍵選擇 `Open with Live Server` 運行，體驗更佳。

---

## 📂 檔案目錄結構

```text
StepFlow/
├── index.html        # 系統主程式 (包含 HTML、CSS 樣式與計算邏輯)
├── .gitignore        # Git 忽略檔案設定
└── README.md         # 本說明文件
```

---

## 🛠️ 開發與維護

本系統採用以下技術開發：
*   **Core**: HTML5, Vanilla JavaScript
*   **Styling**: Tailwind CSS (經由 CDN 載入)
*   **Icons**: Font Awesome

如果您有任何修改建議或發現計算邏輯需要調整，歡迎在 GitHub 提交 Issue 或 Pull Request！
