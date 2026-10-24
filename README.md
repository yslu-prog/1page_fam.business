# 榮泰油行 一頁式網站

純 HTML，一個檔案就是整個網站，不需要安裝任何東西。

## 上線前要填的資料

在 `index.html` 裡搜尋並取代：

| 佔位文字 | 換成 |
|---|---|
| `[電話]` | 電話號碼。`tel:` 連結裡請寫成不含空格與橫線的格式，例如 `tel:0227001234` |
| `[LINE-ID]` | LINE 官方帳號 ID（含 @，例如 `@rongtai`）。按鈕會直接開啟加好友頁面 |

JSON-LD 結構化資料區塊（檔案開頭的 `application/ld+json`）裡的 `telephone` 也要一起改。

## 用 GitHub Pages 發佈

1. 到 repo 的 **Settings → Pages**
2. Source 選 **Deploy from a branch**，Branch 選 `main`、資料夾選 `/ (root)`，按 Save
3. 約 1–2 分鐘後網址會是 `https://yslu-prog.github.io/1page_fam.business/`

之後要改網站，直接在 GitHub 網頁上點 `index.html` → 鉛筆圖示編輯 → Commit，幾分鐘後網站就會更新。

## 使用自己的網域（建議）

買了網域（例如 rongtai-oil.com.tw）後：
1. Settings → Pages → Custom domain 填入網域
2. 在網域商設定 DNS（GitHub 會顯示要填的值）
3. 把 `index.html`、`robots.txt`、`sitemap.xml` 裡的 `yslu-prog.github.io/1page_fam.business` 換成新網域

## 上線後

- 到 Google Search Console 提交 `sitemap.xml`
- 建立 Google 商家檔案，網站欄位填這個網址
