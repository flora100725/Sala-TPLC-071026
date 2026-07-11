Hi please help me create a technical specification for FDA officer using the template report based on the following info in Traitional Chinese in markdown in 4000 to 5000 words. Please include 6 comprehensive use cases for medical device post market management in the report. Ending with 20 comprehensive follow up questions. Report template: [1]醫療器材來源流向追蹤預警系統規格書

1-1 前言 應用AI技術強化醫療器材上市後管理，參考美國FDA HALO/ELSA 4.0、SwissMedic、HSA等應用案例

1-2 現況(盤點現有資訊/資料集) SQL結構化資料 醫療器材許可證資料庫 醫療器材單一識別系統資料庫 醫療器材分類分級資料庫 醫療器材來源流向申報資料

NonSQL非結構化資料 醫療器材安全警訊 醫療器材回收資訊

其他(非食品藥物管理署資料\網路資源) fda recall database fda Swiissmedic adr/safety alerts TGA Safety Alerts HealthCanada Field Correction Notice

1-3 使用情境(應用於醫療器材上市後管理) 3 use cases

1-4 系統架構Architecture

1-5 使用需求 SRS

1-6 特殊需求 Info: TUDID 醫療器材智慧化跨國監管與預警系統 (TUDID Regulatory Guard OS)
系統架構技術規格說明書暨 FDA 執法官員操作指南
導言：全球醫療器材合規與監管之數位革命
在現代全球醫療器材供應鏈中，高風險醫療器材（如 IMDRF 定義之 Class III 植入式心律器、人工關節及生命維持設備）的售後市場監督（Post-Market Surveillance, PMS）面臨前所未有的挑戰。跨國製造商、進口代理商、地方分銷商與醫療機構之間，數據格式高度異質化、申報欄位缺失、全球法規代碼不一致（如 GMDN、UMDNS、WHO MeDevIS、TFDA 與 FDA UDI 規格衝突），且缺乏即時、可防禦性（Defensible）的 AI 輔導與多模型對照推論機制。
本系統 "TUDID 醫療器材智慧化跨國監管與預警系統 (TUDID Regulatory Guard OS)" 為專門應對上述痛點而設計之高協同性、可驗證、全功能 Agentic OS 智慧化決策平台。系統完全相容於 FDA 21 CFR Part 11 (電子紀錄與電子簽章) 規範及 ISO 14971 醫療器材風險管理 標準，採用極簡優雅的單頁大視圖與多維度標籤控制版面，搭載 Google 領先之 @google/genai 伺服器端推論架構，整合動態 D3 拓撲網狀圖、GIS 地理分布地圖與 Side-by-Side 多模型司法證據級對照稽核引擎，實現醫療器材「數據清洗-格式對齊-流向追蹤-風險預警-臨床替代路徑建議」的全鏈條閉環控制。
第一部分：系統架構與技術規格說明書
code
Code
+----------------------------------------------------------------------------------------+
|                                    TUDID UI LAYER                                      |
|  [Dashboard w/ 6 WOW Graphs]  [Standardizer Tool]  [Skill Manager]  [Playground]       |
+----------------------------------------------------------------------------------------+
                                            |
                                            v (Express REST APIs)
+----------------------------------------------------------------------------------------+
|                 
