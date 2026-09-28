<div align="center">

# SparkAi 系統（ChatGPT-SparkAi）

🚀 新一代 { 漸進式 } AIGC 系統 · 一站式 AI B/C 端解決方案，基於 Node.js + NestJS + Vue3 構建，支援獨立私有化部署與商業運營

<a href="../../README.md">简体中文</a> | 繁體中文 | <a href="./README.en.md">English</a>

<p align="center">
  <a href="https://github.com/nosqlnull/ChatGPT-SparkAi/stargazers"><img src="https://img.shields.io/github/stars/nosqlnull/ChatGPT-SparkAi?color=brightgreen" alt="Stars"></a>
  <a href="https://docs.sparkaigc.com/log/"><img src="https://img.shields.io/badge/Version-V6.9.6-brightgreen" alt="Version V6.9.6"></a>
  <a href="https://docs.sparkaigc.com/pro/"><img src="https://img.shields.io/badge/License-Commercial-blue" alt="License Commercial"></a>
</p>

<p align="center">
  <a href="https://docs.sparkaigc.com"><strong>系統文件 · Docs</strong></a>
  &nbsp;•&nbsp;
  <a href="https://test.sparkaigc.com"><strong>演示站 · Live demo</strong></a>
  &nbsp;•&nbsp;
  <a href="https://docs.sparkaigc.com/pro/"><strong>商業授權 · License</strong></a>
  &nbsp;•&nbsp;
  <a href="https://docs.sparkaigc.com/log/"><strong>更新日誌 · Changelog</strong></a>
</p>

<p align="center">
  <a href="#readme-about">專案介紹</a> •
  <a href="#readme-demo">官方演示站</a> •
  <a href="#readme-features">系統核心功能</a> •
  <a href="#readme-compare">版本對比</a> •
  <a href="#readme-preview">介面預覽</a> •
  <a href="#readme-tech">技術架構</a> •
  <a href="#readme-license">商業授權</a>
</p>

</div>

<h2 id="readme-about">📖 專案介紹</h2>

**SparkAi系統是一款支援多語言國際化的{ 漸進式 }AIGC系統，基於OpenAI/ChatGPT、最新旗艦大模型GPT-6、Anthropic Claude（Claude-Opus-5-5 / Claude-Fable-5-1）、Google Gemini、DeepSeek、🎨GPT-Image-2 / GPT-Image-2.5繪畫、🍌Nano-Banana-2第二代繪畫、Midjourney V8、VEO3.1 / Sora-2影片、Seedance2.5影片（即將上線）、Agent智慧體 扣子（Coze）外掛、工作流、函式、知識庫 等AI大模型能力開發的一站式AI系統；支援「🤖AI聊天」、「🎨專業AI繪畫」、「🧠AI智慧體」、「🪟Coze-Agent工作流應用」、「🎬AI影片生成」等，支援獨立私有部署！提供面向個人使用者 (ToC)、開發者 (ToD)、企業 (ToB)的全面解決方案。**

🏅 **截至 2026 年 9 月，SparkAi 已堅持持續開發、更新迭代三年半**，並保持穩定的大版本更新節奏。近期大版本重點支援：

- 🧩 **全模型支援 / 自定義接入最新大模型**：OpenAI、Claude、Gemini、國內主流大模型及三方大模型統一走標準 chat 格式，新模型釋出後即可在後臺自由新增對接，無需系統更新
- 🎨 **多功能 / 多類型大模型繪畫**：文生圖、參考圖生圖、線上編輯繪圖、局部塗抹編輯重繪、圖生文（多模態識圖），覆蓋 GPT-Image-2 / GPT-Image-2.5、Nano Banana 2、Midjourney V7 / V8 等模型
- 🤖 **新一代對話架構**：Chat Completions / Responses 雙端點自動路由，切換會話、關閉頁面不中斷生成
- 📄 **多類型文件理解**：PDF / Word / PPT / Excel 等檔案上傳識別與線上預覽
- 💰 **積分與帳戶安全**：積分明細對帳、模型呼叫失敗零扣費、登入裝置與異地識別

更多內容詳見下方「系統核心功能」與[更新日誌](https://docs.sparkaigc.com/log/)。

<h2 id="readme-demo">🖥️ 官方演示站</h2>

唯一官方演示站點（其他地址均為非官方）：

| 入口 | 地址 |
|---|---|
| 系統使用者端 | <https://test.sparkaigc.com> |
| 管理後端 | <https://test.sparkaigc.com/sparkai/admin> |
| 測試帳號 / 密碼 | `admin` / `123456` |
| SparkAi 系統文件 | <https://docs.sparkaigc.com> |

<h2 id="readme-features">🌟 系統核心功能（授權商業部署版）</h2>

**閱讀說明**

🎉 一站式 AIGC 系統：整合 AI 大模型對話、專業 AI 繪畫、AI 影片生成、AI 智慧體、文件上傳分析、多模態影像理解、TTS & 語音識別對話等能力。

以下按功能模組歸類，並標註對應支援的模型與引入版本（如 `V6.9.6`），各版本完整內容請檢視[更新日誌](https://docs.sparkaigc.com/log/)。具體模型能否使用，取決於所接入上游 API 渠道的支援情況。

### 🔥 近期大版本更新亮點
**V6.9.x 系列重點更新**

- **V6.9.6 大更新**：重構大模型對話架構，支援 OpenAI Chat Completions 與 Responses 雙端點自動路由；新增官方模型多類型文件理解、大模型全域配置中心、對話檔案線上預覽；重構積分明細系統並支援模型呼叫失敗零扣費；新增登入裝置與異地識別系統
- **V6.9.5**：新增對話導航條、對話演示資料、「畫廊精選 / 我的繪畫」分欄載入；重構個人中心 UI；中文字型子集化等效能最佳化，單頁資源下載量降低約 50%
- **V6.9.4**：新增 Nano Banana 2 獨立繪畫模組；重構繪畫模組架構（可複用底座 + 非同步任務編排）；新增強制指定使用者下線、「系統功能測試」開關
- **V6.9.3 大更新**：AI 對話核心重構為上下游解耦的非同步執行模型，SSE 流式鏈路增量持久化；風控敏感詞檢測擴充套件至繪畫與思維導圖；GPT-Image-2 繪畫模組重構
- **V6.9.2**：新增 GPT-Image-2 獨立繪畫模組（文生圖 / 參考圖 / 線上編輯）、網站直播入口
- **V6.9.1**：系統全國際化 + 管理後臺一鍵 AI 國際化、Midjourney V8 支援、登入註冊頁重構
- **V6.9.0**：2026 使用者端 UI 大重構（卡片風格 / Notion 風格雙主題）、AI 對話沉浸模式

### 🤖 一、AI 大模型對話
**對話能力與模型支援**

1. 🔥 **全模型支援**：支援 OpenAI 官方 API + 一切標準 chat 格式中轉 API；覆蓋 OpenAI（GPT-6 / GPT-5.4 / GPT-5.4-pro / o3 / o4-mini / Codex 系列）、Anthropic Claude（Claude-Opus-5-5 / Claude-Fable-5-1 等）、Google Gemini（Gemini-3.1-pro 等）、DeepSeek（deepseek-r1 等）、Azure OpenAI，以及豆包、通義千問、智譜 ChatGLM、Moonshot、訊飛星火、百川、騰訊混元、360 智腦等國內模型；適配 LocalAI / Ollama 本地模型
2. 🎈 **後臺自由自定義接入最新大模型（無需系統更新）**：OpenAI 全模型、Claude 全模型、Gemini 全模型、國內 AI 全模型及三方主流大模型統一走標準 chat（OpenAI）格式，新模型釋出後即可在後臺自由新增對接並立即使用；支援模型自定義分類、名稱、排序、Logo 與廠商分組
3. 🧭 **雙端點智慧路由** `V6.9.6`：按模型能力自動路由 Chat Completions / Responses 端點——命中規則的 OpenAI 官方系列（GPT / o 系列 / Codex）走 Responses 官方通道，Claude / Gemini / DeepSeek 等穩定使用 Chat Completions；內建多級失敗自動降級重試
4. ⚙️ **大模型全域配置中心** `V6.9.6`：統一管理端點路由規則、失敗是否扣費、stream 流式引數等全域策略，支援正則規則與模型名即時測試，儲存即時生效、無需重啟
5. 📄 **多類型文件理解** `V6.9.6`：官方模型支援 PDF / Word / PPT / Excel / 文本 / Markdown / HTML 等檔案上傳識別（非 PDF 檔案建議選擇 GPT 系列模型，經 Responses 端點）；支援 URL 拼接 / Base64 內聯 / 檔案連結三種提交方式，按體積與 Token 上限自動擇優與降級
6. 👀 **對話檔案線上預覽** `V6.9.6`：PDF / Word / PPT / Excel / 文本 / Markdown / HTML 線上檢視、列印、下載，Coze Agent 對話同步支援
7. 🖼️ **多模態影像理解**：單圖 / 多圖上傳（最多 9 張），支援手機原生相機與 PC 攝像頭拍照上傳 `V6.9.3`；使用者訊息多圖自適應排版 `V6.9.6`；API 返回圖片自動預覽
8. 🤔 **深度思考與推理**：支援 o3 / o4-mini、DeepSeek-R1 等推理模型，思維鏈（ReasoningContent / Think 標籤）流式輸出與展示，支援深度搜尋過程顯示
9. 🛜 **聯網搜尋**：支援模型聯網擴充套件搜尋即時內容並總結（如 o4-mini-all：聯網 + 推理 + 影像 + PDF 文件分析）
10. 🛡️ **高可靠對話核心** `V6.9.3`：上游（後端 ↔ 大模型）與下游（前端 ↔ 後端）連線解耦，切換會話、關閉頁面、退出客戶端均不中斷生成；SSE 邊生成邊落庫，切回會話可續顯；「停止回答」即時取消上游請求；首字超時 / 空響應統一兜底；多會話併發隔離
11. 📌 **對話導航條** `V6.9.5`：當前對話組內提問 ≥ 3 條時自動出現，支援摺疊、懸停展開、點選定位
12. Ⓜ️ **強大的內容渲染**：Markdown（程式碼高亮 / LaTeX / KaTeX 公式 / Mermaid / 圖表繪製）、思維導圖生成與 PDF 匯出、程式碼檔案下載、對話重新編輯
13. 🗣️ **語音對話**：支援 OpenAI / Azure 語音識別與 TTS（Whisper & TTS 格式中轉），語音輸入語音回覆、多種音色選擇，後臺可開關語音播放
14. 🏄‍♂️ **外掛系統與開放對接**：內建外掛系統（識圖、文件分析等，持續擴充套件）；相容 chat 介面的知識庫或工作流應用（如 FastGPT 知識庫 / 工作流）可作為模型接入，或繫結到智慧體使用

### 🎨 二、專業 AI 繪畫
**獨立繪畫模組與模型支援**

15. 🖌️ **GPT-Image-2 獨立繪畫模組** `V6.9.2` `V6.9.3`：支援 gpt-image-2、gpt-image-2.5、GPT-Image-2-Dev 等模型，後臺可自定義接入 API 與擴充套件模型版本；文生圖、參考圖繪畫（最多 8 張智慧參考圖）、已生成結果線上編輯與塗抹框選編輯；畫質（low / medium / high / auto）、數量、比例與自定義解析度嚴格按官方引數範圍提交；支援單使用者 / 全系統併發限制
16. 🍌 **Nano Banana 2 獨立繪畫模組** `V6.9.4`：支援 gemini-3.1-flash-image、gemini-3-pro-image，可自定義擴充套件模型版本（如 gemini-3.1-flash-lite-image）；文生圖、多張智慧參考圖編輯、自定義解析度與比例（2K / 4K 輸出取決於模型）；也可在 AI 對話中直接選用 Nano Banana 模型繪圖
17. 🎨 **Midjourney / Niji 全功能**：支援 MJ V7 / V8（V8 待官方 API 正式開放後直接可用）；Imagine / Upscale / Vary / Zoom Out / Pan、Vary Region 局部重繪、影像混合，普通參考圖 / 角色一致（cref）/ 風格一致（sref）參考圖組合使用；Fast / Relax 雙通道獨立計費與併發；繪畫進度即時渲染
18. 🪄 **DALL·E 2 / 3 繪畫**：支援全部引數
19. 🔁 **通用繪畫能力**：「畫同款」一鍵複用引數；各模型、各操作積分價格前端動態顯示；繪畫失敗自動退還積分（冪等退款，杜絕重複返還）`V6.9.6`；異常任務定時補償；原圖 + 縮圖私有化儲存；各繪畫模型前端顯示開關；繪畫進度條
20. 🖼️ **AI 畫廊廣場**：「畫廊精選 / 我的繪畫」分欄載入 `V6.9.5`；作品風格分類、輪播圖、創作者中心；影片作品懸停自動預覽播放
21. 🚥 **繪畫內容風控** `V6.9.3`：GPT-Image / Midjourney / Niji / DALL·E 提示詞提交前即做敏感詞攔截，不呼叫上游、不扣費，違規記錄同步至管理後臺

### 🎬 三、AI 影片生成
**影片模型支援**

22. 📽️ **VEO3 / VEO3.1 影片**：支援 VEO3.1、VEO3.1-fast、VEO3.1-pro 等模型，生成影片自動配套音訊（標準 chat 對話形式呼叫）
23. 📽️ **Sora-2 影片**：支援 Sora-2 影片生成（標準 chat 對話形式呼叫）
24. 🎞️ **Midjourney HD 影片** `V6.8.6`：已生成圖片一鍵生成「動圖（高運動 / 低運動）」，支援自定義動作描述、單次 1 / 2 / 4 條生成，獨立扣費配置
25. 🎬 **獨立 AI 影片模組**：文生影片 / 圖生影片（Pika），影片作品廣場展示
26. 🌱 **Seedance 影片（Coze-Agent）**：通過 Coze-Agent「Seedance 大模型影片生成」應用呼叫字節跳動官方 Seedance 模型，支援首尾幀與帶聲音影片，生成結果在系統內直接預覽播放
27. 🔜 **即將上線**：Seedance2.5 影片、Qwen-Image 圖片編輯、可靈等獨立圖片 / 影片模組（2026 下半年開發計劃）

### 🧠 四、AI 智慧體（Agent）
**智慧體與應用生態**

28. 🤖 **Coze Agent 智慧體模組**：支援扣子（Coze）外掛、工作流、函式、知識庫智慧體對接；即時流式響應，展示思考過程與模型 / 外掛 / 工作流呼叫詳情；單智慧體多開對話；支援多檔案類型上傳，圖片 / 影片結果直接預覽
29. 📥 **智慧體批次管理**：從 Coze 平臺一鍵批次匯入與同步智慧體（Redis 分散式鎖防重複），圖示自動私有化儲存
30. 📈 **智慧體商店**：自研評分、活躍度、熱度演算法；推薦問題、關鍵字搜尋；連結分享、微信掃碼分享、海報分享
31. 🧠 **GPTs 與預設應用**：GPTs 應用全網搜尋一鍵接入；Prompt 自定義預設應用；使用者自建智慧體；應用可繫結模型、分享連結、共享到廣場

### 💰 五、會員積分與商業運營
**計費、支付與增長**

32. 🧑‍🤝‍🧑 **會員積分體系**：普通模型積分、高階模型積分、繪畫積分、Agent 積分多種餘額；按次 / 按時間 / 組合套餐等多種計費方式，每個模型可自定義扣費
33. 🧾 **積分明細系統** `V6.9.6`：使用者端與管理端口徑統一，完整記錄全模型使用的消耗、失敗返還、失敗免扣，時間精確到秒，支援多維度篩選對帳；管理後臺對話列表展示每條回覆的積分消耗
34. 🆓 **模型呼叫失敗零扣費** `V6.9.6`：4xx / 5xx、超時、空回覆可按開關不扣積分；失敗 / 中斷 / 空回覆統一結算出口，杜絕誤扣與重複扣費，並具備防刷保護
35. 🛍️ **支付系統**：微信官方支付（PC 端 Native 掃碼、手機微信內 JSAPI）、易支付、碼支付、虎皮椒支付；訂單狀態同步檢查、訂單搜尋與管理
36. 🛒 **商城與增長工具**：永久 / 限時套餐商城、簽到獎勵、邀請獎勵、卡密兌換（批次生成與管理）、訪客體驗模式
37. ⏏️ **分銷系統**：A + B 分銷模式，可按使用者單獨設定提成；支援提現門檻與支付寶 / 微信 / 銀行卡提現
38. ✨ **渠道負載均衡**：自研渠道均衡負載與分配演算法，API Key 池多 Key 輪詢（優先順序 / 權重 / 狀態管理），支援批次新增與刪除

### 🔐 六、安全與風控
**內容安全與帳戶安全**

39. 🚥 **內容風控**：自定義敏感詞 + 百度內容稽核，覆蓋對話、繪畫、思維導圖，命中即前置攔截；違規檢測記錄與使用者快照全量留痕
40. 📍 **登入裝置與異地識別** `V6.9.6`：記錄登入 IP（解析至運營商與所在城市）、瀏覽器、作業系統與裝置類型；使用者可在個人中心檢視最近 5 次登入裝置與線上狀態，管理端同步展示
41. 🔑 **會話安全**：普通使用者僅允許單裝置線上；超級管理員帳戶按登入 IP 區分會話，異地登入相互強制下線並記錄 IP；支援後臺強制指定使用者下線 `V6.9.4`、封停用戶
42. 🙈 **敏感資訊脫敏**：演示 / 非超管帳戶檢視 IP 與地區、配置值、API 地址、金鑰、使用者名稱、郵箱等資訊時統一脫敏；admin 演示帳戶只讀
43. 📤 **上傳安全**：服務端拒絕指令碼 / 程式碼類執行檔；開啟雲端儲存後禁止匿名寫入本機磁碟，遊客上傳限頻限量
44. 🧪 **「系統功能測試」開關** `V6.9.4`：開啟後所有 AI 生成請求在系統層統一阻斷、不呼叫上游 API，適用於尚未完成生成式人工智慧備案的上線階段
45. 📧 **註冊防護**：郵箱域名白名單、可停用「+」別名郵箱、臨時郵箱過濾；註冊贈送額度防篡改

### 🛠️ 七、管理後臺與站點運營
**後臺管理與運營配置**

46. 📊 **資料儀表盤**：使用者、對話、繪畫、訂單統計與近 7 日趨勢折線圖，模型使用次數與 Token 使用餅圖
47. 💻 **完整管理後臺**：使用者、訂單、對話、繪畫、影片等資料管理，支援 Excel 匯出；百萬級資料量查詢最佳化（統計查詢併發 + Redis 快取）；使用者列表展示登入 IP 記錄 `V6.9.6`
48. 🗂️ **模型與卡池管理**：模型分類、排序、Logo、廠商分組，按廠商預選新一代模型 `V6.9.6`；API 卡池批次新增 / 刪除 Key
49. 🎭 **對話演示資料** `V6.9.5`：可指定任意對話組（最多 5 條）作為全站只讀演示內容
50. ✔️ **站點自定義**：Logo / 站點名稱 / 頁尾 / 百度統計 / 版權資訊 / 備案號 / 公告 / 歡迎語 / 關於我們 / 使用者協議等均可後臺配置；網站直播入口 `V6.9.2`
51. 🧩 **動態選單與輪播圖**：支援內嵌網頁、外鏈、內部路徑跳轉，自定義圖示，PC 與移動端分別配置；廣告位 / 活動 / 教程輪播展示
52. ♻️ **微信公眾號聯動**：公眾號登入、關鍵詞自動回覆
53. 🔐 **許可權系統**：超級管理員與演示帳戶分級許可權

### 🌏 八、多端體驗與系統架構
**體驗、效能與部署**

54. 🌐 **系統全國際化** `V6.9.1`：前端介面 + 後端配置資訊 + 後端返回資訊全量國際化，按訪問 IP 與瀏覽器語言自動切換；管理後臺配置內容一鍵 AI 翻譯，支援出海運營
55. 🎨 **雙風格 UI** `V6.9.0`：卡片風格 / Notion 風格使用者自由切換；AI 對話沉浸模式、「新增選單」收納、液態玻璃按鈕、明暗主題自動適配
56. 📲 **多端支援**：PC 端 + 手機 H5 + 微信公眾號，自適應 PC / 移動端 / 平板；支援 PWA，H5 可打包至其他平臺
57. ⚡ **效能最佳化** `V6.9.5`：中文字型子集化（單個字重 4.2MB → 0.9MB），單頁資源下載量降低約 50%，移動端資源分批載入，降低 iOS 等低記憶體裝置崩潰風險
58. 🚀 **高併發服務端**：Node.js + NestJS 服務端，Redis 快取與 MySQL 連線池自適應，適配高併發業務場景
59. 🗄️ **儲存與資料同步**：本地儲存 / 阿里雲 OSS / 騰訊雲 COS / Chevereto 圖床，使用者檔案與繪畫資料私有化儲存；對話會話隔離、雲端儲存，多裝置資料同步
60. 🖥️ **部署執行**：支援寶塔常規部署與 Docker 一鍵部署，所有對接配置均在後臺介面完成；適用於商業運營、企業內部、教育培訓等多種場景
61. 🏅 **持續更新**：已堅持開發迭代三年半，保持穩定的大版本更新節奏，更多 AI 能力持續開發中……

<h2 id="readme-compare">📊 公益免費商業版 vs 商業授權版</h2>

公益免費商業版（Public Good V2.1.0 · 2026 特別公益重構版，支援會員套餐、線上支付、分銷等商業功能）倉庫：[SparkAi-ChatGPT-AiWeb](https://github.com/nosqlnull/SparkAi-ChatGPT-AiWeb)

| 功能 | 公益免費商業版（Public Good V2.1.0） | 商業授權版（V6.9.6） |
|---|---|---|
| 使用範圍 | ✅ 支援商業運營 | ✅ 支援商業運營 |
| 版本迭代 | 2026 特別公益重構版（功能底座 V3.2.0），部分功能更新 | ✅ 持續大版本更新 |
| AI 大模型 | ✅ GPT-3.5 / GPT-4.0、Azure 及部分國內模型<br>🔜 即將支援 GPT-6、Claude-Opus-5-5 / Claude-Fable-5-1、Gemini、DeepSeek 等全模型（預計 2026.10） | ✅ GPT-6、Claude-Opus-5-5 / Claude-Fable-5-1、Gemini、DeepSeek 等全模型 |
| 後臺自定義接入最新大模型（無需系統更新） | 🔜 即將支援（待更新至 GitHub，預計 2026.10） | ✅ |
| 雙端點智慧路由 / 大模型全域配置中心 | ❌ | ✅ |
| 深度思考推理（o3 / DeepSeek-R1 等） | ❌ | ✅ |
| 多圖識圖 / 多類型文件理解與線上預覽 | ❌ | ✅ |
| DALL·E 繪畫 | ✅ DALL·E 2 / 3 | ✅ DALL·E 2 / 3 |
| Midjourney 繪畫 | ✅ 文生圖、圖生圖、局部重繪 | ✅ 全功能：V7 / V8、Niji、角色 / 風格一致參考圖、HD 影片 |
| GPT-Image-2 / Nano Banana 2 獨立繪畫模組 | ❌ | ✅ |
| AI 影片生成（VEO3.1 / Sora-2 / Pika / Seedance） | ❌ | ✅ |
| AI 智慧體 | ✅ Prompt 自定義預設應用 | ✅ 另支援 Coze Agent、GPTs 應用、智慧體商店 |
| 註冊登入 | ✅ 微信掃碼 / 郵箱 / 手機號 | ✅ 另支援登入裝置與異地識別 |
| 卡密兌換 | ✅ | ✅ |
| 會員套餐 | ✅ 永久 / 限時會員套餐 | ✅ 多種積分餘額，永久 / 限時 / 組合套餐，每個模型自定義扣費 |
| 支付系統 | ✅ 易支付 / 碼支付 / 虎皮椒 | ✅ 微信官方支付 / 易支付 / 碼支付 / 虎皮椒 |
| 分銷推廣 | ✅ 分銷邀請、佣金提現 | ✅ A + B 分銷、按使用者單獨設定提成、提現門檻 |
| 積分明細 / 模型呼叫失敗零扣費 | ❌ | ✅ |
| 增強風控（敏感資訊脫敏、「系統功能測試」開關等） | ❌ | ✅ |
| 系統全國際化 | ❌ | ✅ |
| 2026 新版 UI（卡片 / Notion 雙風格、沉浸模式） | ❌ | ✅ |
| 完整商用管理後臺 | 基礎管理 | ✅ 資料儀表盤、模型與卡池、動態選單、全域配置 |

<h2 id="readme-preview">🖼️ 介面預覽</h2>

> 截圖與 [商業版系統介紹文件（飛書）](https://bx5gkpqv57j.feishu.cn/docx/EOWUdQ04no9PoBxyp6Ecg3AAnhf) 保持一致，非即時最新，實際效果請以 [官方演示站](https://test.sparkaigc.com) 為準。

### 💻 PC 端（部分展示）

#### 使用者註冊登入

支援微信環境靜默登入、瀏覽器中微信主動掃碼登入、郵箱註冊登入、手機號註冊登入。`V6.9.1` 起全新的創意動畫登入介面（原生 CSS + Vue 3 Composition API 從零實現）。

<p align="center">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-login-1.jpg" alt="使用者註冊登入" width="49%">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-login-2.jpg" alt="使用者註冊登入" width="49%">
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-login-3.jpg" alt="使用者註冊登入" width="49%">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-login-4.jpg" alt="使用者註冊登入" width="49%">
</p>

#### 系統多語言國際化

全國際化：不僅是前端固定內容，還支援後端配置資訊與後端返回資訊的國際化。

![系統多語言國際化](https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-i18n.jpg)

#### AI 大模型對話

支援 OpenAI、Gemini、Claude 全模型，以及國內 AI 全模型與三方主流大模型（市面標準 Chat 格式 API 均可對接）。

![AI 大模型對話](https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-chat.jpg)

#### AI 智慧體應用

GPTs 應用 + Prompt 自定義預設應用；GPTs 支援後臺自定義新增，也可全站搜尋（同官方搜尋）。

![AI 智慧體應用](https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-agent.jpg)

#### 使用者自定義建立預設應用智慧體

智慧體應用工作臺，支援連續上下文使用。

<p align="center">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-agent-custom-1.jpg" alt="使用者自定義建立預設應用智慧體" width="49%">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-agent-custom-2.jpg" alt="使用者自定義建立預設應用智慧體" width="49%">
</p>

#### Midjourney 繪畫全功能

支援繪畫進度即時渲染顯示。

<p align="center">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-mj-1.jpg" alt="Midjourney 繪畫全功能" width="49%">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-mj-2.jpg" alt="Midjourney 繪畫全功能" width="49%">
</p>

#### 墊圖生圖

支援普通參考圖、角色一致參考圖、風格一致參考圖，可單獨或組合使用；支援上傳預覽、圖片類型與墊圖序號顯示。

![墊圖生圖](https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-mj-reference.jpg)

#### Vary Region 局部編輯重繪

![Vary Region 局部編輯重繪](https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-mj-vary-region.jpg)

#### 影像混合

![影像混合](https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-mj-blend.jpg)

#### DALL·E 繪畫

![DALL·E 繪畫](https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-dalle.jpg)

#### Midjourney HD 影片

全新的 MJ 高畫質影片創作能力（`V6.8.6` 起）。

![Midjourney HD 影片](https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-mj-video-1.jpg)

<p align="center">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-mj-video-2.jpg" alt="Midjourney HD 影片" width="49%">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-mj-video-3.jpg" alt="Midjourney HD 影片" width="49%">
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-mj-video-4.jpg" alt="Midjourney HD 影片" width="49%">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-mj-video-5.jpg" alt="Midjourney HD 影片" width="49%">
</p>

#### AI 畫廊廣場

包含創作者功能。

![AI 畫廊廣場](https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-gallery-1.jpg)

<p align="center">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-gallery-2.jpg" alt="AI 畫廊廣場" width="49%">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-gallery-3.jpg" alt="AI 畫廊廣場" width="49%">
</p>

#### AI 影片生成 / AI 影片廣場

支援文生影片、圖生影片。

![AI 影片生成 / AI 影片廣場](https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-video.jpg)

#### 使用者會員套餐商城

後臺自定義限時套餐與永久套餐，可隨意組合。

<p align="center">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-shop-1.jpg" alt="使用者會員套餐商城" width="49%">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-shop-2.jpg" alt="使用者會員套餐商城" width="49%">
</p>

#### 分銷推介

<p align="center">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-distribution-1.jpg" alt="分銷推介" width="49%">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-distribution-2.jpg" alt="分銷推介" width="49%">
</p>

### 📱 H5 手機端（部分展示）

<p align="center">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/h5-01.jpg" alt="H5 手機端" width="32%">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/h5-02.jpg" alt="H5 手機端" width="32%">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/h5-03.jpg" alt="H5 手機端" width="32%">
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/h5-04.jpg" alt="H5 手機端" width="32%">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/h5-05.jpg" alt="H5 手機端" width="32%">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/h5-06.jpg" alt="H5 手機端" width="32%">
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/h5-07.jpg" alt="H5 手機端" width="32%">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/h5-08.jpg" alt="H5 手機端" width="32%">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/h5-09.jpg" alt="H5 手機端" width="32%">
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/h5-10.jpg" alt="H5 手機端" width="32%">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/h5-11.jpg" alt="H5 手機端" width="32%">
</p>

更多內容請訪問 [官方演示站](https://test.sparkaigc.com) 體驗。

### 💳 微信官方原生支付

支援官方微信支付、易支付、碼支付、虎皮椒支付等方式，支援同步檢查訂單狀態、訂單搜尋與管理。

開啟官方微信支付後，PC 端呼叫 Native 支付（直接生成二維碼支付）：

![PC 端微信 Native 支付](https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pay-pc-native.jpg)

手機微信環境內呼叫 JSAPI 支付（直接喚起微信錢包支付）：

<p align="center">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pay-h5-jsapi.jpg" alt="手機端微信 JSAPI 支付" width="32%">
</p>

### 🛠️ 系統管理後臺

請訪問 [官方演示站管理後臺](https://test.sparkaigc.com/sparkai/admin) 檢視（測試帳號 `admin` / `123456`）。

<h2 id="readme-tech">🧱 技術架構與部署環境</h2>

### ✨系統技術架構
**系統架構**

- 前端：Vite + Vue3 + TypeScript + NaiveUI + TailwindCSS
- 管理端：Vite4 + Vue3 + Element-Plus
- 服務端（後端）：Node.js + NestJS
- 資料支援：MySQL5.7(+) / MySQL8 + Redis
- 執行環境：Linux、Windows、macOS（推薦使用Linux）
- 資料儲存：本地儲存 | 物件儲存阿里雲OSS | 物件儲存騰訊雲COS | Chevereto圖床

### 🛠️執行環境
**執行環境**

- Linux (推薦)
- Windows
- MacOS Server
- Docker
- Kubernetes
- 支援 ARM64 & X86 (32/64) 架構

### 🎯伺服器配置要求
**最低伺服器配置執行要求 1C1G（實際佔用記憶體 < 500M）, 高併發推薦使用 2C4G 及以上。**

<h2 id="readme-license">🛒 商業授權（私有化獨立部署）</h2>

私有化部署版本主要面向有意搭建 AI 平臺的站長與企業，交付使用者端 | 管理端 | 後端三端加密原始碼（閉源）+ 授權碼。

- 📗 商業授權版介紹：<https://docs.sparkaigc.com/pro/>
- 🗂️ 商業版系統介紹文件與定價（飛書）：[點選檢視](https://bx5gkpqv57j.feishu.cn/docx/EOWUdQ04no9PoBxyp6Ecg3AAnhf)
- 🧭 部署教程：<https://docs.sparkaigc.com/deploy/baota/process.html>
- 💬 作者微信：`DjiMain` · 作者 QQ：`501439094`（新增請備註 `SparkAi`）

![](https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/Wechat.png)

<h2 id="readme-star-history">⭐ Star History</h2>

<div align="center">

[![Star History Chart](https://api.star-history.com/svg?repos=nosqlnull/ChatGPT-SparkAi&type=Date)](https://star-history.com/#nosqlnull/ChatGPT-SparkAi&Date)

</div>
