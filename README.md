# 🌟 9Starmax 報價單系統部署指南

這是一個完整的商品報價單管理系統，專為玖星吉國際貿易設計。

## 📋 系統功能

- ✅ 客戶資訊管理
- ✅ 商品明細管理  
- ✅ 自動價格計算
- ✅ 報價單生成與列印
- ✅ PDF/圖片輸出
- ✅ 響應式設計
- ✅ 完整的法律聲明

## 🚀 部署方案

### 方案一：GitHub Pages（免費推薦）

1. **準備工作**
   ```bash
   # 將 9Starmax.html 重新命名為 index.html
   mv 9Starmax.html index.html
   ```

2. **創建 GitHub 倉庫**
   - 到 [GitHub](https://github.com) 註冊帳號
   - 創建新的公開倉庫（名稱：`9starmax-website`）
   - 上傳 `index.html` 檔案

3. **啟用 GitHub Pages**
   - 進入倉庫 → Settings → Pages
   - Source 選擇 "Deploy from a branch"
   - Branch 選擇 "main"
   - 點擊 Save

4. **設定自定義域名**
   - 在 Pages 設定中，Custom domain 輸入：`9starmax.com`
   - 勾選 "Enforce HTTPS"

### 方案二：Netlify（簡單快速）

1. **註冊 Netlify**
   - 到 [Netlify](https://netlify.com) 註冊帳號

2. **拖拽部署**
   - 將您的 HTML 檔案拖到 Netlify 部署區域
   - 等待部署完成

3. **設定域名**
   - Site settings → Domain management
   - Add custom domain → 輸入 `9starmax.com`

### 方案三：Vercel（開發者友好）

1. **註冊 Vercel**
   - 到 [Vercel](https://vercel.com) 註冊帳號

2. **部署專案**
   - 連接 GitHub 倉庫或直接上傳檔案
   - 選擇專案進行部署

3. **域名設定**
   - Project Settings → Domains
   - 添加 `9starmax.com`

## 🌐 DNS 設定

### 使用 GitHub Pages

在您的域名註冊商設定以下 DNS 記錄：

```
類型: A
名稱: @
值: 185.199.108.153

類型: A  
名稱: @
值: 185.199.109.153

類型: A
名稱: @  
值: 185.199.110.153

類型: A
名稱: @
值: 185.199.111.153

類型: CNAME
名稱: www
值: yourusername.github.io
```

### 使用 Netlify/Vercel

通常這些平台會提供自動的 DNS 設定指引，按照其指示操作即可。

## 📁 檔案結構

```
9starmax-website/
├── index.html          # 主要的報價單系統
├── README.md           # 本說明文件
└── CNAME              # 域名設定檔（自動生成）
```

## 🛠️ 本地測試

如果您想在本地測試：

```bash
# 使用 Python 開啟本地伺服器
python -m http.server 8000

# 或使用 Node.js
npx serve .

# 然後在瀏覽器開啟 http://localhost:8000
```

## ⚡ 效能優化建議

1. **啟用 HTTPS**
   - 所有主流託管平台都提供免費 SSL
   - 確保啟用 "Force HTTPS" 選項

2. **設定快取**
   - 大多數託管平台會自動處理
   - 靜態資源會被適當快取

3. **壓縮優化**
   - HTML/CSS/JS 會自動被壓縮
   - 圖片建議使用 WebP 格式

## 🔧 自定義設定

### 修改公司資訊

在 `index.html` 中找到以下區域並修改：

```html
<div class="company-info">
    <div class="company-logo" id="logo-container">
        <span class="default-logo-text">玖星吉國際貿易</span>
    </div>
    <p>統編：89061654</p>
    <p>電話：02-7709-4666</p>
    <p>信箱：Service@9Starmax.com</p>
</div>
```

### 修改銀行資訊

找到銀行資訊區域並更新：

```html
<div class="bank-info content-box-white">
    <div class="info-group">
        <p><span class="info-label">金融機構：</span><span>第一銀行</span></p>
        <p><span class="info-label">機構分支：</span><span>東港分行</span></p>
        <!-- 其他銀行資訊 -->
    </div>
</div>
```

## 🌍 SEO 優化

系統已包含基本的 SEO 優化：

- ✅ 適當的 meta 標籤
- ✅ Open Graph 標籤  
- ✅ 響應式設計
- ✅ 語義化 HTML
- ✅ 快速載入時間

## 📱 瀏覽器支援

- ✅ Chrome 60+
- ✅ Firefox 55+  
- ✅ Safari 12+
- ✅ Edge 79+
- ✅ 手機瀏覽器

## 🔒 安全性

- ✅ 無伺服器架構，無後端安全風險
- ✅ HTTPS 加密
- ✅ 無資料庫，無 SQL 注入風險
- ✅ 純前端運作，安全性高

## 📞 技術支援

如果您在部署過程中遇到問題：

1. **檢查 DNS 傳播**
   - 使用 [DNS Checker](https://dnschecker.org) 檢查
   - DNS 更新可能需要 24-48 小時

2. **清除快取**
   - 清除瀏覽器快取
   - 嘗試無痕模式瀏覽

3. **檢查檔案**
   - 確認 `index.html` 檔案完整
   - 確認檔案編碼為 UTF-8

## 🎯 下一步

部署完成後，您可以：

1. **測試功能**
   - 填寫報價單
   - 測試列印功能
   - 檢查響應式設計

2. **培訓員工**
   - 教導如何使用系統
   - 建立操作手冊

3. **蒐集回饋**
   - 記錄使用問題
   - 規劃功能改進

---

## 🔄 更新系統

當需要更新系統時：

1. **GitHub Pages**
   - 直接在 GitHub 上編輯檔案
   - 或本地修改後推送

2. **Netlify/Vercel**  
   - 重新上傳檔案
   - 或連接 Git 倉庫自動部署

---

**🎉 恭喜！您的 9Starmax 報價單系統即將上線！**

如需進一步的客製化或技術支援，歡迎隨時詢問。 