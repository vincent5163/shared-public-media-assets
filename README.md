# Shared Public Media Assets

跨專案共用的公開靜態素材庫。僅存放可公開讀取的圖片與文件，不放置程式憑證、環境設定或非公開資料。

## 目錄規則

```text
<project-name>/
└─ <feature-name>/
   └─ assets...
```

目前內容：

- `line-bot-construction-fee/regulation/`：營建工程空氣污染防制法規宣導圖片
- `shelfie-gas/branding/`：管家貓三隻角色原圖與 App 圖示
- `shelfie-gas/onboarding/`：初次引導的視覺（茶會圖、介紹海報）

## 圖片來源

- `line-bot-construction-fee/`：111.09.28 環保署－營建工程設施管理辦法簡報（執行方式說明）
- `shelfie-gas/`：AI 生成，供 shelfie-gas（管家貓）專案使用

## 網頁使用版本

原圖多為 1000px 以上、1–2.5MB，直接引用對行動裝置太重。
需要在網頁中載入時請使用檔名帶尺寸的壓縮版本，例如：

```text
shelfie-gas/onboarding/splash-tea-party.png       原圖 941x1672 2.1MB（保存用）
shelfie-gas/onboarding/splash-tea-party-720.webp  網頁用 720x1279 157KB
```

各專案應使用固定英文檔名；更新既有素材時，如需立即避開 CDN 快取，請同步調整引用網址的版本參數。
