<div align="center">

# SparkAi 系统（ChatGPT-SparkAi）

🚀 新一代 { 渐进式 } AIGC 系统 · 一站式 AI B/C 端解决方案，基于 Node.js + NestJS + Vue3 构建，支持独立私有化部署与商业运营

简体中文 | <a href="./docs/i18n/README.zh_TW.md">繁體中文</a> | <a href="./docs/i18n/README.en.md">English</a>

<p align="center">
  <a href="https://github.com/nosqlnull/ChatGPT-SparkAi/stargazers" target="_blank" rel="noopener noreferrer"><img src="https://img.shields.io/github/stars/nosqlnull/ChatGPT-SparkAi?color=brightgreen" alt="Stars"></a>
  <a href="https://docs.sparkaigc.com/log/" target="_blank" rel="noopener noreferrer"><img src="https://img.shields.io/badge/Version-V6.9.6-brightgreen" alt="Version V6.9.6"></a>
  <a href="https://docs.sparkaigc.com/pro/" target="_blank" rel="noopener noreferrer"><img src="https://img.shields.io/badge/License-Commercial-blue" alt="License Commercial"></a>
</p>

<p align="center">
  <a href="https://docs.sparkaigc.com" target="_blank" rel="noopener noreferrer"><strong>系统文档 · Docs</strong></a>
  &nbsp;•&nbsp;
  <a href="https://test.sparkaigc.com" target="_blank" rel="noopener noreferrer"><strong>演示站 · Live demo</strong></a>
  &nbsp;•&nbsp;
  <a href="https://docs.sparkaigc.com/pro/" target="_blank" rel="noopener noreferrer"><strong>商业授权 · License</strong></a>
  &nbsp;•&nbsp;
  <a href="https://docs.sparkaigc.com/log/" target="_blank" rel="noopener noreferrer"><strong>更新日志 · Changelog</strong></a>
</p>

<p align="center">
  <a href="#readme-about">项目介绍</a> •
  <a href="#readme-demo">官方演示站</a> •
  <a href="#readme-features">系统核心功能</a> •
  <a href="#readme-compare">版本对比</a> •
  <a href="#readme-preview">界面预览</a> •
  <a href="#readme-tech">技术架构</a> •
  <a href="#readme-license">商业授权</a> •
  <a href="#readme-agpl">许可证</a>
</p>

</div>

<h2 id="readme-about">📖 项目介绍</h2>

**SparkAi系统是一款支持多语言国际化的{ 渐进式 }AIGC系统，基于OpenAI/ChatGPT、最新旗舰大模型GPT-6、Anthropic Claude（Claude-Opus-5-5 / Claude-Fable-5-1）、Google Gemini、DeepSeek、🎨GPT-Image-2 / GPT-Image-2.5绘画、🍌Nano-Banana-2第二代绘画、Midjourney V8、VEO3.1 / Sora-2视频、Seedance2.5视频（即将上线）、Agent智能体 扣子（Coze）插件、工作流、函数、知识库 等AI大模型能力开发的一站式AI系统；支持「🤖AI聊天」、「🎨专业AI绘画」、「🧠AI智能体」、「🪟Coze-Agent工作流应用」、「🎬AI视频生成」等，支持独立私有部署！提供面向个人用户 (ToC)、开发者 (ToD)、企业 (ToB)的全面解决方案。**

🏅 **截至 2026 年 9 月，SparkAi 已坚持持续开发、更新迭代三年半**，并保持稳定的大版本更新节奏。近期大版本重点支持：

- 🧩 **全模型支持 / 自定义接入最新大模型**：OpenAI、Claude、Gemini、国内主流大模型及三方大模型统一走标准 chat 格式，新模型发布后即可在后台自由新增对接，无需系统更新
- 🎨 **多功能 / 多类型大模型绘画**：文生图、参考图生图、在线编辑绘图、局部涂抹编辑重绘、图生文（多模态识图），覆盖 GPT-Image-2 / GPT-Image-2.5、Nano Banana 2、Midjourney V7 / V8 等模型
- 🤖 **新一代对话架构**：Chat Completions / Responses 双端点自动路由，切换会话、关闭页面不中断生成
- 📄 **多类型文档理解**：PDF / Word / PPT / Excel 等文件上传识别与在线预览
- 💰 **积分与账户安全**：积分明细对账、模型调用失败零扣费、登录设备与异地识别

更多内容详见下方「系统核心功能」与<a href="https://docs.sparkaigc.com/log/" target="_blank" rel="noopener noreferrer">更新日志</a>。

> [!IMPORTANT]
> - SparkAi 是一套可私有化部署的 **AI 应用系统**（AIGC 网站系统软件），**不是 API 中转 / 代理系统**。
> - **系统本身不提供任何生成式人工智能服务，也不提供任何 AI 大模型、模型 API 及模型能力**；系统中的对话、绘画、视频等 AI 功能，均由使用者自行对接的第三方模型服务提供。
> - 使用者须通过合法途径自行获取上游模型服务的 API Key、账号及接口授权，并遵守上游服务商的服务条款及所在地法律法规。
> - 本项目仅面向合法合规的 AI 应用搭建、企业内部使用与私有化部署场景，禁止用于任何违法违规用途。

> [!WARNING]
> - 将本系统部署为面向公众的 AI 服务时，部署方（运营者）即为服务提供者，对站点内容与运营行为承担全部责任；SparkAi 仅提供系统软件，不参与任何站点的运营。
> - 在中国境内面向公众提供生成式人工智能服务，须遵守 <a href="http://www.cac.gov.cn/2023-07/13/c_1690898327029107.htm" target="_blank" rel="noopener noreferrer">《生成式人工智能服务管理暂行办法》</a> 等规定，自行完成备案、内容安全、用户实名、日志留存、税务、支付资质及上游授权等合规义务。
> - 系统内置的敏感词过滤、内容审核等风控功能仅为辅助工具，不能替代运营者的合规义务。

<h2 id="readme-demo">🖥️ 官方演示站</h2>

唯一官方演示站点（其他地址均为非官方）：

| 入口 | 地址 |
|---|---|
| 系统用户端 | <a href="https://test.sparkaigc.com" target="_blank" rel="noopener noreferrer">https://test.sparkaigc.com</a> |
| 管理后端 | <a href="https://test.sparkaigc.com/sparkai/admin" target="_blank" rel="noopener noreferrer">https://test.sparkaigc.com/sparkai/admin</a> |
| 测试账号 / 密码 | `admin` / `123456` |
| SparkAi 系统文档 | <a href="https://docs.sparkaigc.com" target="_blank" rel="noopener noreferrer">https://docs.sparkaigc.com</a> |

<h2 id="readme-features">🌟 系统核心功能（授权商业部署版）</h2>

**阅读说明**

🎉 一站式 AIGC 系统：集成 AI 大模型对话、专业 AI 绘画、AI 视频生成、AI 智能体、文档上传分析、多模态图像理解、TTS & 语音识别对话等能力。

以下按功能模块归类，并标注对应支持的模型与引入版本（如 `V6.9.6`），各版本完整内容请查看<a href="https://docs.sparkaigc.com/log/" target="_blank" rel="noopener noreferrer">更新日志</a>。具体模型能否使用，取决于所接入上游 API 渠道的支持情况。

### 🔥 近期大版本更新亮点
**V6.9.x 系列重点更新**

- **V6.9.6 大更新**：重构大模型对话架构，支持 OpenAI Chat Completions 与 Responses 双端点自动路由；新增官方模型多类型文档理解、大模型全局配置中心、对话文件在线预览；重构积分明细系统并支持模型调用失败零扣费；新增登录设备与异地识别系统
- **V6.9.5**：新增对话导航条、对话演示数据、「画廊精选 / 我的绘画」分栏加载；重构个人中心 UI；中文字体子集化等性能优化，单页资源下载量降低约 50%
- **V6.9.4**：新增 Nano Banana 2 独立绘画模块；重构绘画模块架构（可复用底座 + 异步任务编排）；新增强制指定用户下线、「系统功能测试」开关
- **V6.9.3 大更新**：AI 对话内核重构为上下游解耦的异步运行模型，SSE 流式链路增量持久化；风控敏感词检测扩展至绘画与思维导图；GPT-Image-2 绘画模块重构
- **V6.9.2**：新增 GPT-Image-2 独立绘画模块（文生图 / 参考图 / 在线编辑）、网站直播入口
- **V6.9.1**：系统全国际化 + 管理后台一键 AI 国际化、Midjourney V8 支持、登录注册页重构
- **V6.9.0**：2026 用户端 UI 大重构（卡片风格 / Notion 风格双主题）、AI 对话沉浸模式

### 🤖 一、AI 大模型对话
**对话能力与模型支持**

1. 🔥 **全模型支持**：支持 OpenAI 官方 API + 一切标准 chat 格式中转 API；覆盖 OpenAI（GPT-6 / GPT-5.4 / GPT-5.4-pro / o3 / o4-mini / Codex 系列）、Anthropic Claude（Claude-Opus-5-5 / Claude-Fable-5-1 等）、Google Gemini（Gemini-3.1-pro 等）、DeepSeek（deepseek-r1 等）、Azure OpenAI，以及豆包、通义千问、智谱 ChatGLM、Moonshot、讯飞星火、百川、腾讯混元、360 智脑等国内模型；适配 LocalAI / Ollama 本地模型
2. 🎈 **后台自由自定义接入最新大模型（无需系统更新）**：OpenAI 全模型、Claude 全模型、Gemini 全模型、国内 AI 全模型及三方主流大模型统一走标准 chat（OpenAI）格式，新模型发布后即可在后台自由新增对接并立即使用；支持模型自定义分类、名称、排序、Logo 与厂商分组
3. 🧭 **双端点智能路由** `V6.9.6`：按模型能力自动路由 Chat Completions / Responses 端点——命中规则的 OpenAI 官方系列（GPT / o 系列 / Codex）走 Responses 官方通道，Claude / Gemini / DeepSeek 等稳定使用 Chat Completions；内置多级失败自动降级重试
4. ⚙️ **大模型全局配置中心** `V6.9.6`：统一管理端点路由规则、失败是否扣费、stream 流式参数等全局策略，支持正则规则与模型名实时测试，保存即时生效、无需重启
5. 📄 **多类型文档理解** `V6.9.6`：官方模型支持 PDF / Word / PPT / Excel / 文本 / Markdown / HTML 等文件上传识别（非 PDF 文件建议选择 GPT 系列模型，经 Responses 端点）；支持 URL 拼接 / Base64 内联 / 文件链接三种提交方式，按体积与 Token 上限自动择优与降级
6. 👀 **对话文件在线预览** `V6.9.6`：PDF / Word / PPT / Excel / 文本 / Markdown / HTML 在线查看、打印、下载，Coze Agent 对话同步支持
7. 🖼️ **多模态图像理解**：单图 / 多图上传（最多 9 张），支持手机原生相机与 PC 摄像头拍照上传 `V6.9.3`；用户消息多图自适应排版 `V6.9.6`；API 返回图片自动预览
8. 🤔 **深度思考与推理**：支持 o3 / o4-mini、DeepSeek-R1 等推理模型，思维链（ReasoningContent / Think 标签）流式输出与展示，支持深度搜索过程显示
9. 🛜 **联网搜索**：支持模型联网扩展搜索实时内容并总结（如 o4-mini-all：联网 + 推理 + 图像 + PDF 文档分析）
10. 🛡️ **高可靠对话内核** `V6.9.3`：上游（后端 ↔ 大模型）与下游（前端 ↔ 后端）连接解耦，切换会话、关闭页面、退出客户端均不中断生成；SSE 边生成边落库，切回会话可续显；「停止回答」即时取消上游请求；首字超时 / 空响应统一兜底；多会话并发隔离
11. 📌 **对话导航条** `V6.9.5`：当前对话组内提问 ≥ 3 条时自动出现，支持折叠、悬停展开、点击定位
12. Ⓜ️ **强大的内容渲染**：Markdown（代码高亮 / LaTeX / KaTeX 公式 / Mermaid / 图表绘制）、思维导图生成与 PDF 导出、代码文件下载、对话重新编辑
13. 🗣️ **语音对话**：支持 OpenAI / Azure 语音识别与 TTS（Whisper & TTS 格式中转），语音输入语音回复、多种音色选择，后台可开关语音播放
14. 🏄‍♂️ **插件系统与开放对接**：内置插件系统（识图、文档分析等，持续扩展）；兼容 chat 接口的知识库或工作流应用（如 FastGPT 知识库 / 工作流）可作为模型接入，或绑定到智能体使用

### 🎨 二、专业 AI 绘画
**独立绘画模块与模型支持**

15. 🖌️ **GPT-Image-2 独立绘画模块** `V6.9.2` `V6.9.3`：支持 gpt-image-2、gpt-image-2.5、GPT-Image-2-Dev 等模型，后台可自定义接入 API 与扩展模型版本；文生图、参考图绘画（最多 8 张智能参考图）、已生成结果在线编辑与涂抹框选编辑；画质（low / medium / high / auto）、数量、比例与自定义分辨率严格按官方参数范围提交；支持单用户 / 全系统并发限制
16. 🍌 **Nano Banana 2 独立绘画模块** `V6.9.4`：支持 gemini-3.1-flash-image、gemini-3-pro-image，可自定义扩展模型版本（如 gemini-3.1-flash-lite-image）；文生图、多张智能参考图编辑、自定义分辨率与比例（2K / 4K 输出取决于模型）；也可在 AI 对话中直接选用 Nano Banana 模型绘图
17. 🎨 **Midjourney / Niji 全功能**：支持 MJ V7 / V8（V8 待官方 API 正式开放后直接可用）；Imagine / Upscale / Vary / Zoom Out / Pan、Vary Region 局部重绘、图像混合，普通参考图 / 角色一致（cref）/ 风格一致（sref）参考图组合使用；Fast / Relax 双通道独立计费与并发；绘画进度实时渲染
18. 🪄 **DALL·E 2 / 3 绘画**：支持全部参数
19. 🔁 **通用绘画能力**：「画同款」一键复用参数；各模型、各操作积分价格前端动态显示；绘画失败自动退还积分（幂等退款，杜绝重复返还）`V6.9.6`；异常任务定时补偿；原图 + 缩略图私有化存储；各绘画模型前端显示开关；绘画进度条
20. 🖼️ **AI 画廊广场**：「画廊精选 / 我的绘画」分栏加载 `V6.9.5`；作品风格分类、轮播图、创作者中心；视频作品悬停自动预览播放
21. 🚥 **绘画内容风控** `V6.9.3`：GPT-Image / Midjourney / Niji / DALL·E 提示词提交前即做敏感词拦截，不调用上游、不扣费，违规记录同步至管理后台

### 🎬 三、AI 视频生成
**视频模型支持**

22. 📽️ **VEO3 / VEO3.1 视频**：支持 VEO3.1、VEO3.1-fast、VEO3.1-pro 等模型，生成视频自动配套音频（标准 chat 对话形式调用）
23. 📽️ **Sora-2 视频**：支持 Sora-2 视频生成（标准 chat 对话形式调用）
24. 🎞️ **Midjourney HD 视频** `V6.8.6`：已生成图片一键生成「动图（高运动 / 低运动）」，支持自定义动作描述、单次 1 / 2 / 4 条生成，独立扣费配置
25. 🎬 **独立 AI 视频模块**：文生视频 / 图生视频（Pika），视频作品广场展示
26. 🌱 **Seedance 视频（Coze-Agent）**：通过 Coze-Agent「Seedance 大模型视频生成」应用调用字节跳动官方 Seedance 模型，支持首尾帧与带声音视频，生成结果在系统内直接预览播放
27. 🔜 **即将上线**：Seedance2.5 视频、Qwen-Image 图片编辑、可灵等独立图片 / 视频模块（2026 下半年开发计划）

### 🧠 四、AI 智能体（Agent）
**智能体与应用生态**

28. 🤖 **Coze Agent 智能体模块**：支持扣子（Coze）插件、工作流、函数、知识库智能体对接；实时流式响应，展示思考过程与模型 / 插件 / 工作流调用详情；单智能体多开对话；支持多文件类型上传，图片 / 视频结果直接预览
29. 📥 **智能体批量管理**：从 Coze 平台一键批量导入与同步智能体（Redis 分布式锁防重复），图标自动私有化存储
30. 📈 **智能体商店**：自研评分、活跃度、热度算法；推荐问题、关键字搜索；链接分享、微信扫码分享、海报分享
31. 🧠 **GPTs 与预设应用**：GPTs 应用全网搜索一键接入；Prompt 自定义预设应用；用户自建智能体；应用可绑定模型、分享链接、共享到广场

### 💰 五、会员积分与商业运营
**计费、支付与增长**

32. 🧑‍🤝‍🧑 **会员积分体系**：普通模型积分、高级模型积分、绘画积分、Agent 积分多种余额；按次 / 按时间 / 组合套餐等多种计费方式，每个模型可自定义扣费
33. 🧾 **积分明细系统** `V6.9.6`：用户端与管理端口径统一，完整记录全模型使用的消耗、失败返还、失败免扣，时间精确到秒，支持多维度筛选对账；管理后台对话列表展示每条回复的积分消耗
34. 🆓 **模型调用失败零扣费** `V6.9.6`：4xx / 5xx、超时、空回复可按开关不扣积分；失败 / 中断 / 空回复统一结算出口，杜绝误扣与重复扣费，并具备防刷保护
35. 🛍️ **支付系统**：微信官方支付（PC 端 Native 扫码、手机微信内 JSAPI）、易支付、码支付、虎皮椒支付；订单状态同步检查、订单搜索与管理
36. 🛒 **商城与增长工具**：永久 / 限时套餐商城、签到奖励、邀请奖励、卡密兑换（批量生成与管理）、访客体验模式
37. ⏏️ **分销系统**：A + B 分销模式，可按用户单独设置提成；支持提现门槛与支付宝 / 微信 / 银行卡提现
38. ✨ **渠道负载均衡**：自研渠道均衡负载与分配算法，API Key 池多 Key 轮询（优先级 / 权重 / 状态管理），支持批量添加与删除

### 🔐 六、安全与风控
**内容安全与账户安全**

39. 🚥 **内容风控**：自定义敏感词 + 百度内容审核，覆盖对话、绘画、思维导图，命中即前置拦截；违规检测记录与用户快照全量留痕
40. 📍 **登录设备与异地识别** `V6.9.6`：记录登录 IP（解析至运营商与所在城市）、浏览器、操作系统与设备类型；用户可在个人中心查看最近 5 次登录设备与在线状态，管理端同步展示
41. 🔑 **会话安全**：普通用户仅允许单设备在线；超级管理员账户按登录 IP 区分会话，异地登录相互强制下线并记录 IP；支持后台强制指定用户下线 `V6.9.4`、封禁用户
42. 🙈 **敏感信息脱敏**：演示 / 非超管账户查看 IP 与地区、配置值、API 地址、密钥、用户名、邮箱等信息时统一脱敏；admin 演示账户只读
43. 📤 **上传安全**：服务端拒绝脚本 / 代码类可执行文件；开启云存储后禁止匿名写入本机磁盘，游客上传限频限量
44. 🧪 **「系统功能测试」开关** `V6.9.4`：开启后所有 AI 生成请求在系统层统一阻断、不调用上游 API，适用于尚未完成生成式人工智能备案的上线阶段
45. 📧 **注册防护**：邮箱域名白名单、可禁用「+」别名邮箱、临时邮箱过滤；注册赠送额度防篡改

### 🛠️ 七、管理后台与站点运营
**后台管理与运营配置**

46. 📊 **数据仪表盘**：用户、对话、绘画、订单统计与近 7 日趋势折线图，模型使用次数与 Token 使用饼图
47. 💻 **完整管理后台**：用户、订单、对话、绘画、视频等数据管理，支持 Excel 导出；百万级数据量查询优化（统计查询并发 + Redis 缓存）；用户列表展示登录 IP 记录 `V6.9.6`
48. 🗂️ **模型与卡池管理**：模型分类、排序、Logo、厂商分组，按厂商预选新一代模型 `V6.9.6`；API 卡池批量添加 / 删除 Key
49. 🎭 **对话演示数据** `V6.9.5`：可指定任意对话组（最多 5 条）作为全站只读演示内容
50. ✔️ **站点自定义**：Logo / 站点名称 / 页脚 / 百度统计 / 版权信息 / 备案号 / 公告 / 欢迎语 / 关于我们 / 用户协议等均可后台配置；网站直播入口 `V6.9.2`
51. 🧩 **动态菜单与轮播图**：支持内嵌网页、外链、内部路径跳转，自定义图标，PC 与移动端分别配置；广告位 / 活动 / 教程轮播展示
52. ♻️ **微信公众号联动**：公众号登录、关键词自动回复
53. 🔐 **权限系统**：超级管理员与演示账户分级权限

### 🌏 八、多端体验与系统架构
**体验、性能与部署**

54. 🌐 **系统全国际化** `V6.9.1`：前端界面 + 后端配置信息 + 后端返回信息全量国际化，按访问 IP 与浏览器语言自动切换；管理后台配置内容一键 AI 翻译，支持出海运营
55. 🎨 **双风格 UI** `V6.9.0`：卡片风格 / Notion 风格用户自由切换；AI 对话沉浸模式、「添加菜单」收纳、液态玻璃按钮、明暗主题自动适配
56. 📲 **多端支持**：PC 端 + 手机 H5 + 微信公众号，自适应 PC / 移动端 / 平板；支持 PWA，H5 可打包至其他平台
57. ⚡ **性能优化** `V6.9.5`：中文字体子集化（单个字重 4.2MB → 0.9MB），单页资源下载量降低约 50%，移动端资源分批加载，降低 iOS 等低内存设备崩溃风险
58. 🚀 **高并发服务端**：Node.js + NestJS 服务端，Redis 缓存与 MySQL 连接池自适应，适配高并发业务场景
59. 🗄️ **存储与数据同步**：本地存储 / 阿里云 OSS / 腾讯云 COS / Chevereto 图床，用户文件与绘画数据私有化存储；对话会话隔离、云端存储，多设备数据同步
60. 🖥️ **部署运行**：支持宝塔常规部署与 Docker 一键部署，所有对接配置均在后台界面完成；适用于商业运营、企业内部、教育培训等多种场景
61. 🏅 **持续更新**：已坚持开发迭代三年半，保持稳定的大版本更新节奏，更多 AI 能力持续开发中……

<h2 id="readme-compare">📊 公益免费商业版 vs 商业授权版</h2>

公益免费商业版（Public Good V2.1.0 · 2026 特别公益重构版，支持会员套餐、在线支付、分销等商业功能）仓库：<a href="https://github.com/nosqlnull/SparkAi-ChatGPT-AiWeb" target="_blank" rel="noopener noreferrer">SparkAi-ChatGPT-AiWeb</a>

| 功能 | 公益免费商业版（Public Good V2.1.0） | 商业授权版（V6.9.6） |
|---|---|---|
| 使用范围 | ✅ 支持商业运营 | ✅ 支持商业运营 |
| 版本迭代 | 2026 特别公益重构版（功能底座 V3.2.0），部分功能更新 | ✅ 持续大版本更新 |
| AI 大模型 | ✅ GPT-3.5 / GPT-4.0、Azure 及部分国内模型<br>🔜 即将支持 GPT-6、Claude-Opus-5-5 / Claude-Fable-5-1、Gemini、DeepSeek 等全模型（预计 2026.10） | ✅ GPT-6、Claude-Opus-5-5 / Claude-Fable-5-1、Gemini、DeepSeek 等全模型 |
| 后台自定义接入最新大模型（无需系统更新） | 🔜 即将支持（待更新至 GitHub，预计 2026.10） | ✅ |
| 双端点智能路由 / 大模型全局配置中心 | ❌ | ✅ |
| 深度思考推理（o3 / DeepSeek-R1 等） | ❌ | ✅ |
| 多图识图 / 多类型文档理解与在线预览 | ❌ | ✅ |
| DALL·E 绘画 | ✅ DALL·E 2 / 3 | ✅ DALL·E 2 / 3 |
| Midjourney 绘画 | ✅ 文生图、图生图、局部重绘 | ✅ 全功能：V7 / V8、Niji、角色 / 风格一致参考图、HD 视频 |
| GPT-Image-2 / Nano Banana 2 独立绘画模块 | ❌ | ✅ |
| AI 视频生成（VEO3.1 / Sora-2 / Pika / Seedance） | ❌ | ✅ |
| AI 智能体 | ✅ Prompt 自定义预设应用 | ✅ 另支持 Coze Agent、GPTs 应用、智能体商店 |
| 注册登录 | ✅ 微信扫码 / 邮箱 / 手机号 | ✅ 另支持登录设备与异地识别 |
| 卡密兑换 | ✅ | ✅ |
| 会员套餐 | ✅ 永久 / 限时会员套餐 | ✅ 多种积分余额，永久 / 限时 / 组合套餐，每个模型自定义扣费 |
| 支付系统 | ✅ 易支付 / 码支付 / 虎皮椒 | ✅ 微信官方支付 / 易支付 / 码支付 / 虎皮椒 |
| 分销推广 | ✅ 分销邀请、佣金提现 | ✅ A + B 分销、按用户单独设置提成、提现门槛 |
| 积分明细 / 模型调用失败零扣费 | ❌ | ✅ |
| 增强风控（敏感信息脱敏、「系统功能测试」开关等） | ❌ | ✅ |
| 系统全国际化 | ❌ | ✅ |
| 2026 新版 UI（卡片 / Notion 双风格、沉浸模式） | ❌ | ✅ |
| 完整商用管理后台 | 基础管理 | ✅ 数据仪表盘、模型与卡池、动态菜单、全局配置 |

<h2 id="readme-preview">🖼️ 界面预览</h2>

> 截图与 <a href="https://bx5gkpqv57j.feishu.cn/docx/EOWUdQ04no9PoBxyp6Ecg3AAnhf" target="_blank" rel="noopener noreferrer">商业版系统介绍文档（飞书）</a> 保持一致，非实时最新，实际效果请以 <a href="https://test.sparkaigc.com" target="_blank" rel="noopener noreferrer">官方演示站</a> 为准。

### 💻 PC 端（部分展示）

#### 用户注册登录

支持微信环境静默登录、浏览器中微信主动扫码登录、邮箱注册登录、手机号注册登录。`V6.9.1` 起全新的创意动画登录界面（原生 CSS + Vue 3 Composition API 从零实现）。

<p align="center">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-login-1.jpg" alt="用户注册登录" width="49%">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-login-2.jpg" alt="用户注册登录" width="49%">
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-login-3.jpg" alt="用户注册登录" width="49%">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-login-4.jpg" alt="用户注册登录" width="49%">
</p>

#### 系统多语言国际化

全国际化：不仅是前端固定内容，还支持后端配置信息与后端返回信息的国际化。

![系统多语言国际化](https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-i18n.jpg)

#### AI 大模型对话

支持 OpenAI、Gemini、Claude 全模型，以及国内 AI 全模型与三方主流大模型（市面标准 Chat 格式 API 均可对接）。

![AI 大模型对话](https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-chat.jpg)

#### AI 智能体应用

GPTs 应用 + Prompt 自定义预设应用；GPTs 支持后台自定义添加，也可全站搜索（同官方搜索）。

![AI 智能体应用](https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-agent.jpg)

#### 用户自定义创建预设应用智能体

智能体应用工作台，支持连续上下文使用。

<p align="center">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-agent-custom-1.jpg" alt="用户自定义创建预设应用智能体" width="49%">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-agent-custom-2.jpg" alt="用户自定义创建预设应用智能体" width="49%">
</p>

#### Midjourney 绘画全功能

支持绘画进度实时渲染显示。

<p align="center">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-mj-1.jpg" alt="Midjourney 绘画全功能" width="49%">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-mj-2.jpg" alt="Midjourney 绘画全功能" width="49%">
</p>

#### 垫图生图

支持普通参考图、角色一致参考图、风格一致参考图，可单独或组合使用；支持上传预览、图片类型与垫图序号显示。

![垫图生图](https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-mj-reference.jpg)

#### Vary Region 局部编辑重绘

![Vary Region 局部编辑重绘](https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-mj-vary-region.jpg)

#### 图像混合

![图像混合](https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-mj-blend.jpg)

#### DALL·E 绘画

![DALL·E 绘画](https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-dalle.jpg)

#### Midjourney HD 视频

全新的 MJ 高清视频创作能力（`V6.8.6` 起）。

![Midjourney HD 视频](https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-mj-video-1.jpg)

<p align="center">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-mj-video-2.jpg" alt="Midjourney HD 视频" width="49%">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-mj-video-3.jpg" alt="Midjourney HD 视频" width="49%">
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-mj-video-4.jpg" alt="Midjourney HD 视频" width="49%">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-mj-video-5.jpg" alt="Midjourney HD 视频" width="49%">
</p>

#### AI 画廊广场

包含创作者功能。

![AI 画廊广场](https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-gallery-1.jpg)

<p align="center">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-gallery-2.jpg" alt="AI 画廊广场" width="49%">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-gallery-3.jpg" alt="AI 画廊广场" width="49%">
</p>

#### AI 视频生成 / AI 视频广场

支持文生视频、图生视频。

![AI 视频生成 / AI 视频广场](https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-video.jpg)

#### 用户会员套餐商城

后台自定义限时套餐与永久套餐，可随意组合。

<p align="center">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-shop-1.jpg" alt="用户会员套餐商城" width="49%">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-shop-2.jpg" alt="用户会员套餐商城" width="49%">
</p>

#### 分销推介

<p align="center">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-distribution-1.jpg" alt="分销推介" width="49%">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-distribution-2.jpg" alt="分销推介" width="49%">
</p>

### 📱 H5 手机端（部分展示）

<p align="center">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/h5-01.jpg" alt="H5 手机端" width="32%">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/h5-02.jpg" alt="H5 手机端" width="32%">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/h5-03.jpg" alt="H5 手机端" width="32%">
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/h5-04.jpg" alt="H5 手机端" width="32%">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/h5-05.jpg" alt="H5 手机端" width="32%">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/h5-06.jpg" alt="H5 手机端" width="32%">
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/h5-07.jpg" alt="H5 手机端" width="32%">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/h5-08.jpg" alt="H5 手机端" width="32%">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/h5-09.jpg" alt="H5 手机端" width="32%">
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/h5-10.jpg" alt="H5 手机端" width="32%">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/h5-11.jpg" alt="H5 手机端" width="32%">
</p>

更多内容请访问 <a href="https://test.sparkaigc.com" target="_blank" rel="noopener noreferrer">官方演示站</a> 体验。

### 💳 微信官方原生支付

支持官方微信支付、易支付、码支付、虎皮椒支付等方式，支持同步检查订单状态、订单搜索与管理。

开启官方微信支付后，PC 端调用 Native 支付（直接生成二维码支付）：

![PC 端微信 Native 支付](https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pay-pc-native.jpg)

手机微信环境内调用 JSAPI 支付（直接唤起微信钱包支付）：

<p align="center">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pay-h5-jsapi.jpg" alt="手机端微信 JSAPI 支付" width="32%">
</p>

### 🛠️ 系统管理后台

请访问 <a href="https://test.sparkaigc.com/sparkai/admin" target="_blank" rel="noopener noreferrer">官方演示站管理后台</a> 查看（测试账号 `admin` / `123456`）。

<h2 id="readme-tech">🧱 技术架构与部署环境</h2>

### ✨系统技术架构
**系统架构**

- 前端：Vite + Vue3 + TypeScript + NaiveUI + TailwindCSS
- 管理端：Vite4 + Vue3 + Element-Plus
- 服务端（后端）：Node.js + NestJS
- 数据支持：MySQL5.7(+) / MySQL8 + Redis
- 运行环境：Linux、Windows、macOS（推荐使用Linux）
- 数据存储：本地存储 | 对象存储阿里云OSS | 对象存储腾讯云COS | Chevereto图床

### 🛠️运行环境
**运行环境**

- Linux (推荐)
- Windows
- MacOS Server
- Docker
- Kubernetes
- 支持 ARM64 & X86 (32/64) 架构

### 🎯服务器配置要求
**最低服务器配置运行要求 1C1G（实际占用内存 < 500M）, 高并发推荐使用 2C4G 及以上。**

<h2 id="readme-license">🛒 商业授权（私有化独立部署）</h2>

私有化部署版本主要面向有意搭建 AI 平台的站长与企业，交付用户端 | 管理端 | 后端三端加密源代码（闭源）+ 授权码。

- 📗 商业授权版介绍：<a href="https://docs.sparkaigc.com/pro/" target="_blank" rel="noopener noreferrer">https://docs.sparkaigc.com/pro/</a>
- 🗂️ 商业版系统介绍文档与定价（飞书）：<a href="https://bx5gkpqv57j.feishu.cn/docx/EOWUdQ04no9PoBxyp6Ecg3AAnhf" target="_blank" rel="noopener noreferrer">点击查看</a>
- 🧭 部署教程：<a href="https://docs.sparkaigc.com/deploy/baota/process.html" target="_blank" rel="noopener noreferrer">https://docs.sparkaigc.com/deploy/baota/process.html</a>
- 💬 作者微信：`DjiMain` · 作者 QQ：`501439094`（添加请备注 `SparkAi`）

![](https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/Wechat.png)

<h2 id="readme-star-history">⭐ Star History</h2>

<div align="center">

<a href="https://star-history.com/#nosqlnull/ChatGPT-SparkAi&Date" target="_blank" rel="noopener noreferrer">![Star History Chart](https://api.star-history.com/svg?repos=nosqlnull/ChatGPT-SparkAi&type=Date)</a>

</div>

<h2 id="readme-agpl">📜 许可证</h2>

本仓库公开内容（项目说明文档、系统界面截图等）采用 [GNU Affero 通用公共许可证 v3.0 (AGPLv3)](./LICENSE) 授权。

SparkAi 商业授权版系统（用户端 / 管理端 / 服务端）不包含在本仓库内，也不适用上述开源许可证，需通过 <a href="https://docs.sparkaigc.com/pro/" target="_blank" rel="noopener noreferrer">官方商业授权</a> 获取使用许可。

如果您所在的组织政策不允许使用 AGPLv3 许可的内容，或您希望规避 AGPLv3 的开源义务，请发送邮件至：[evenkepler@gmail.com](mailto:evenkepler@gmail.com)，或添加作者微信 `DjiMain`（备注 `SparkAi`）。
