# 核心檢核表

整理基準：2026-11-26。每項的「查法」為本 Skill 的執行方式；官方規範的效力以對應原文及適用條件為準

## T：搜尋資格與可理解性

| 編號 | 檢查與取證 | 依據層級與判定界線 |
|---|---|---|
| T01 | 目標需公開收錄時，查可公開存取、robots.txt 與相關存取設定 | 技術要求；一般客戶端成功存取與 Googlebot 存取分別取證 |
| T02 | 讀取最終網址與 HTTP 狀態，確認目標內容正常 | 技術要求；HTTP 200 為資格條件之一 |
| T03 | 查可索引主內容，以及 meta robots／X-Robots-Tag 等索引控制 | 技術要求；先確認使用者是否希望該頁出現在搜尋 |
| T04 | 依 URL Inspection／Search Console 確認實際索引狀態與資料日期 | 證據確認；資格條件與實際收錄分別記錄 |
| T05 | 查標題、主標題、替代文字及連結文字能否準確表達內容 | 最佳實務；依讀者實際用語判斷 |
| T06 | 讀取站內相關連結，確認能找到目標頁與延伸內容 | 最佳實務；按已授權範圍取證 |

T01–T04 依 [Google 搜尋技術要求](https://developers.google.com/search/docs/essentials/technical)；T05–T06 依 [Search Essentials：主要最佳實務](https://developers.google.com/search/docs/essentials#key-best-practices)。索引控制細節依 [robots meta 與 X-Robots-Tag](https://developers.google.com/search/docs/crawling-indexing/robots-meta-tag)

## C：內容品質與可信度

| 編號 | 檢查與取證 | 適用方式 |
|---|---|---|
| C01 | 指出目標讀者的任務，核對全文能否完成任務 | 品質建議；依資訊、交易、比較、工具等頁面用途判斷 |
| C02 | 找出原創資訊、實作、研究或分析及其證據 | 品質建議；工具、圖片、影片與互動功能也可構成主內容 |
| C03 | 查主張的資料、來源、條件及可驗證事實 | 品質建議；按主張的重要性回查一手證據 |
| C04 | 核對作者／網站背景、相關經驗與專業的真實支持 | 品質建議；E-E-A-T 各面向依用途選擇證據，以可信度為核心 |
| C05 | 重大健康、財務、安全主張核對專業依據與適用條件 | 品質建議；此類 YMYL 主題提高查證深度 |
| C06 | 核對標題與正文一致、內容深度、可讀性與新增價值 | 品質建議；篇幅依完成任務所需決定 |
| C07 | 核對時效資訊與日期變動是否有實質內容更新 | 品質建議；依主題對新鮮度的需求判斷 |

依 [實用、可靠、以讀者為本的內容](https://developers.google.com/search/docs/fundamentals/creating-helpful-content) 的自評、主內容及 E-E-A-T 章節。E-E-A-T 為品質面向，Google 以多種信號辨識；評估人員的回饋用來評估系統品質，實際排名由自動系統處理

## E：網頁體驗

| 編號 | 檢查與取證 | 依據層級 |
|---|---|---|
| E01 | 實際量測 Core Web Vitals，註明網址、日期、資料類型及有效樣本 | 已公開的排名考量；草稿或缺量測資料時待查證 |
| E02 | 查安全連線與手機畫面呈現 | 體驗建議 |
| E03 | 檢視廣告、插頁視窗與主內容辨識，保留實際畫面證據 | 體驗建議 |

依 [Google 網頁體驗指南](https://developers.google.com/search/docs/appearance/page-experience)。Core Web Vitals 與其他體驗建議分別標示；頁面體驗包含多個面向，量測結果的適用範圍依原始資料

## A：AI 搜尋資格與內容表示

使用者要求 AI 搜尋檢核時使用；一般草稿檢查只在目標包含 AI 搜尋時載入此節

| 編號 | 檢查與取證 | 判定界線 |
|---|---|---|
| A01 | 查實際索引與摘要顯示資格，沿用 T 類證據 | 官方資格要求；與實際獲得引用分開記錄 |
| A02 | 查重要資訊的文字表示與可發現的站內連結 | 官方最佳實務 |
| A03 | 有結構化資料時比對畫面內容；商家資料適用時查更新狀態 | 官方最佳實務；資料正確性與特定搜尋功能資格分別驗證 |
| A04 | 要求檢查已出現的 AI 回答時，保存查詢、日期、地區、回答與引用網址 | 表示準確性檢查；讀回來源是否支持相關主張 |
| A05 | 讀取 Search Console 的 Search generative AI 設定及父資源繼承後的實際有效值 | AI 搜尋資格設定；依目標核對 Include／Exclude，缺後台資料時待查證 |
| A06 | 要求評估 AI 曝光時讀取 Generative AI performance report，保留報表、期間、PT 時區、維度與彙整方式 | AI 曝光量測；區分曝光、流量及轉換，缺報表時查曝光量與 A05 設定 |

依 [AI 搜尋功能與網站指南](https://developers.google.com/search/docs/appearance/ai-features) 與 [AI 來源與事實性](https://developers.google.com/search/docs/fundamentals/gen-ai-attribution-factuality)。Google 明列沿用 SEO 基礎；專用 AI 檔案與特殊 schema 並非資格要求。建議的價值須連到可觀察的讀者需求、可理解性或來源證據

A05 依 [Search generative AI control](https://support.google.com/webmasters/answer/16908024)，核對資源及父資源繼承的實際狀態，公開預設值只作背景；設定調整依使用者授權。A06 依 [Generative AI performance report](https://support.google.com/webmasters/answer/16984139)，報表涵蓋 AI Overviews／AI Mode 曝光，Discover 另用對應報表。官方說明下載時可能將介面的 `~`／`-` 轉為 0，分析時保留原介面狀態及缺值意義

## 系統背景的使用方式

需要解釋觀察界線時，讀 [Google 排名系統指南](https://developers.google.com/search/docs/appearance/ranking-systems-guide)：語意理解、原創、連結、評論、新鮮度、去重與垃圾偵測等系統作為背景。以實際內容檢查對應品質；內部系統的觸發、權重與分數列為外部觀察範圍以外

[Ranking Hub 原則](https://developers.google.com/search/docs/ranking/principles-for-ranking-results) 說明共同的實用性標準；各搜尋功能的結果與來源選擇須依其實際行為取證
