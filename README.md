# travel

子家的旅遊筆記合集 — 自由行精選景點、行程模板、實用 tips。

🌐 **Live site:** https://tzchia.github.io/travel/

## 內容

- **台灣東部 9 天 8 夜親子悠遊** (`taiwan-east-family-202610.html`) — 2026/10/3–10/11，蘆洲→花蓮→玉里→池上→台東→旭海→車城→船帆石（2 晚）→高雄→蘆洲；每日實際道路路線圖（OSRM）、景點實景照（`assets/taiwan-east/`）
- **沖繩 5 天 4 夜雙家庭自駕** (`okinawa-family-202607.html`) — 2026/7/23–7/27 行後實錄
- **福岡 6 天 5 夜親子旅遊紀錄** (`fukuoka-family-202606.html`) — 2026/6/9–6/14 親子實際執行版（原訂 6/13 回程，虎航延誤改 6/14）
- **喀比攀岩 8 天逐日紀錄** (`krabi-climbing-202502.html`) — 2025/2/7–2/14

## 結構

```
travel/
├── index.html                       # 首頁導覽
├── taiwan-east-family-202610.html   # 台灣東部親子悠遊
├── okinawa-family-202607.html       # 沖繩雙家庭自駕
├── fukuoka-family-202606.html       # 福岡親子交通計畫
├── krabi-climbing-202502.html       # 喀比攀岩紀錄
├── assets/
│   ├── krabi/                       # CC 授權實景照 + SOURCES.txt
│   └── taiwan-east/                 # CC 授權實景照 + SOURCES.txt
└── README.md
```

## 慣例

- 圖片：只用 Wikimedia Commons 的 CC／公眾領域圖，縮圖後存本站，`SOURCES.txt` 與頁尾列攝影者＋授權；政府觀光網站圖片（林業署、台東觀光網等）多為「版權所有、需事先同意」，不要熱連。
- 地圖：Leaflet + OpenStreetMap 標準圖磚（CARTO 免費圖磚自 2026 起需 API key，已全站改掉）。路線幾何用 OSRM 公用伺服器抓後編碼為 polyline 內嵌。
- 頁內導覽：sticky 進度條＋TOC（手機）／右側 sidedock（≥1100–1280px），scrollspy 高亮，三頁共用同一段程式。

## 新增旅遊指南

1. 複製既有 HTML 當骨架
2. 在 `index.html` 加新卡片
3. `git add -A && git commit -m "..." && git push`
4. 等 GitHub Pages 重建（30-60 秒）
