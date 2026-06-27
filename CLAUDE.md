# CLAUDE.md — 接手指南：Pawtient AI × 2026 和泰加速器報名表

> 你（Claude Code）正在協助同事完成 **2026 和泰加速器第二期報名表**，並製作 **提案簡報**。
> **動工前第一件事：讀本資料夾的 `HANDOFF.md`** —— 完整背景、提案策略、公司事實都在裡面。
> 用繁體中文（台灣）跟使用者溝通。

---

## 你的任務（兩個交付物）

1. **完成報名表草稿頁 `index.html`** —— 補齊所有「待填／待確認」欄位。
2. **製作 Q23 的提案簡報** —— 產出一個可分享的連結，填進報名表 Q23。

申請截止：**2026/06/30**。提案主軸：**主題 3「創新產險銷售方案」**（其餘兩主題勾「無」）。

---

## 單一真實來源 & 工作方式

- 本 repo＝`genrevcorp/pawtient-hotai-accelerator`，**所有工作都在這裡**。
- 線上頁（push 後約 1 分鐘自動更新）：<https://genrevcorp.github.io/pawtient-hotai-accelerator/>
- `index.html` 是**自包含的單一檔案**；每一題是一張 `.card`，草稿放在 `data-copy` 屬性裡。
- 本機預覽（**複製鍵需在 localhost 才有效**，別用 `file://`）：
  ```bash
  python3 -m http.server 8000      # 開 http://localhost:8000
  ```
- 更新線上頁：
  ```bash
  git add -A && git commit -m "更新報名表草稿" && git push
  ```

---

## ✅ 一定要做

- 動工前先讀 `HANDOFF.md`。
- 缺的事實（**電話、公司設立日期、城市、Email、募資金額、Q23 簡報連結、如何得知／是否看過廣告**）**一律先問使用者，絕不自行編造**。
- 改完先用 localhost 預覽確認，再 commit / push。
- 撰稿語氣參考既有保險提案網站（見下方「做簡報」），維持自然台灣中文、不要翻譯腔。

## 🚫 絕對不要

- **不要自行送出 Google 表單，也不要勾「同意條款」** —— 那是 Sean 本人要做的。你只做到「草稿備齊、可貼上」為止。
- **不要捏造**任何數字、日期、金額、客戶名稱或公司資訊。不確定就問。
- **不要改掉下方「對保險溝通的紅線」。**

---

## 🛑 對保險公司溝通的紅線（撰稿＋簡報都適用）

1. **只談流程效益**（審核工時、補件往返次數、風險分級），**不談賠付率／損失率／理賠成本**。
2. **AI 輔助、人工核定**：AI 只標示風險點，最終由理賠人員判斷（醫療紅線：我們是記錄整理，不做診斷）。
3. **資料不落地**：飼主授權、自附健康摘要，不需與保險系統整合。
4. **每筆資料標來源**（獸醫原始／飼主輸入／裝置偵測）；Pawtient Watch 寫「難以事後捏造」，**不要**寫「無法偽造」。
5. **效益＝待驗證假設**；客戶案例是「**代表性情境**」，不是已簽約客戶。
6. **醫療免責**：AI 內容僅供整理參考，不構成醫療診斷、不取代獸醫師。

---

## 公司關鍵事實（已用於填表，請勿重新猜測；細節見 HANDOFF.md §6）

- 公司登記名稱：**通用創新有限公司**（General Innovation Co., Ltd.；品牌 GenRev / generalrev.com）
- 負責人／創辦人：**林緯軒（Sean Lin）**；全職人數：**1**（＋ 委外：Android／後端／資安／美術／翻譯）
- 政府計畫：**新竹縣 114 年度 地方型 SBIR**，合約 **G114HS15**，補助款 NT$950,000，期間 2025/09–2026/06
- 產品：iOS 2025/12、Android 2026/02 上架，**約 1,000 名使用者**；64 種血檢參數、21 種健康紀錄型態、9 種語言
- AI 指標：血檢辨識 95.2%、語音轉錄 91.2%、AI 諮詢滿意度 82.6%
- 市場：台灣寵物市場約 631 億元；10 歲以上貓 40%、15 歲以上 80% 受 CKD 影響
- 產品線：Pawtient AI（主 App）＋ Pawtient Watch（舊手機變 AI 寵物攝影機；**下一步將開發專用硬體寵物攝影機**）

---

## 還沒填、要跟使用者要的欄位

Q3 Email（換成保險提案用信箱）、Q4 電話、Q7 設立日期、Q9 官網確認、Q11 城市、**Q23 簡報連結（必填，最重要）**、Q24–28 募資金額、Q31 如何得知、Q33 是否看過廣告、最後同意條款（Sean 勾）。

> 建議開場：先掃一遍 `index.html` 的紅標欄位，列清單問使用者要齊，再動手填。

---

## 🖼️ 做簡報（Q23）

1. 內容直接用 `index.html` 裡 **Q23 展開的「8 段式建議內容」**（解決方案／應用情境／對應主題／≥1.5 個月規劃／所需資源／實績／團隊／成就）。
2. **素材與語氣**：clone `genrevcorp/pawtient-insurance-pitch-site`（裡面有定位文案、App 實機截圖、市場數據 —— 做簡報的主要素材庫）。
3. 形式二選一：
   - **Google Slides**（最好分享）→ 設「知道連結的人可檢視」→ 連結貼 Q23。
   - **HTML 簡報**（參考 `genrevcorp/irl-api-deck` 的做法）→ 上 GitHub Pages → 連結貼 Q23。
4. 全程遵守上方「保險溝通的紅線」。

---

## 需要更深背景時可 clone（唯讀、免 build）

- `genrevcorp/pawtient-insurance-pitch-site` — 簡報素材庫（最常用）
- `genrevcorp/PawtientAI` — App 主 repo（`docs/insurance-demo/`、`docs/marketing/` 有完整合作示範與行銷素材）
- `genrevcorp/PawtientWatch` — Pawtient Watch 產品細節
- 註：SBIR 原始文件只在 Sean 本機、不在 GitHub；填表要用的事實已整理在 `HANDOFF.md`。

---

## 完成後

把 `index.html` 每題確認好的答案，貼進 Google 表單：
<https://docs.google.com/forms/d/e/1FAIpQLSfuQXLhH8iXhLBny40Rpzr63qU6eQlhRpJ5D0oK1VIngu6SzQ/viewform>
**送出與勾「同意條款」交給 Sean 本人完成。**
