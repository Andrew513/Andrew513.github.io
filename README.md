# 個人作品集網站

一個現代化、響應式的個人作品集網站模板，可部署到 GitHub Pages。

## 🌟 特點

- **響應式設計** - 在所有設備上完美展示（桌面、平板、手機）
- **現代化風格** - 漸層、陰影、動畫和過渡效果
- **多頁面結構** - 首頁、關於、作品集、聯絡頁面
- **互動功能** - 作品篩選、表單驗證、平滑滾動
- **高性能** - 輕量級、無框架依賴
- **GitHub Pages 友善** - 完全靜態，可直接部署

## 📁 文件結構

```
portfolio/
├── index.html          # 首頁
├── about.html          # 關於頁面
├── portfolio.html      # 作品展示頁面
├── contact.html        # 聯絡頁面
├── styles.css          # 樣式表
├── script.js           # JavaScript 功能
└── README.md           # 說明文件
```

## 🚀 快速開始

### 本地預覽

1. 克隆或下載此項目
2. 用任何 Web 瀏覽器打開 `index.html`
3. 開始編輯檔案添加你的內容

### 自定義內容

#### 1. 基本信息
編輯以下檔案中的文本內容：
- `index.html` - 更改名字、職位和描述
- `about.html` - 新增個人故事和經驗
- `portfolio.html` - 新增或修改項目
- `contact.html` - 更新聯絡方式

#### 2. 顏色主題
在 `styles.css` 中編輯 CSS 變數：

```css
:root {
    --primary-color: #667eea;      /* 主色調 */
    --secondary-color: #764ba2;    /* 副色調 */
    --accent-color: #f5576c;       /* 強調色 */
    --dark-color: #1a1a2e;         /* 深色 */
    --light-color: #f7f7f7;        /* 淺色 */
    --text-color: #333;            /* 文字色 */
}
```

#### 3. 社交連結
在頁尾中更新社交媒體連結：
```html
<li><a href="https://github.com/你的用戶名" target="_blank">GitHub</a></li>
<li><a href="https://linkedin.com/in/你的用戶名" target="_blank">LinkedIn</a></li>
```

#### 4. 聯絡表單
目前表單只是記錄到控制台。要使其實際工作，可以整合：

**使用 Formspree（推薦）：**
1. 訪問 [formspree.io](https://formspree.io)
2. 建立新表單並獲取表單 ID
3. 在 `script.js` 中取消註釋 Formspree 代碼並添加你的表單 ID

**使用 EmailJS：**
1. 訪問 [emailjs.com](https://emailjs.com)
2. 設置電子郵件服務
3. 在 HTML 中新增 EmailJS 指令碼並配置

## 📱 頁面說明

### 首頁 (index.html)
- 英雄部分，包含歡迎文字
- 特色項目網格
- 技能部分
- 行動號召部分

### 關於頁面 (about.html)
- 個人簡介
- 工作經驗時間線
- 教育背景
- 個人故事

### 作品頁面 (portfolio.html)
- 項目網格展示
- 可篩選的項目類別
- 項目詳細信息
- 使用的技術標籤

### 聯絡頁面 (contact.html)
- 聯絡表單
- 聯絡信息（電話、郵箱、位置）
- 社交媒體連結
- 可用性狀態

## 🎨 自定義指南

### 更改項目圖像
用實際項目截圖替換佔位符梯度：

```html
<!-- 替換這個 -->
<div class="placeholder-image" style="background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);"></div>

<!-- 用這個 -->
<img src="path/to/your-image.jpg" alt="Project name">
```

### 添加新項目
複製一個項目卡片，修改內容：

```html
<div class="featured-card">
    <div class="card-image">
        <img src="project-image.jpg" alt="Project name">
    </div>
    <div class="card-content">
        <h3>你的項目名稱</h3>
        <p>項目描述...</p>
        <div class="tech-tags">
            <span class="tag">技術1</span>
            <span class="tag">技術2</span>
        </div>
    </div>
</div>
```

### 添加新的技能類別
在 skills 部分添加：

```html
<div class="skill-category">
    <h3>新類別</h3>
    <ul class="skill-list">
        <li>技能1</li>
        <li>技能2</li>
        <li>技能3</li>
    </ul>
</div>
```

## 🌐 部署到 GitHub Pages

### 方法 1：使用 GitHub 網頁界面（簡單）

1. 在 GitHub 上建立新倉庫，命名為 `你的用戶名.github.io`
2. 上傳所有檔案到倉庫
3. 倉庫會自動部署到 `https://你的用戶名.github.io`

### 方法 2：使用命令行（建議）

1. 初始化 Git 倉庫：
```bash
cd portfolio
git init
git add .
git commit -m "Initial commit"
```

2. 在 GitHub 上建立倉庫（命名為 `你的用戶名.github.io`）

3. 連接並推送：
```bash
git remote add origin https://github.com/你的用戶名/你的用戶名.github.io.git
git branch -M main
git push -u origin main
```

4. 訪問 `https://你的用戶名.github.io` 查看你的網站

### 方法 3：使用自定義域名

1. 購買域名（Namecheap、GoDaddy 等）
2. 在倉庫設置中添加自定義域名
3. 在 GitHub 倉庫根目錄新增 `CNAME` 檔案，內容為你的域名
4. 在域名提供商設置 DNS 記錄（A 或 CNAME）

## 🛠️ 技術棧

- **HTML5** - 語義化標記
- **CSS3** - 現代樣式（Flexbox、Grid、動畫）
- **JavaScript** - 互動功能（ES6+）
- **無框架** - 純原生 JavaScript

## 📊 性能最佳實踐

- ✅ 無外部依賴 - 快速載入
- ✅ 優化的 CSS - 最小化並組織良好
- ✅ 原生 JavaScript - 無框架開銷
- ✅ 響應式圖像 - 自適應設備
- ✅ 懶加載動畫 - 使用 Intersection Observer

## 🔧 可能的增強功能

- [ ] 添加暗黑模式切換
- [ ] 集成 Formspree/EmailJS 的聯絡表單
- [ ] 添加搜索功能
- [ ] 博客部分
- [ ] 用戶評論系統
- [ ] 多語言支持
- [ ] PWA 功能

## 📝 許可證

此項目開源免費使用。可自由修改和部署。

## 💡 提示

1. **測試響應式設計** - 使用瀏覽器開發者工具檢查不同設備
2. **SEO 優化** - 更新 meta 標籤中的描述
3. **性能** - 使用 Google PageSpeed Insights 檢查
4. **可訪問性** - 確保足夠的顏色對比度和 ARIA 標籤

## 🤝 貢獻

如果你有改進建議，歡迎提交 Issue 或 Pull Request。

---

**開始創建你的個人品牌！** 🚀

需要幫助？查看 `index.html` 了解代碼結構，或編輯 `styles.css` 自定義外觀。
