<div align="right">

[English](README.md) ｜ **繁體中文**

</div>

# 🔍 Competitor Sprint｜一鍵競品情報衝刺

> 輸入一個對手，**5 個 AI 角色分工**，2 分鐘產出含**功能矩陣 + SWOT + 市場缺口 + 戰略建議**的完整競品報告（**報告語言跟隨你，預設繁體中文**）。
>
> 專為 **新創 / PM / 接案行銷** 打造 —— 不用年費 3 萬的 SaaS、不用自架 Python 系統，貼上指令就能跑。

![status](https://img.shields.io/badge/Claude_Code-Skill-blue) ![lang](https://img.shields.io/badge/繁中%20%2F%20EN-✓-green) ![license](https://img.shields.io/badge/License-MIT-yellow)

---

## 安裝（Claude Code）

```
/plugin marketplace add av8d-levelup/competitor-sprint
/plugin install competitor-sprint@competitor-sprint
```

## 用法

裝好後有兩種叫用方式：

**① 直接跟 Claude 說（推薦，會自動觸發）**
```
幫我跑競品 Notion，對手放 Coda、Obsidian、Craft
分析競品 AI 筆記工具，我方是「我的筆記 App」
```

**② 用指令**（外掛技能的完整名稱是 `competitor-sprint:competitor-sprint`）
```
/competitor-sprint:competitor-sprint Notion 競品 --competitors "Coda, Obsidian, Craft"
/competitor-sprint:competitor-sprint SaaS 專案管理 --competitors "Asana, monday, ClickUp" --招聘信號
```

| 旗標 | 作用 |
|---|---|
| `--competitors "A, B, C"` | 指定競品名單（不給就自動發現 4–6 家）|
| `--我方 "你的產品"` | 把你的產品也放進功能矩陣做對照 |
| `--招聘信號` | 選用：多跑一節「招聘信號解讀」，用對手在招什麼人反推它下一步 |
| `--lang en` | 選用：強制用英文輸出報告（預設跟隨你的輸入語言）|

---

## 為什麼跟別的競品工具不一樣

- 🧑‍💼 **5 角色分工**：研究員 → 分析師 → 產品經理 → 戰略顧問 → 評估員，像一支小型情報團隊
- ✅ **品質反思循環**：評估員 6 維度打分，低於 7 分自動補搜重跑
- 🕵️ **招聘信號**（選用）：用 104 / LinkedIn 職缺反推對手的下一步戰略
- 🗂️ **Markdown 增量事實庫**：每家一個 `db/<競品>.md`（YAML 欄位 + changelog），重跑會 diff 舊值、累積時間序列 —— 純文字、可 git 版控、看得到對手這半年改了什麼
- 🌏 **雙語**：報告語言跟隨你的輸入，繁中／English 都行，並對台灣在地來源（PTT/Dcard/104）有第一手優化
- ⏰ **定時監控**：可掛排程每週重跑，有變化就推播

## 範例輸出

見 [`examples/Notion競品/`](examples/Notion競品/)：
- [`report.md`](examples/Notion競品/report.md) — 完整報告（功能矩陣 / SWOT / 市場缺口 / 戰略建議）
- [`_index.md`](examples/Notion競品/_index.md) — 4 家橫向對照總覽
- [`db/`](examples/Notion競品/db/) — 結構化事實庫

> 另有在地生意範例 [`examples/台灣手搖飲品牌/`](examples/台灣手搖飲品牌/)（實體店競品；Google 逐店評價需另接 Places API）。

---

## 適合誰

| ✅ 適合 | ❌ 不適合 |
|---|---|
| 新創早期 / PM 做 PRD、市場分析 | 大企業競品部門（需一手流量/廣告數據）|
| 接案行銷做提案時的競品速寫 | —— 那請用 Crayon / Similarweb |
| 獨立開發者開新產品前掃賽道 | |

**定位**：這是「競品速寫」，不是「情報平台」。資料來自公開網路搜尋，適合沒有情報預算、又需要競品洞察的人。

---

## 想少走彎路？

<div align="center">

會跑競品只是開始 —— 怎麼把 AI 接成「選題 → 生產 → 變現」的完整工作流，我在做給你看。

### AV8D LevelUp｜追蹤我，少走彎路

[![Facebook](https://img.shields.io/badge/Facebook-追蹤AV8D%20LevelUp-1877F2?logo=facebook&logoColor=white)](https://www.facebook.com/AV8D.levelup)

**👉 https://www.facebook.com/AV8D.levelup**

</div>

---

## 授權

MIT © 2026 AV8D LevelUp。工具指令與定價會隨版本更新，使用前以官方文件為準。
