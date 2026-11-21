# 異動日誌（Append-Only）

## [2026-11-21] init | 初始化知識庫目錄與索引檔
- 建立 `raw/`、`wiki/`、`index.md`、`log.md` 與維護規範檔。
## [2026-11-21] ingest | 116學年度大學繁星推薦招生簡章總則
- 來源：`raw/116學年度大學繁星推薦招生簡章總則.pdf`
- 新增：
  - `wiki/channels/star.md`
  - `wiki/rules/star_screening.md`
  - `wiki/rules/star_academic_records.md`
  - `wiki/rules/channel_restrictions.md`
- 更新：`index.md`、`log.md`
- 摘要：依據 116 學年度大學繁星推薦簡章總則，完成知識庫初次匯入。建立繁星推薦核心架構、分發比序與第八類篩選機制、在校學業成績計算與上傳規範，以及繁星錄取對申請入學與分發入學之跨管道排他與法定放棄限制。

## [2026-11-21] ingest | 116學年度大學申請入學招生簡章總則
- 來源：`raw/116學年度大學申請入學招生簡章總則.pdf`
- 新增：
  - `wiki/channels/application.md`
  - `wiki/rules/application_screening.md`
  - `wiki/rules/learning_portfolio_second_stage.md`
  - `wiki/rules/unified_distribution.md`
  - `wiki/comparisons/star_vs_application.md`
- 更新：
  - `wiki/rules/channel_restrictions.md`
  - `wiki/channels/star.md`
  - `wiki/rules/star_screening.md`
  - `wiki/rules/star_academic_records.md`
  - `index.md`
  - `log.md`
- 摘要：完成 116 學年度大學申請入學簡章總則匯入。建立申請入學核心架構與關鍵時程（六校系與各校自訂限制、報名與分發時程）；建立第一階段學測/英聽/APCS/術科檢定、倍率篩選及同級分超額比序完整機制；建立學習歷程檔案 A~T 代碼架構、勾選與 PDF 二擇一上傳、多元表現綜整心得要求及第六學期成績專案時程；建立正備取統一分發與志願序登記演算法；更新跨管道排他與放棄時序矩陣，並產出繁星推薦 vs 申請入學跨管道策略對照頁面。


## [2026-11-21] ingest | 115分發簡章、116科技校院四技申請簡章與116大考中心考試簡章
- 來源：
  - `raw/115學年度大學分發入學招生簡章總則.pdf`（依主管機關最新核定基準，附年度時效說明）
  - `raw/116學年度科技校院日間部四年制申請入學聯合招生簡章總則.pdf`
  - `raw/116學年度簡章.pdf`（大考中心高中英聽、學測、分科測驗考試簡章）
- 新增：
  - `wiki/channels/distribution.md`
  - `wiki/channels/tech_application.md`
  - `wiki/rules/entrance_examinations.md`
  - `wiki/rules/distribution_placement.md`
  - `wiki/comparisons/all_channels_overview.md`
- 更新：
  - `wiki/rules/channel_restrictions.md`
  - `wiki/channels/star.md`
  - `wiki/channels/application.md`
  - `wiki/comparisons/star_vs_application.md`
  - `wiki/rules/unified_distribution.md`
  - `index.md`
  - `log.md`
- 摘要：完成高中升大學知識庫全管道擴充，匯入來源累計達 5 篇。新增大學分發入學總則與考分會登記、最低登記標準、採計加權、特種生加分及同分參酌規範；新增高中生跨足技專校院之「科技校院四技申請」管道總則與獨立 6 志願雙軌機制；新增大考中心英聽、學測與分科測驗三大考試時程、15 級分與 60 級分級距公式、學測轉 60 級分機制及 116 試場嚴禁智慧眼鏡等重大防弊新制；全面擴充跨管道排他條款納入四技申請放棄規範與 13 項前置管道排除清單；產出四大主流升學管道全景深度橫向對照表與家長學生評估決策樹。

## [2026-11-21] update | 重新生成互動式 HTML 簡報（修復 LaTeX 符號、更新 116 簡章版本標示與獨立單檔防護）
- 檔案：`wiki/exports/college_admission_guide.html`
- 變更項目：
  1. 修復 LaTeX 符號未渲染問題：第 7 頁表格「學習歷程採計」欄位修正為標準 HTML 文字 `關鍵採計（占比 ≥ 50%）`；第 8 頁學測轉 60 級分說明修正為 `（× 4）`，全檔掃除殘留 LaTeX 數學語法。
  2. 更新分發入學簡章版本標示：第 6 頁與第 12 頁統一更新為「依據已公告之 116 學年度正式簡章」。
  3. 調整放棄時限寫法：第 10 頁避免寫死特定日期，改為「3月中旬（放榜後約 5 日內）」與「6月中旬（放榜後約 4 日內）」，並加註「確切截止時間以當年度甄選會日程表為準」。
  4. 頁尾 Wiki 來源處理：針對單獨外發給家長/學生開啟之情境，將頁尾相對路徑超連結改為純文字知識庫徽章標籤，杜絕 404 死連結，同時完整保留每一頁對應之 Wiki 條目路徑。
  5. 完整保留 RWD 響應式、鍵盤/觸控滑動翻頁、章節目錄 Modal、全螢幕播放、15轉60級分重算公式、同分參酌增額錄取、13項前置排他名單及116智慧眼鏡試場新制。
