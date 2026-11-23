# 臥推知識庫變更歷史日誌 (Changelog)

本檔案為追加寫入（Append-only）的歷史維護紀錄。每筆紀錄均以一致的前綴開頭，方便使用 `grep "^## \[" log.md` 快速檢索。

---

## [2026-11-23] init | 臥推知識庫初始化
- 確立 Karpathy LLM Wiki 運作模式與三大操作協定（Ingest, Query & Writeback, Lint）。
- 建立雙軌架構（力量舉 [PL] 與 健美肌肥大 [BB] 兼具）。
- 完成專案結構規劃與 `AGENTS.md` 規範檔撰寫。

## [2026-11-23] ingest | 槓鈴臥推怎麼做才不傷肩？動作細節、常見問題完整解析
- **來源**: `raw/01-chichihso-bench-press.md` (肌製所)
- **萃取核心**: 臥推動作解剖（胸大肌、三角肌、三頭長頭雙關節角色）、胸椎伸展 vs 腰椎代償、1.5~2倍肩峰握距、出槓至肩關節上方、手肘 60° 夾角。
- **影響與建立頁面**:
  - 建立 [[technique/setup-and-execution]]
  - 建立 [[biomechanics/muscle-recruitment]]
  - 建立 [[technique/grip-and-wrist]]

## [2026-11-23] ingest | 臥推行程變化與應用指南
- **來源**: `raw/02-lkkwellness-bench-rom.md` (師大運動競技所 王宣仁 / 練健康)
- **萃取核心**: 全程臥推 (Full ROM)、上半程臥推 (Top ROM，三頭肌活化與鎖定段超負荷)、下半程臥推 (Bottom ROM，伸展介導肌肥大與高代謝刺激)、Fischer 2025 肌電研究、退階動作。
- **影響與建立頁面**:
  - 建立 [[variations/range-of-motion]]
  - 建立 [[sticking-points/lockout-and-off-chest]]
  - 更新 [[biomechanics/muscle-recruitment]]

## [2026-11-23] ingest | 臥推肩膀痛是姿勢問題還是不適合妳？先看這3點
- **來源**: `raw/03-herfit-shoulder-pain.md` (HerFIT)
- **萃取核心**: 臥推肩痛三大根本原因（加重太急動作崩塌/旋轉肌疲勞、推拉訓練量失衡缺乏後盾、手肘 90° 外展死角夾擠）、無痛退階路徑（啞鈴、地板推、機械推）。
- **影響與建立頁面**:
  - 建立 [[injury-prehab/shoulder-pain]]
  - 交叉更新 [[technique/setup-and-execution]]
  - 交叉更新 [[biomechanics/muscle-recruitment]]

## [2026-11-23] ingest | 重訓臥推時容易造成手腕傷害的原因以及熱身技巧
- **來源**: `raw/04-fitnessfactory-wrist-pain.md` (健身工廠 / 運動星球)
- **萃取核心**: 8 塊腕骨解剖、腕管與正中神經受壓、過度背屈剪力成因、掌根直立對齊原則、5 分鐘手腕動態熱身 5 步流程。
- **影響與建立頁面**:
  - 建立 [[injury-prehab/wrist-pain]]
  - 交叉更新 [[technique/grip-and-wrist]]

## [2026-11-23] ingest | 漸進式超負荷：完整指南
- **來源**: `raw/05-repcount-progressive-overload.md` (RepCount)
- **萃取核心**: 漸進式超負荷 5 大操作維度（重量、次數、組數、頻率、動作品質與停頓）、RPE/RIR 疲勞控制、加重過急的常見代償陷阱。
- **影響與建立頁面**:
  - 建立 [[programming/progressive-overload]]
  - 交叉更新 [[sticking-points/lockout-and-off-chest]]
  - 交叉更新 [[injury-prehab/shoulder-pain]]

## [2026-11-23] lint | 知識庫全域初次健康巡檢
- 驗證所有 Wikilinks 雙向鏈接有效性。
- 確認無孤島頁面（Orphan Pages），所有頁面均已登錄於 `wiki/00-index.md`。
- 確認雙軌視角 [PL] / [BB] 在各關鍵技術點均有標註。

## [2026-11-23] writeback | 突破臥推 100 公斤大難關專題綜合分析
- **觸發**: 使用者需求產出 100kg 突破專題投影片。
- **產出投影片**: `slides/bench-press-100kg-guide.html`（8頁互動式全螢幕簡報）。
- **知識庫回寫**: 建立 [[syntheses/bench-press-100kg-breakthrough]]，整合力學設定、關節防護、黏滯點突破與 6 週衝刺週期，同步更新 `wiki/00-index.md`。

## [2026-11-23] refactor | 臥推 100KG 簡報風格全面升級為清新活力運動風
- **升級要點**: 改採明亮大卡片與高呼吸感版面、幽默風趣好兄弟教練語氣。
- **擴展規模**: 擴充為 15 頁完整大師班，涵蓋力學設定、手腕防護、8週課表、測驗日熱身金字塔。
- **互動彩蛋**: 內建【臥推卡關互動排查診斷器】與【100KG 熱身金字塔重量速算小工具】。
