MeDevIS（Medical Devices Information System，醫療器械資訊系統）是由世界衛生組織（WHO）於 2024 年 7 月正式推出的全球首個開放獲取、標準化醫療器械資訊平台。該系統旨在解決全球醫療器械數據零散、命名混亂的問題，為各國政府、衛生主管機關、醫療機構與採購決策者提供一個一站式的國際參考庫。以下為您帶來關於 MeDevIS 系統的全面且深度的教學，涵蓋其背景、架構、技術核心、運作機制、全球影響及對未來醫療產業的變革。 [1, 2, 3] 
------------------------------
## WHO MeDevIS 全球醫療器械資訊系統深度教學## 1. 導論與核心定義## 1.1 什麼是 MeDevIS？
MeDevIS 的全稱為 Medical Devices Information System（醫療器械資訊系統）。它是世界衛生組織（WHO）基於全球公共衛生需求，建立的第一個全球性、開源且標準化的醫療器械線上清算中心與數據庫。 [1, 4] 
在 MeDevIS 問世之前，全球市場上存在著超過 10,000 種不同類型的醫療器械，從最簡單的數位體溫計、一次性注射器，到高度複雜的放射治療設備與臨床實驗室診斷系統。然而，這些器械的技術規格、名稱定義、使用風險及基礎設施需求等資訊，長期散落在各國監管機構、國際組織和跨國製造商的私有數據庫中。MeDevIS 的核心使命，就是將這些破碎的資訊集中化、標準化與數位化，打造一個供全球免費查詢的「醫療器械一站式資訊平台」。 [3, 4] 
## 1.2 發展沿革與重要時間節點
MeDevIS 的誕生並非一蹴而就，而是經過了十多年的國際公共衛生政策鋪墊：

* 2007 年（WHA60.29 決議）： 世界衛生大會（WHA）通過決議，強調醫療技術在全球衛生覆蓋中的關鍵地位，並首次提出建立全球醫療器械數據庫的構想。
* 2015 年 - 2021 年（優先醫療器械清單的累積）： WHO 先後發布了多項針對特定健康領域的「優先醫療器械清單（MDL）」，包括生殖與婦幼健康（2015）、癌症管理（2017）、COVID-19 應對（2020）以及心血管疾病與糖尿病（2021）。這些清單成為了 MeDevIS 的核心數據基礎。
* 2022 年（WHA75(25) 決議）： 世界衛生大會再度授權 WHO，要求其整合現有的醫療器械術語、編碼和定義，正式啟動線上數據庫與清算中心的建置。
* 2024 年 3 月（內部試運行）： MeDevIS 平台上線並開放給 WHO 成員國進行內部諮詢與數據校正。
* 2024 年 7 月 8 日（正式全球發布）： WHO 召開全球網路研討會，正式向公眾全面開放 MeDevIS 平台，標誌著全球醫療器械資訊進入標準化時代。 [4, 5, 6, 7, 8, 9] 

------------------------------
## 2. MeDevIS 的建立背景與公共衛生痛點
為了深入理解 MeDevIS 的重要性，必須先了解全球醫療器械市場長期面臨的嚴峻痛點。

【傳統醫療採購與監管的痛點】
 ├── 資訊孤島化 ── 數據散落在不同國家與製造商，缺乏統一查詢管道
 ├── 命名混亂化 ── 同一種器械在不同國家有數種完全不同的稱呼
 └── 資源錯配化 ── 發展中國家因缺乏技術指南，採購到無法匹配基礎設施的設備

## 2.1 數據零散與「資訊孤島」
全球醫療技術發展迅猛，但資訊卻極不對稱。發達國家（如美國 FDA、歐盟 EMA）擁有完善的醫療器械登記系統，而許多中低收入國家（LMICs）則缺乏相應的資源來建立本國的數據庫。這導致這些國家的政策制定者在進行醫療採購或制定報銷政策時，很難找到客觀、權威且不帶商業利益偏見的技術指南。 [3, 4, 10] 
## 2.2 術語混亂（Nomenclature Chaos）
在 MeDevIS 推出之前，全球缺乏一個一統天下的醫療器械命名體系。同一個「脈搏血氧儀」或「內視鏡手術刀」，在歐洲、美國、日本或亞太地區可能採用截然不同的編碼與名稱。這種「同物不同名」或「同名不同物」的混亂局面，給跨國監管審批、海關進出口追蹤以及全球供應鏈管理帶來了巨大的行政成本與安全隱患。 [3, 11, 12] 
## 2.3 基礎設施與設備的「資源錯配」
許多國際援助機構或發展中國家政府在採購高階醫療設備（如 CT 掃描儀、放射治療機）時，往往忽略了設備運作所需的「隱形成本」——例如穩定的電力供應、特定的環境溫度控制、耗材的持續供應以及專業技術人員的配置。這導致大量昂貴的醫療設備被運抵目的地後，因缺乏基礎設施支持而長期閒置，造成公共衛生資金的極大浪費。 [3, 13] 
------------------------------
## 3. MeDevIS 平台的四大核心功能與架構
MeDevIS 目前已收錄了超過 2,301 種特定醫療器械的詳細檔案，並為使用者提供了以下四大核心功能： [2, 12] 

 MeDevIS 四大核心功能
 ├── 1. 多維度高精度檢索（按類型、醫療體系等級、基礎設施需求過濾）
 ├── 2. 國際命名雙體系對照（EMDN 與 GMDN 代碼無縫轉換）
 ├── 3. 醫療體系等級匹配（基於初級、次級、三級醫療提供精準配置建議）
 └── 4. 技術規格與關聯耗材清單（提供一體化的「套裝/模組」採購參考）

## 3.1 功能一：多維度高精度檢索系統
使用者登入 [WHO MeDevIS 官方入口網站](https://medevis.who-healthtechnologies.org/) 後，可以不限於傳統的「關鍵字」搜尋，而是透過以下多種核心維度進行交叉篩選： [3, 14] 

* 器械類型（Device Type）： 例如影像診斷、實驗室分析、手術工具、介入性植入物等。
* 支持的健康領域（Scope of Use）： 例如專門用於生殖健康、癌症治療、傳染病應對或心血管疾病的器械。
* 所需的硬體基礎設施（Required Infrastructure）： 過濾出是否需要持續交流電（Mains Electricity）、中央醫療氣體系統、特定的空調控溫環境或特殊的醫療廢棄物處理管道。 [3, 7, 13, 15, 16] 

## 3.2 功能二：國際命名雙體系對照（EMDN & GMDN）
這是 MeDevIS 最具革命性的技術突破。該平台首次在一個公開數據庫中，將全球兩大主流醫療器械命名系統進行了無縫整合與交叉引用： [12, 17] 

   1. EMDN（European Medical Device Nomenclature，歐洲醫療器械命名系統）： 隨著歐盟醫療器械法規（MDR/IVDR）的強制實施，EMDN 已成為歐洲及多個緊密合作市場的法定的編碼標準。
   2. GMDN（Global Medical Device Nomenclature，全球醫療器械命名系統）： 由 GMDN 機構維護，在全球 70 多個國家的監管機構（包括美國 FDA 等）中被廣泛採用。

MeDevIS 為每種收錄的器械同時標註其 EMDN 代碼與 GMDN 代碼。這意味著，無論一個國家的監管體系傾向於哪一個系統，都可以透過 MeDevIS 實現即時對照，極大地簡化了全球法規合規與採購核查的程序。 [12, 17] 
## 3.3 功能三：醫療體系等級匹配（Level of Healthcare System Support）
MeDevIS 會明確指出每一種醫療器械適合部署在何種層級的醫療機構中： [3] 

* 初級醫療（Primary Care）： 社區診所、衛生所。適合配置如電子體溫計、可攜式脈搏血氧儀、基本急救包等低風險、易操作的器械。
* 次級醫療（Secondary Care）： 地區性綜合醫院。適合配置如基礎 X 光機、中階血液分析儀、常規手術器械。
* 三級醫療（Tertiary Care）： 大型教學醫院、國家級醫學中心。適合配置如 MRI（核磁共振）、線性加速器（放射治療）、高階心導管手術設備。 [3] 

這種分級引導，能有效防止資源錯配，確保稀缺的公共衛生資金用在最合適的地方。
## 3.4 功能四：技術規格與關聯耗材（MeDevPacks）
在 MeDevIS 系統中，醫療器械不再是一個孤立的名稱，而是以「包裝與系統」的概念呈現。MeDevIS 引入了 MeDevPacks 框架，將產品劃分為以下五大範疇： [18] 

* 系統（System）： 包含醫療設備本體、核心軟體及必要配件的完整運作單元。
* 耗材（Consumables）： 單次臨床程序所需的單次使用醫療物品包。
* 套組（Kit）： 為了達成特定臨床目的而包裝在一起的產品集合（例如 WHO 創傷與緊急手術套組，可供 50 名患者使用）。
* 模組（Module）： 一組可互換的醫療產品，共同滿足特定科室或診療環境的功能需求。
* 組合（Set）： 屬於特定臨床研究或特定手術流程的一組專用器械。 [5, 18] 

------------------------------
## 4. MeDevIS 核心架構對比
為了讓您更直觀地理解 MeDevIS 與 WHO 旗下其他著名的公共衛生清單（如 EML 必備藥物清單）以及傳統查詢方式的差異，以下透過表格進行深度對比。
## 4.1 MeDevIS 與 WHO EML、傳統查詢方式的全面對比

| 比較維度 | 傳統紙本/多數據庫查詢 | WHO EML（必備藥物清單） | WHO MeDevIS（本系統） |
|---|---|---|---|
| 創立背景與年份 | 散落在各國監管機構、廠商官網 | 1977 年創立（即將迎來 50 週年） | 2024 年 7 月正式發布 |
| 涵蓋對象 | 各種異質性極高的硬體、耗材 | 化學藥物、生物製品、疫苗 | 從簡單耗材到複雜百萬級設備 |
| 數據量級 | 數據鏈接破碎，難以統計 | 約 500-600 種核心藥物 | 首波即收錄 2,301 種器械類型 |
| 命名/編碼標準 | 各國自行定義，缺乏跨國對照 | ATC 編碼（解剖學治療學化學分類） | 同時整合並對照 EMDN 與 GMDN |
| 基礎設施需求標註 | 無，需自行查閱說明書或諮詢工程師 | 低（多數為儲存溫度與劑型要求） | 明確標註電力、水質、空調、廢棄物需求 |
| 核心公共衛生功能 | 耗時且容易因資訊不對稱導致錯誤採購 | 全球藥物採購與醫保報銷的黃金標準 | 全球醫療技術決策的「一站式導航」 |

------------------------------
## 5. MeDevIS 對全球醫療生態圈的深遠影響
MeDevIS 的推出，絕不僅僅是多了一個網頁數據庫，它正在深刻改變全球醫療產業的四大核心生態圈。

【MeDevIS 對全球生態圈的連鎖反應】
 ├── 對國家政策制定者 ── 提供本國採購清單與全民健康保險（UHC）報銷的科學依據
 ├── 對醫院採購與工程師 ── 提前規劃基礎設施，降低設備因「水土不服」而閒置的風險
 ├── 對跨國法規監管機構 ── 推動各國法規互認，縮短救命設備上市的審批週期
 └── 對醫療器械製造商 ── 建立統一的研發合規標準，降低進入新興市場的合規門檻

## 5.1 對國家政策制定者與全民健康保險（UHC）的系統性支持
許多國家在推進**全民健康覆蓋（Universal Health Coverage, UHC）**時，面臨最大的難題就是「醫療保險到底該報銷哪些醫療器械？」。 [8] 

* 制定國家採購清單（National Procurement Lists）： 各國衛生部可直接參考 MeDevIS 的結構，結合本國的疾病負擔（如癌症、心血管疾病盛行率），篩選出最迫切需要的基本醫療器械清單。
* 優化醫保報銷決策（Health Insurance & Reimbursement Policies）： 醫保決策機構可以利用 MeDevIS 的客觀分類與定價基準參考，剔除那些昂貴但臨床效益不高的商業噱頭產品，確保醫保基金每一分錢都花在刀口上。 [8, 17] 

## 5.2 對醫院管理層與臨床工程師的運維優化
在微觀的醫療機構運作中，MeDevIS 成為了資產管理與臨床工程（Clinical Engineering）的有力工具。

* 全生命週期管理（Life-cycle Management）： 從採購前的評估、基礎設施對接、到後續的維護與校準，MeDevIS 提供的技術指標為臨床工程師提供了標準的查核清單（Checklist）。
* 降低整體擁有成本（Total Cost of Ownership, TCO）： 通過 MeDevPacks 系統，採購人員能提前將未來的耗材費用、維護配件納入預算，避免「買得起設備，用不起耗材」的財政陷阱。 [13, 15, 16, 18] 

## 5.3 對法規監管（Regulatory Science）與全球互認的催化作用
醫療器械法規的地域性極強。一個在美國核准的產品，要進入亞洲或拉美市場，往往需要重新翻譯、重新編碼、重新走一遍冗長的流程。

* 打破代碼壁壘： MeDevIS 透過同時鏈接 EMDN 與 GMDN，扮演了法規翻譯官的角色。這有助於各國監管機構（如台灣 TFDA、歐盟主管機關等）在審查技術文件時進行跨國數據互認。
* 上市後不良事件監測（Post-market Surveillance & Vigilance）： 當全球某一款器械發生集體安全瑕疵時，標準化的代碼能讓各國衛生部在幾秒鐘內鎖定國內現有的同類庫存，啟動精準召回，保障患者安全。 [17, 19, 20] 

------------------------------
## 6. 從 MeDevIS 看醫療器械分類與法規實務（以亞太地區為例）
為了讓本篇教學更具實戰與應用價值，我們結合 MeDevIS 的分類邏輯，來探討實際在亞太市場（如台灣與香港）進行醫療器械法規合規與品名撰寫時的關鍵實務。
## 6.1 醫療器械的基本分類邏輯（Risk-Based Classification）
MeDevIS 中的器械，在各國監管實務中都會依照「對人體產生的風險高低」進行分級。無論是通用醫療器械（General Medical Devices）還是體外診斷醫療器械（IVD），基本都遵循四級分類法： [21] 

【醫療器械風險分級與實例】
 ├── Class A / Class I   (極低風險) ── 繃帶、手術口罩、壓舌板、數位體溫計
 ├── Class B / Class II  (低至中風險) ── 導尿管、一次性注射器、血壓計、一般內視鏡
 ├── Class C / Class III (中至高風險) ── 血糖計、複雜生化分析儀、血液透析管路
 └── Class D / Class IV  (極高/植入風險) ── 心臟節律器、人工關節、冠狀動脈支架

## 6.2 實務案例：醫療器械品名撰寫與合規要點
當企業欲將一款產品登記並對接如 MeDevIS 的系統時，產品名稱與技術文件的撰寫必須遵循極其嚴格的科學性與獨特性原則（參考 [台灣食藥署 TFDA 規範](https://www.fda.gov.tw/) 與國際 MDR 標準）： [19, 20] 

   1. 嚴禁直接使用模糊的通用名稱： 不能僅用「醫療內視鏡」作為註冊品名，因為這會與市場上無數其他廠牌混淆。 [19] 
   2. 標準結構公式： 建議採用 [製造廠名稱/商標] + [特定核心功能/適用部位] + [器械通用名稱] + (型號/規格)。
   * 正確範例： 「安妥（Anto）胃鏡用切片手術鉗（型號：AT-200）」 [19] 
   3. 多型號合併申報原則： 若產品的分類類別、主品名、製造廠及預期用途完全相同，僅有尺寸、長度或直徑等規格差異（例如不同長度的導尿管），可在同一個註冊案中合併申報，登記在同一張許可證上，這與 MeDevIS 的系統管理邏輯高度契合。 [19] 

------------------------------
## 7. 同名辨析：WHO MeDevIS 系統 vs 商業醫療科技公司 Medivis
在學習醫療器械與數字醫療過程中，常有初學者將 WHO 的官方數據庫 MeDevIS 與美國一家名為 Medivis 的頂尖醫療科技公司混淆。兩者雖然名稱極其相似，但在性質、定位與應用上有著本質的不同。 [22, 23] 
## 7.1 商業醫療科技公司 Medivis 簡介
[Medivis 公司](https://www.medivis.com/) 是一家總部位於美國紐約的先鋒數字醫療企業，專注於利用**擴增實境（AR）、人工智慧（AI）與電腦視覺（Computer Vision）**來變革現代外科手術的視覺化流程。 [22, 23] 
其核心旗艦產品 SurgicalAR 已獲得美國 FDA 的上市許可。該技術能將患者的 CT（電腦斷層）或 MRI（核磁共振）等二維醫學影像數據，透過高精度演算法即時轉化為全息 3D 數位孿生體（Holographic Digital Twin）。醫生在手術室內佩戴 Microsoft HoloLens 2 智慧眼鏡，即可直接「透視」患者的身體結構（如頭顱內的神經、動脈、靜脈、骨骼及腫瘤位置），實現亞毫米級（Sub-millimeter）的精準定位與導航，大幅提升了神經外科、耳鼻喉科（ENT）與骨科手術的安全與效率。 [23, 24] 
## 7.2 MeDevIS 與 Medivis 的本質差異對照表

| 特性/維度 | WHO MeDevIS（醫療器械資訊系統） | Medivis（美國醫療科技公司） |
|---|---|---|
| 主體性質 | 聯合國世界衛生組織（WHO）官方公共衛生平台 | 私營商業高科技公司、獨角獸企業 |
| 核心技術/產品 | 標準化關係型數據庫、Web 搜尋與清算引擎 | SurgicalAR 軟體系統、AI 影像渲染、AR 硬體整合 |
| 主要功能 | 提供全球醫療器械的代碼、規格、基礎設施對照 | 手術室內 3D 醫學影像全息投影與實時手術導航 |
| 收費模式 | 全球免費、開放獲取（Open Access） | 商業軟體授權、企業級 PACS 系統集成收費 |
| 主要用戶 | 各國政府、政策制定者、醫院採購主管 | 外科醫生、手術室團隊、醫學院教授與學生 |

------------------------------
## 8. 總結與未來展望## 8.1 邁向動態更新的醫療技術生態系
世界衛生組織（WHO）承諾，MeDevIS 絕非一個靜態的網頁，而是一個持續演進與動態優化的全球公共衛生資產。隨著未來大流行病（Pandemics）的應對需求、緊急醫療救援場景的變更，WHO 將不斷邀請各國政府、學術界、醫療行業協會等利益相關者，持續擴充平台收錄的器械範圍與新興數字醫療技術（如醫療 AI 軟體、遠距醫療終端等）。 [8, 17, 19] 
## 8.2 給公共衛生從業者與企業的行動建議
對於未來的公共衛生決策者與醫療器械企業而言，熟練掌握並運用 MeDevIS 系統，是接軌國際先進標準、優化資源配置、打通全球供應鏈的必修課題。這不僅能縮短救命技術抵達患者床邊的時間，更將為實現全球通用衛生覆蓋（UHC）奠定堅實的數字化技術基石。 [8, 12, 17] 
------------------------------
## 9. 延伸閱讀與參考資源
為了進一步深入研究，建議您造訪以下權威官方鏈接，以獲取最即時、最權威的行業規範與技術指南：

* WHO 官方平台： WHO MeDevIS 醫療器械資訊系統入口網站 —— 全球醫療器械代碼與技術規格的權威免費查詢終端。
* WHO 官方新聞公告： [世界衛生組織關於 MeDevIS 平台發布的正式新聞稿](https://www.who.int/news/item/08-07-2024-medevis-platform-announced-to-boost-access-to-medical-technologies-and-devices) —— 深入了解該平台建立的政治與公共衛生背景。
* 法規主管機關參考： 台灣衛生福利部食品藥物管理署 (TFDA) —— 了解在地醫療器械分類法規、QSD/GMP 品質系統文件申報以及醫療器械單一識別碼 (UDI) 的實務推動進程。 [9, 14, 19, 20] 

------------------------------
如果您希望針對特定的醫療器械或法規深入探討，請隨時告訴我：

* 您是否有特定類型的醫療器械（例如：體外診斷 IVD、高階影像、植入物）需要查詢其 EMDN/GMDN 代碼？
* 您是否需要進一步了解某個國家（例如：台灣 TFDA、歐盟 MDR）的醫療器械查驗登記與上市前審查流程？
* 您是否需要為特定醫療設備（例如：移動式 X 光機、超音波分析儀）編寫符合國際標準的技術規格查核清單（Technical Specification Checklist）？ [13, 17, 20, 21, 25] 

我將根據您的具體需求，為您提供最精準的實務合規指引！

[1] [https://www.who.int](https://www.who.int/news/item/08-07-2024-medevis-platform-announced-to-boost-access-to-medical-technologies-and-devices)
[2] [https://24x7mag.com](https://24x7mag.com/news/regulations-and-standards/who-introduces-medevis-platform-for-medical-device-information/)
[3] [https://www.linkedin.com](https://www.linkedin.com/pulse/who-launches-medevis-global-medical-device-information-qcqne)
[4] [https://healthpolicy-watch.news](https://healthpolicy-watch.news/who-launches-platform-for-standardised-medical-device-information/)
[5] [https://medevis.who-healthtechnologies.org](https://medevis.who-healthtechnologies.org/about)
[6] [https://onesight.essilorluxottica.com](https://onesight.essilorluxottica.com/research/medevis-who-list-of-priority-medical-devices-eye-care/)
[7] [https://medevis.who-healthtechnologies.org](https://medevis.who-healthtechnologies.org/about)
[8] [https://trpma.org.tw](https://trpma.org.tw/eng/news/news_6083)
[9] [https://www.who.int](https://www.who.int/news/item/08-07-2024-medevis-platform-announced-to-boost-access-to-medical-technologies-and-devices)
[10] [https://mexicobusiness.news](https://mexicobusiness.news/health/news/who-launches-medevis-global-medical-device-information?tag=medevis)
[11] [https://www.medicaldevice-developments.com](https://www.medicaldevice-developments.com/news/who-introduces-medevis-platform-to-enhance-access-to-medical-devices/)
[12] [https://24x7mag.com](https://24x7mag.com/news/regulations-and-standards/who-introduces-medevis-platform-for-medical-device-information/)
[13] [https://medevis.who-healthtechnologies.org](https://medevis.who-healthtechnologies.org/devices/COM_248)
[14] https://who-healthtechnologies.org
[15] https://medevis.who-healthtechnologies.org
[16] [https://www.researchgate.net](https://www.researchgate.net/publication/337055217_Brief_Talking_about_the_Development_of_Medical_Device_Industry_in_China)
[17] [https://finance.yahoo.com](https://finance.yahoo.com/news/launches-medevis-platform-enhance-global-085228027.html)
[18] [https://medevis.who-healthtechnologies.org](https://medevis.who-healthtechnologies.org/medevpacks)
[19] [https://www.fda.gov.tw](https://www.fda.gov.tw/ENG/siteListContent.aspx?sid=10334&id=41175)
[20] [https://www.easychinapprov.com](https://www.easychinapprov.com/registration-in-taiwan)
[21] [https://www.mdd.gov.hk](https://www.mdd.gov.hk/filemanager/common/information-publication/what_is_medical_device-e.pdf)
[22] https://www.medivis.com
[23] [https://www.youtube.com](https://www.youtube.com/watch?v=qiyPBiLaDkU&t=6)
[24] [https://www.youtube.com](https://www.youtube.com/watch?v=bkzkelf7IpI&t=1)
[25] [https://www.easychinapprov.com](https://www.easychinapprov.com/chinese-device-description)
