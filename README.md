# RHCSA (EX200) 繁體中文學習指南

本倉庫收錄 Red Hat Certified System Administrator (RHCSA / EX200) 繁體中文學習指南與單頁速記重點（Cram Jam），並於根目錄提供可即時檢索章節與內嵌閱讀的入口網站 (`index.html`)。

🌐 **線上網站（GitHub Pages）**：[https://marker1111014.github.io/harunaadoga-rhcsa-ex200-exam-labs/](https://marker1111014.github.io/harunaadoga-rhcsa-ex200-exam-labs/)
- [完整深度學習指南](https://marker1111014.github.io/harunaadoga-rhcsa-ex200-exam-labs/rhcsa/index.html)
- [單頁速記重點 (Cram Jam)](https://marker1111014.github.io/harunaadoga-rhcsa-ex200-exam-labs/rhcsa/cram.html)

## 倉庫結構

```text
.
├── index.html                  # 入口首頁（章節/指令即時搜尋、站內即時閱讀器、高頻指令複製）
├── rhcsa/
│   ├── index.html              # 完整深度學習指南（14 大章節 + 側邊欄目錄與 Scrollspy）
│   ├── cram.html               # 單頁速記重點 Cram Jam（支援橫向列印）
│   ├── index_standalone.html   # 完整指南單檔離線版（內嵌 CSS / JS）
│   └── cram_standalone.html    # 速記重點單檔離線版（內嵌 CSS）
├── assets/
│   ├── style.css               # 深度指南共用樣式
│   ├── cram.css                # 速記表共用樣式
│   └── scrollspy.js            # 側欄捲動定位腳本
└── .nojekyll                   # 確保靜態資源直接發佈不受 Jekyll 過濾
```

## 網頁存取與部署方式

可透過以下方式在網頁瀏覽或自行部署內容：

1. **GitHub Pages 線上閱讀（已啟用）**：直接由 `main` 分支根目錄 `.` 發佈，開啟 [GitHub Pages 入口首頁](https://marker1111014.github.io/harunaadoga-rhcsa-ex200-exam-labs/) 即可瀏覽。
2. **其他靜態託管平台（Vercel / Cloudflare Pages）**：如需自行鏡像部署，可直接匯入此 GitHub 倉庫，無須額外建置指令（Framework Preset 選 `Other` / Static），Root Directory 保持 `.` 即可發布。
3. **本機靜態伺服器預覽**：
   ```bash
   python3 -m http.server 8080
   ```
   啟動後於瀏覽器開啟 `http://localhost:8080`。
4. **單檔離線開啟**：直接雙擊開啟 `rhcsa/index_standalone.html` 或 `rhcsa/cram_standalone.html` 即可於無網路環境檢視。
