# Pawtient AI × 2026 和泰加速器（第二期）報名表 — 交接文件 HANDOFF

> 最後更新：2026/06/27。本文件給接手的同事，在自己的電腦上用 Claude Code 接續完成「和泰加速器報名表」與「提案簡報」。

---

## 一、這份工作是什麼

我們要報名 **2026 和泰加速器第二期**（主辦：和泰集團 × StarFab 豪覓顧問）。和泰集團旗下有 **和泰產險**，且有販售**寵物保險**，所以我們用 Pawtient AI 切入徵案的：

> **主題 3：創新商模拓展 → 創新產險銷售方案（Innovative Insurance Sales Solutions）**

其餘兩個主題（主題 1 AI 營運賦能、主題 2 AI 智慧決策）一律勾「無」。

- 報名表（Google 表單）：<https://docs.google.com/forms/d/e/1FAIpQLSfuQXLhH8iXhLBny40Rpzr63qU6eQlhRpJ5D0oK1VIngu6SzQ/viewform>
- 申請截止：**2026/06/30**
- 表單登入帳號：`magnetic.lin@gmail.com`

---

## 二、成果現在放在哪裡（單一真實來源）

所有草稿答案做成一頁「審閱頁」`index.html`，逐題列出中文草稿、建議勾選、以及需要補的欄位。

- **GitHub repo（請以這裡為準）：** `genrevcorp/pawtient-hotai-accelerator`（public）
- **線上頁面（GitHub Pages，noindex）：** <https://genrevcorp.github.io/pawtient-hotai-accelerator/>
- 你在這個 repo 編輯 `index.html` → `git push` → 約 1 分鐘後線上頁面自動更新。

> 註：這頁原本誕生於 Sean 本機的 `PawtientAI/docs/hotai-accelerator/`，但**接手後請一律以 GitHub repo 為單一真實來源**，避免兩邊各改各的版本。

---

## 三、提案策略與不可踩的紅線（撰稿、做簡報都要遵守）

這些是我們對保險公司溝通的原則，請保留、不要改掉：

1. **只談流程效益，不談賠付率**：可講審核工時、補件往返次數、風險分級；**不要**提賠付率／損失率／理賠成本。
2. **AI 輔助、人工核定**：AI 只標示風險點，最終一定由理賠人員判斷（這也是醫療紅線：我們是記錄與整理，不做診斷）。
3. **資料不落地**：由飼主授權、自行附上健康摘要，不需要與保險公司系統整合。
4. **可追溯 > 結構化**：每筆資料標註來源（獸醫原始／飼主輸入／裝置偵測）。
5. **效益是待驗證假設**：審核變快、爭議下降等，都寫成「待和泰一起用實際數據驗證」，不要當成已證實。
6. **用詞**：Pawtient Watch 的被動紀錄寫「難以事後捏造」，不要寫成「無法偽造」。
7. **醫療免責**：AI 內容僅供整理參考，不構成醫療診斷、不取代獸醫師。

---

## 四、目前進度

- **已完成（中文草稿，可直接用）：** 公司簡介、創辦人＋創業動機、亮眼成就、客戶案例（代表性情境寫法）、下一輪資金用途、三個主題勾選，以及 Q23 的「8 段式簡報建議內容」。
- **待補：** 見第五點。

---

## 五、需要 Sean 提供／確認的欄位（頁面上都有紅標）

- **Q3 Email**：換成「保險提案 deck 用的信箱」（目前暫放 `magnetic.lin@gmail.com`）
- **Q4 聯絡人電話**
- **Q7 公司設立／登記日期**
- **Q9 公司官網**（暫放 generalrev.com，請確認）
- **Q11 公司所在城市**（暫放新竹縣，請依公司登記地）
- **Q23 提案簡報下載連結（必填，最重要）**
- **Q24–28 募資相關金額**（草稿假設「未做股權募資、自籌＋SBIR 補助」，金額請填實際）
- **Q31 如何得知計劃**、**Q33 是否看過廣告**
- **最後「同意條款」** 由 Sean 本人於送出前勾選

---

## 六、公司關鍵事實（填表已用，供查對）

- 公司登記名稱：**通用創新有限公司**（General Innovation Co., Ltd.；品牌 GenRev / generalrev.com）
- 負責人／創辦人：**林緯軒（Sean Lin）**，`magnetic.lin@gmail.com`
- 全職人數：**1**（創辦人）＋ 專業委外（Android／後端／資安／美術／翻譯）
- 政府計畫：**新竹縣政府 114 年度 地方型 SBIR**，計畫名「Pawtient AI 毛孩智能照護系統」，合約編號 **G114HS15**，補助款 NT$950,000，執行期間 2025/09–2026/06
- 產品現況：iOS 2025/12 上架、Android 2026/02 上架，**約 1,000 名實際使用者**
- 產品數據：64 種血檢參數、21 種健康紀錄型態、9 種語言；血檢辨識 95.2%、語音轉錄 91.2%、AI 諮詢滿意度 82.6%
- 市場：台灣寵物市場約 631 億元；10 歲以上貓 40%、15 歲以上 80% 受慢性腎臟病影響
- 產品線：Pawtient AI（主 App）＋ Pawtient Watch（把舊手機變成 AI 寵物攝影機；**下一步將開發專用硬體寵物攝影機**）

---

## 七、在你的電腦用 Claude Code 接手（環境設定）

你已裝好 Claude Code，以下假設你用 Sean 的 GitHub 權限（genrevcorp）。

1. 確認 GitHub CLI 已登入、且具 genrevcorp 權限：
   ```bash
   gh auth status
   ```
   若沒有，執行 `gh auth login`（選 GitHub.com、HTTPS），用 Sean 給你的權限登入。

2. Clone 工作 repo：
   ```bash
   gh repo clone genrevcorp/pawtient-hotai-accelerator
   cd pawtient-hotai-accelerator
   ```
   （或 `git clone https://github.com/genrevcorp/pawtient-hotai-accelerator.git`）

3. 在這個資料夾打開 Claude Code，並請它先讀本文件：
   ```bash
   claude
   ```
   進去後可以直接說：「請先讀 HANDOFF.md，我要接續完成和泰加速器報名表」。

4. 本機預覽（**複製按鈕要在 localhost 才能用**，不要用 file:// 直接開）：
   ```bash
   python3 -m http.server 8000
   ```
   瀏覽器開 <http://localhost:8000>

---

## 八、完成報名表的步驟

1. 跟 Sean 收齊第五點的待補資料。
2. 編輯 `index.html`（每一題是一張「card」，內含 `data-copy` 草稿）。可以直接請 Claude Code 改，例如：「把 Q4 電話改成 ___」「把 Q23 連結填成 ___」「Q31 勾 StarFab 官方網站」。
3. `python3 -m http.server 8000` 預覽確認。
4. 推上去讓線上頁同步：
   ```bash
   git add -A && git commit -m "更新報名表草稿" && git push
   ```
   約 1 分鐘後 <https://genrevcorp.github.io/pawtient-hotai-accelerator/> 會更新。
5. 全部確認後，把每題答案貼進 Google 表單；**送出與勾選「同意條款」由 Sean 本人完成**。

---

## 九、製作提案簡報（Q23，必填）

1. 內容直接用頁面 Q23 展開的「8 段式簡報建議內容」（解決方案／應用情境／對應主題／≥1.5 個月規劃／所需資源／實績／團隊／成就）。
2. 素材與語氣可直接沿用既有的保險提案網站：repo `genrevcorp/pawtient-insurance-pitch-site`（線上是同事改版的版本），裡面有定位文案、App 實機截圖、市場數據。
3. 簡報形式二選一：
   - **Google Slides**（最好分享）→ 設「知道連結的人可檢視」→ 連結貼到 Q23。
   - **HTML 簡報**（可參考 `genrevcorp/irl-api-deck` 的做法）→ 上 GitHub Pages → 連結貼到 Q23。
4. 全程遵守第三點的紅線。

---

## 十、延伸參考（需要更深入再 clone）

- `genrevcorp/pawtient-insurance-pitch-site` — 既有保險提案（做簡報的主要素材庫）
- `genrevcorp/PawtientAI` — App 主 repo（`docs/insurance-demo/`、`docs/marketing/` 有更完整的合作示範與行銷素材）
- `genrevcorp/PawtientWatch` — Pawtient Watch 產品細節
- 註：SBIR 計畫的原始文件只在 Sean 本機、不在 GitHub；填表要用到的事實已整理在第六點。
