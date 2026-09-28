<div align="center">

# SparkAi System (ChatGPT-SparkAi)

🚀 The new generation { Progressive } AIGC system · a one-stop AI B/C-end solution built on Node.js + NestJS + Vue3, supporting independent private deployment and commercial operation

<a href="../../README.md">简体中文</a> | <a href="./README.zh_TW.md">繁體中文</a> | English

<p align="center">
  <a href="https://github.com/nosqlnull/ChatGPT-SparkAi/stargazers" target="_blank" rel="noopener noreferrer"><img src="https://img.shields.io/github/stars/nosqlnull/ChatGPT-SparkAi?color=brightgreen" alt="Stars"></a>
  <a href="https://docs.sparkaigc.com/en/log/" target="_blank" rel="noopener noreferrer"><img src="https://img.shields.io/badge/Version-V6.9.6-brightgreen" alt="Version V6.9.6"></a>
  <a href="https://docs.sparkaigc.com/en/pro/" target="_blank" rel="noopener noreferrer"><img src="https://img.shields.io/badge/License-Commercial-blue" alt="License Commercial"></a>
</p>

<p align="center">
  <a href="https://docs.sparkaigc.com/en/" target="_blank" rel="noopener noreferrer"><strong>Docs</strong></a>
  &nbsp;•&nbsp;
  <a href="https://test.sparkaigc.com" target="_blank" rel="noopener noreferrer"><strong>Live demo</strong></a>
  &nbsp;•&nbsp;
  <a href="https://docs.sparkaigc.com/en/pro/" target="_blank" rel="noopener noreferrer"><strong>Commercial License</strong></a>
  &nbsp;•&nbsp;
  <a href="https://docs.sparkaigc.com/en/log/" target="_blank" rel="noopener noreferrer"><strong>Changelog</strong></a>
</p>

<p align="center">
  <a href="#readme-about">Introduction</a> •
  <a href="#readme-demo">Official Demo</a> •
  <a href="#readme-features">Core Functions</a> •
  <a href="#readme-compare">Comparison</a> •
  <a href="#readme-preview">Screenshots</a> •
  <a href="#readme-tech">Architecture</a> •
  <a href="#readme-license">Commercial License</a> •
  <a href="#readme-agpl">License</a>
</p>

</div>

<h2 id="readme-about">📖 Project Introduction</h2>

**SparkAi is a { Progressive } AIGC system with multi-language internationalization support – a one-stop AI system built on OpenAI/ChatGPT, the latest flagship model GPT-6, Anthropic Claude (Claude-Opus-5-5 / Claude-Fable-5-1), Google Gemini, DeepSeek, 🎨GPT-Image-2 / GPT-Image-2.5 painting, 🍌Nano-Banana-2 second-generation painting, Midjourney V8, VEO3.1 / Sora-2 video, Seedance2.5 video (coming soon), Agent intelligent agents with Coze plugins, workflows, functions, knowledge bases, and other large-model capabilities; it supports "🤖AI Chat", "🎨Professional AI Painting", "🧠AI Agents", "🪟Coze-Agent Workflow Apps", "🎬AI Video Generation", etc., and supports independent private deployment!**

It provides comprehensive solutions for individual users (ToC), developers (ToD), and enterprises (ToB).

🏅 **As of September 2026, SparkAi has been under continuous development and iteration for three and a half years**, with a steady cadence of major releases. Recent major versions focus on:

- 🧩 **Full model support / custom integration of the latest models**: OpenAI, Claude, Gemini, mainstream domestic models, and third-party models all use the standard chat format, so newly released models can be added freely in the admin backend without a system update
- 🎨 **Multi-function / multi-type model painting**: text-to-image, reference-image generation, online image editing, partial brush-edit repainting, and image-to-text (multimodal image understanding), covering GPT-Image-2 / GPT-Image-2.5, Nano Banana 2, Midjourney V7 / V8 and more
- 🤖 **New-generation dialogue architecture**: automatic routing between Chat Completions / Responses endpoints; switching sessions or closing the page does not interrupt generation
- 📄 **Multi-type document understanding**: upload recognition and online preview of PDF / Word / PPT / Excel and other files
- 💰 **Points and account security**: points details reconciliation, zero charge on failed model calls, login device and remote-login detection

See "System Core Functions" below and the <a href="https://docs.sparkaigc.com/en/log/" target="_blank" rel="noopener noreferrer">Changelog</a> for more details.

> [!IMPORTANT]
> - SparkAi is a privately deployable **AI application system** (AIGC website system software), **not an API relay or proxy system**.
> - **The system itself does not provide any generative AI service, nor any AI large model, model API, or model capability.** The chat, painting, video, and other AI features are provided by third-party model services that the user connects on their own.
> - Users must obtain API keys, accounts, and interface authorization for upstream model services through legitimate channels, and comply with the upstream providers' terms of service and applicable local laws and regulations.
> - This project is intended only for lawful AI application building, internal enterprise use, and private deployment. Any illegal use is prohibited.

> [!WARNING]
> - When the system is deployed as a public-facing AI service, the deployer (operator) is the service provider and bears full responsibility for the site's content and operations. SparkAi only provides the system software and does not take part in operating any site.
> - Public-facing generative AI services in mainland China must comply with the <a href="http://www.cac.gov.cn/2023-07/13/c_1690898327029107.htm" target="_blank" rel="noopener noreferrer">Interim Measures for the Management of Generative AI Services</a> and related rules. Operators must complete filing, content security, real-name verification, log retention, taxation, payment qualification, upstream authorization, and other compliance obligations themselves.
> - The built-in sensitive-word filtering, content moderation, and other risk-control features are auxiliary tools only and do not replace the operator's compliance obligations.

<h2 id="readme-demo">🖥️ Official Demo</h2>

The only official demo site (all other addresses are unofficial):

| Entry | Address |
|---|---|
| User end | <a href="https://test.sparkaigc.com" target="_blank" rel="noopener noreferrer">https://test.sparkaigc.com</a> |
| Admin backend | <a href="https://test.sparkaigc.com/sparkai/admin" target="_blank" rel="noopener noreferrer">https://test.sparkaigc.com/sparkai/admin</a> |
| Test account / password | `admin` / `123456` |
| SparkAi documentation | <a href="https://docs.sparkaigc.com/en/" target="_blank" rel="noopener noreferrer">https://docs.sparkaigc.com/en/</a> |

<h2 id="readme-features">🌟 System Core Functions (Authorized Commercial Deployment Version)</h2>

**How to Read This Section**

🎉 One-stop AIGC system: integrates AI large-model dialogue, professional AI painting, AI video generation, AI agents, document upload and analysis, multimodal image understanding, TTS & voice recognition dialogue, and more.

Features below are grouped by module and labeled with the supported models and the version that introduced them (e.g. `V6.9.6`). See the <a href="https://docs.sparkaigc.com/en/log/" target="_blank" rel="noopener noreferrer">Changelog</a> for full details of each version. Whether a specific model is available depends on the upstream API channel you connect.

### 🔥 Highlights of Recent Major Updates
**Key Updates in the V6.9.x Series**

- **V6.9.6 Major Update**: Refactored the large-model dialogue architecture with automatic routing between the OpenAI Chat Completions and Responses endpoints; added multi-type document understanding for official models, a large-model global configuration center, and in-dialogue file preview; refactored the points details system with zero charges on failed model calls; added a login device & remote-login detection system
- **V6.9.5**: Added a dialogue navigation bar, dialogue demo data, and "Gallery Picks / My Paintings" tabs; refactored the personal center UI; performance optimizations such as Chinese font subsetting, reducing single-page resource downloads by about 50%
- **V6.9.4**: Added the standalone Nano Banana 2 painting module; refactored the painting module architecture (reusable foundation + asynchronous task orchestration); added forcing specified users offline and the "System Function Test" switch
- **V6.9.3 Major Update**: Refactored the AI dialogue core into an asynchronous execution model with decoupled upstream/downstream connections and incremental persistence of the SSE stream; extended sensitive-word risk control to painting and mind maps; refactored the GPT-Image-2 painting module
- **V6.9.2**: Added the standalone GPT-Image-2 painting module (text-to-image / reference images / online editing) and a website live-stream entry
- **V6.9.1**: Full system internationalization + one-click AI internationalization in the admin backend, Midjourney V8 support, refactored login/registration pages
- **V6.9.0**: 2026 user-end UI overhaul (card style / Notion style themes) and AI dialogue immersion mode

### 🤖 1. AI Large-Model Dialogue
**Dialogue Capabilities & Model Support**

1. 🔥 **Full Model Support**: Supports the official OpenAI API + any standard chat-format relay API; covers OpenAI (GPT-6 / GPT-5.4 / GPT-5.4-pro / o3 / o4-mini / Codex series), Anthropic Claude (Claude-Opus-5-5 / Claude-Fable-5-1, etc.), Google Gemini (Gemini-3.1-pro, etc.), DeepSeek (deepseek-r1, etc.), Azure OpenAI, and domestic models such as Doubao, Tongyi Qianwen, Zhipu ChatGLM, Moonshot, iFlytek Spark, Baichuan, Tencent Hunyuan, and 360 Zhi Nao; adapts to LocalAI / Ollama local models
2. 🎈 **Freely Integrate the Latest Models in the Backend (No System Update Needed)**: All OpenAI, Claude, Gemini, domestic, and mainstream third-party models use the standard chat (OpenAI) format, so newly released models can be added freely in the admin backend and used immediately; supports custom model categories, names, sorting, logos, and vendor groups
3. 🧭 **Dual-Endpoint Smart Routing** `V6.9.6`: Automatically routes between the Chat Completions / Responses endpoints based on model capabilities — official OpenAI series matching the rules (GPT / o-series / Codex) use the official Responses channel, while Claude / Gemini / DeepSeek, etc. consistently use Chat Completions; built-in multi-level automatic fallback retries on failure
4. ⚙️ **Large Model Global Configuration Center** `V6.9.6`: Centrally manages global policies such as endpoint routing rules, whether to charge on failure, and the `stream` parameter; supports regex rules and real-time testing against model names; changes take effect immediately on save without a restart
5. 📄 **Multi-Type Document Understanding** `V6.9.6`: Official models support uploading and recognizing PDF / Word / PPT / Excel / Text / Markdown / HTML files (for non-PDF files, a GPT-series model via the Responses endpoint is recommended); supports URL concatenation / Base64 inline / file link submission, automatically choosing the best option and falling back based on file size and token limits
6. 👀 **In-Dialogue File Preview** `V6.9.6`: View, print, and download PDF / Word / PPT / Excel / Text / Markdown / HTML files online; also supported in Coze Agent dialogues
7. 🖼️ **Multimodal Image Understanding**: Single / multiple image upload (up to 9 images), including photo upload from the native mobile camera or a PC webcam `V6.9.3`; adaptive multi-image layout in user messages `V6.9.6`; automatic preview of images returned by the API
8. 🤔 **Deep Thinking & Reasoning**: Supports reasoning models such as o3 / o4-mini and DeepSeek-R1, with streaming output and display of the reasoning chain (ReasoningContent / Think tags) and deep search progress
9. 🛜 **Web Search**: Models can be extended to search and summarize real-time web content (e.g. o4-mini-all: web search + reasoning + images + PDF analysis)
10. 🛡️ **Highly Reliable Dialogue Core** `V6.9.3`: Upstream (backend ↔ large model) and downstream (frontend ↔ backend) connections are decoupled, so switching sessions, closing the page, or exiting the client does not interrupt generation; SSE content is saved while generating and resumes when you switch back; "Stop answering" cancels the upstream request immediately; unified fallback for first-token timeouts / empty responses; multi-session concurrency isolation
11. 📌 **Dialogue Navigation Bar** `V6.9.5`: Appears automatically when the current dialogue group has ≥ 3 questions, with collapse, expand on hover, and click-to-locate
12. Ⓜ️ **Rich Content Rendering**: Markdown (code highlighting / LaTeX / KaTeX formulas / Mermaid / charts), mind map generation with PDF export, code file download, and message re-editing
13. 🗣️ **Voice Dialogue**: Supports OpenAI / Azure speech recognition and TTS (Whisper & TTS format relays), voice-in / voice-out replies, multiple voice options, and an admin switch for voice playback
14. 🏄‍♂️ **Plugin System & Open Integration**: Built-in plugin system (image recognition, document analysis, etc., continuously expanding); knowledge base or workflow apps compatible with the chat API (e.g. FastGPT knowledge bases / workflows) can be connected as models or bound to agents

### 🎨 2. Professional AI Painting
**Standalone Painting Modules & Model Support**

15. 🖌️ **Standalone GPT-Image-2 Painting Module** `V6.9.2` `V6.9.3`: Supports gpt-image-2, gpt-image-2.5, GPT-Image-2-Dev, and more, with custom API integration and extended model versions in the admin backend; text-to-image, reference image painting (up to 8 smart reference images), and online editing / brush-and-box editing of generated results; quality (low / medium / high / auto), quantity, aspect ratio, and custom resolution are submitted strictly within the official parameter ranges; supports per-user / system-wide concurrency limits
16. 🍌 **Standalone Nano Banana 2 Painting Module** `V6.9.4`: Supports gemini-3.1-flash-image and gemini-3-pro-image, with custom extended model versions (e.g. gemini-3.1-flash-lite-image); text-to-image, editing with multiple smart reference images, and custom resolution and aspect ratio (2K / 4K output depends on the model); Nano Banana models can also be used directly in AI dialogue
17. 🎨 **Midjourney / Niji Full Features**: Supports MJ V7 / V8 (V8 becomes available once the official API opens); Imagine / Upscale / Vary / Zoom Out / Pan, Vary Region inpainting, image blending, and combined use of standard / character-consistent (cref) / style-consistent (sref) reference images; Fast / Relax dual channels with separate billing and concurrency; real-time progress rendering
18. 🪄 **DALL·E 2 / 3 Painting**: All parameters supported
19. 🔁 **Common Painting Capabilities**: "Paint the Same" to reuse parameters in one click; dynamic display of points prices for each model and operation; automatic points refund on failure (idempotent, preventing duplicate refunds) `V6.9.6`; scheduled compensation tasks; private storage of original images + thumbnails; per-model frontend display switches; painting progress bar
20. 🖼️ **AI Gallery Plaza**: "Gallery Picks / My Paintings" tabs with separate loading `V6.9.5`; style categories, carousel, and creator center; hover to auto-preview video works
21. 🚥 **Painting Content Risk Control** `V6.9.3`: Prompts for GPT-Image / Midjourney / Niji / DALL·E are checked for sensitive words before submission — no upstream call, no charge — and violation records are synced to the admin backend

### 🎬 3. AI Video Generation
**Video Model Support**

22. 📽️ **VEO3 / VEO3.1 Video**: Supports VEO3.1, VEO3.1-fast, VEO3.1-pro, and more, with automatically generated audio (called via standard chat dialogue)
23. 📽️ **Sora-2 Video**: Supports Sora-2 video generation (called via standard chat dialogue)
24. 🎞️ **Midjourney HD Video** `V6.8.6`: Turn generated images into animations (high motion / low motion) in one click, with custom motion prompts, 1 / 2 / 4 videos per run, and separate billing configuration
25. 🎬 **Standalone AI Video Module**: Text-to-video / image-to-video (Pika), with a video works plaza
26. 🌱 **Seedance Video (Coze-Agent)**: Calls ByteDance's official Seedance model through the Coze-Agent "Seedance Video Generation" app, supporting first/last frames and videos with sound; results can be previewed and played directly in the system
27. 🔜 **Coming Soon**: Standalone image / video modules for Seedance2.5 video, Qwen-Image editing, Kling, and more (development plan for the second half of 2026)

### 🧠 4. AI Agents
**Agents & App Ecosystem**

28. 🤖 **Coze Agent Module**: Integrates Coze agents with plugins, workflows, functions, and knowledge bases; real-time streaming responses showing the thinking process and model / plugin / workflow call details; multiple concurrent conversations per agent; multi-file-type uploads with direct preview of image / video results
29. 📥 **Batch Agent Management**: One-click batch import and sync of agents from the Coze platform (Redis distributed lock prevents duplicates), with icons stored privately
30. 📈 **Agent Store**: Self-developed rating, activity, and popularity algorithms; suggested questions and keyword search; link sharing, WeChat QR code sharing, and poster sharing
31. 🧠 **GPTs & Preset Apps**: Search and add GPTs apps from across the web in one click; custom Prompt preset apps; user-created agents; apps can be bound to models, shared via link, or published to the plaza

### 💰 5. Membership Points & Commercial Operation
**Billing, Payments & Growth**

32. 🧑‍🤝‍🧑 **Membership Points System**: Multiple balances — regular model points, advanced model points, painting points, and Agent points; multiple billing methods such as per-use, time-based, and combo packages, with custom charges per model
33. 🧾 **Points Details System** `V6.9.6`: Consistent between the user end and admin backend, fully recording consumption, failure refunds, and failure exemptions for all model usage, with second-level timestamps and multi-dimensional filtering for reconciliation; the admin dialogue list shows the points consumed by each reply
34. 🆓 **Zero Charges on Failed Model Calls** `V6.9.6`: 4xx / 5xx errors, timeouts, and empty replies can be exempted from charges via a switch; failures / interruptions / empty replies go through a single settlement exit, eliminating incorrect and duplicate charges, with anti-abuse protection
35. 🛍️ **Payment System**: Official WeChat Pay (Native QR code on PC, JSAPI inside WeChat on mobile), EasyPay, CodePay, and HupiJiao Pay; synchronous order status checks, order search, and management
36. 🛒 **Store & Growth Tools**: Store with permanent / limited-time packages, check-in rewards, invitation rewards, redemption codes (batch generation and management), and guest mode
37. ⏏️ **Distribution System**: A + B distribution model with per-user commission settings; supports withdrawal thresholds and withdrawals via Alipay / WeChat / bank card
38. ✨ **Channel Load Balancing**: Self-developed channel load balancing and distribution algorithm, API key pool with multi-key polling (priority / weight / status management), and batch add / delete

### 🔐 6. Security & Risk Control
**Content Security & Account Security**

39. 🚥 **Content Risk Control**: Custom sensitive words + Baidu content moderation covering dialogue, painting, and mind maps, intercepted upfront on a hit; violation records and user snapshots are fully logged
40. 📍 **Login Device & Remote-Login Detection** `V6.9.6`: Records login IP (resolved to carrier and city/district), browser, operating system, and device type; users can view their last 5 login devices and online status in the personal center, also shown in the admin backend
41. 🔑 **Session Security**: Regular users can be online on only one device; super administrator sessions are separated by login IP, with logins from different locations forcing each other offline and recording the IP; supports forcing specified users offline from the admin backend `V6.9.4` and banning users
42. 🙈 **Sensitive Information Masking**: IPs and regions, configuration values, API addresses, keys, usernames, emails, etc. are masked for demo / non-super-admin accounts; the admin demo account is read-only
43. 📤 **Upload Security**: The server rejects script / code executables; when cloud storage is enabled, anonymous writes to the local disk are prohibited, and guest uploads are rate- and size-limited
44. 🧪 **"System Function Test" Switch** `V6.9.4`: When enabled, all AI generation requests are blocked at the system level without calling upstream APIs — suitable for going live before generative AI filing has been completed
45. 📧 **Registration Protection**: Email domain whitelist, optional blocking of "+" alias emails, disposable email filtering, and tamper-proof registration bonuses

### 🛠️ 7. Admin Backend & Site Operation
**Backend Management & Operation Settings**

46. 📊 **Data Dashboard**: User, dialogue, painting, and order statistics with 7-day trend charts, plus model usage counts and token usage pie charts
47. 💻 **Complete Admin Backend**: Manage users, orders, dialogues, paintings, videos, and more, with Excel export; query optimization for millions of records (concurrent count + Redis cache); login IP records in the user list `V6.9.6`
48. 🗂️ **Model & Key Pool Management**: Model categories, sorting, logos, and vendor groups, with pre-selected new-generation models by vendor `V6.9.6`; batch add / delete keys in the API key pool
49. 🎭 **Dialogue Demo Data** `V6.9.5`: Designate any dialogue groups (up to 5) as site-wide read-only demo content
50. ✔️ **Site Customization**: LOGO / site name / footer / Baidu statistics / copyright / ICP number / announcements / welcome messages / About Us / user agreement, etc. are all configurable in the backend; website live-stream entry `V6.9.2`
51. 🧩 **Dynamic Menus & Carousel**: Embedded web pages, external links, internal path navigation, custom icons, and separate PC / mobile settings; carousel for ads / events / tutorials
52. ♻️ **WeChat Official Account Integration**: Official account login and keyword auto-replies
53. 🔐 **Permission System**: Tiered permissions for super administrators and demo accounts

### 🌏 8. Multi-Platform Experience & System Architecture
**Experience, Performance & Deployment**

54. 🌐 **Full System Internationalization** `V6.9.1`: Full i18n of the frontend UI + backend configuration + backend responses, switching automatically by visitor IP and browser language; one-click AI translation of admin configuration content, ready for overseas operation
55. 🎨 **Dual-Style UI** `V6.9.0`: Users can switch freely between card style and Notion style; AI dialogue immersion mode, "Add Menu" collection, liquid-glass buttons, and automatic light/dark theme
56. 📲 **Multi-Platform Support**: PC + mobile H5 + WeChat official account, adapting to PC / mobile / tablet; PWA support, and H5 can be packaged for other platforms
57. ⚡ **Performance Optimization** `V6.9.5`: Chinese font subsetting (single font weight 4.2MB → 0.9MB), about 50% less single-page resource download, and batched resource loading on mobile, reducing crash risk on low-memory devices such as iOS
58. 🚀 **High-Concurrency Server**: Node.js + NestJS server with Redis caching and an adaptive MySQL connection pool, suited to high-concurrency business scenarios
59. 🗄️ **Storage & Data Sync**: Local storage / Alibaba Cloud OSS / Tencent Cloud COS / Chevereto image hosting, with private storage of user files and painting data; dialogue session isolation, cloud storage, and data sync across devices
60. 🖥️ **Deployment**: Supports regular Baota panel deployment and Docker one-click deployment, with all integration settings completed in the admin interface; suitable for commercial operation, internal enterprise use, education and training, and more
61. 🏅 **Continuous Updates**: The system has been continuously iterated for three and a half years, and more AI capabilities are in development...

<h2 id="readme-compare">📊 Public Good Free Commercial Edition vs Commercial License Version</h2>

Public Good Free Commercial Edition (Public Good V2.1.0 · 2026 Special Public-Good Rebuild, with membership packages, online payment, distribution, and other commercial features) repository: <a href="https://github.com/nosqlnull/SparkAi-ChatGPT-AiWeb" target="_blank" rel="noopener noreferrer">SparkAi-ChatGPT-AiWeb</a>

| Feature | Public Good Free Commercial Edition (Public Good V2.1.0) | Commercial License Version (V6.9.6) |
|---|---|---|
| Scope of use | ✅ Commercial operation supported | ✅ Commercial operation supported |
| Version iteration | 2026 Special Public-Good Rebuild (V3.2.0 feature base), with some feature updates | ✅ Continuous major updates |
| AI models | ✅ GPT-3.5 / GPT-4.0, Azure, and some domestic models<br>🔜 Coming soon: GPT-6, Claude-Opus-5-5 / Claude-Fable-5-1, Gemini, DeepSeek, and all other models (expected 2026.10) | ✅ GPT-6, Claude-Opus-5-5 / Claude-Fable-5-1, Gemini, DeepSeek, and all other models |
| Custom integration of the latest models in the backend (no system update needed) | 🔜 Coming soon (GitHub update pending, expected 2026.10) | ✅ |
| Dual-endpoint routing / model global configuration center | ❌ | ✅ |
| Deep reasoning (o3 / DeepSeek-R1, etc.) | ❌ | ✅ |
| Multi-image understanding / multi-type document understanding and online preview | ❌ | ✅ |
| DALL·E painting | ✅ DALL·E 2 / 3 | ✅ DALL·E 2 / 3 |
| Midjourney painting | ✅ Text-to-image, image-to-image, partial repainting | ✅ Full features: V7 / V8, Niji, character / style reference images, HD video |
| Standalone GPT-Image-2 / Nano Banana 2 painting modules | ❌ | ✅ |
| AI video generation (VEO3.1 / Sora-2 / Pika / Seedance) | ❌ | ✅ |
| AI agents | ✅ Custom Prompt preset apps | ✅ Plus Coze Agent, GPTs apps, and agent store |
| Registration and login | ✅ WeChat QR code / email / mobile number | ✅ Plus login device and remote-login detection |
| Redemption codes | ✅ | ✅ |
| Membership packages | ✅ Permanent / limited-time membership packages | ✅ Multiple points balances; permanent / limited-time / combo packages; custom pricing per model |
| Payment system | ✅ EasyPay / CodePay / HupiJiao Pay | ✅ WeChat Pay / EasyPay / CodePay / HupiJiao Pay |
| Distribution | ✅ Referral invitations, commission withdrawals | ✅ A + B distribution, per-user commission rates, withdrawal thresholds |
| Points details / zero charge on failed model calls | ❌ | ✅ |
| Enhanced risk control (sensitive info masking, "System Function Test" switch, etc.) | ❌ | ✅ |
| Full system internationalization | ❌ | ✅ |
| 2026 new UI (card / Notion dual styles, immersion mode) | ❌ | ✅ |
| Complete commercial admin backend | Basic management | ✅ Data dashboard, model and key pools, dynamic menus, global configuration |

<h2 id="readme-preview">🖼️ Screenshots</h2>

> Screenshots match the <a href="https://bx5gkpqv57j.feishu.cn/docx/EOWUdQ04no9PoBxyp6Ecg3AAnhf" target="_blank" rel="noopener noreferrer">commercial system introduction (Feishu)</a> and may lag behind the latest release; see the <a href="https://test.sparkaigc.com" target="_blank" rel="noopener noreferrer">live demo</a> for the actual experience.

### 💻 PC (partial)

#### User registration & login

Silent login inside WeChat, WeChat QR-code login in the browser, email and mobile-number registration. Since `V6.9.1`, a brand-new animated login page built from scratch with native CSS + Vue 3 Composition API.

<p align="center">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-login-1.jpg" alt="User registration & login" width="49%">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-login-2.jpg" alt="User registration & login" width="49%">
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-login-3.jpg" alt="User registration & login" width="49%">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-login-4.jpg" alt="User registration & login" width="49%">
</p>

#### Multi-language internationalization

Full internationalization: not only fixed front-end text, but also back-end configuration and back-end responses.

![Multi-language internationalization](https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-i18n.jpg)

#### AI model chat

Supports all OpenAI, Gemini and Claude models, plus domestic and third-party mainstream models (any standard Chat-format API).

![AI model chat](https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-chat.jpg)

#### AI agent apps

GPTs apps + custom Prompt preset apps; GPTs can be added in the admin panel or searched site-wide (same as the official search).

![AI agent apps](https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-agent.jpg)

#### User-created preset agents

Agent workbench with continuous context.

<p align="center">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-agent-custom-1.jpg" alt="User-created preset agents" width="49%">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-agent-custom-2.jpg" alt="User-created preset agents" width="49%">
</p>

#### Full-featured Midjourney painting

Real-time rendering of painting progress.

<p align="center">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-mj-1.jpg" alt="Full-featured Midjourney painting" width="49%">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-mj-2.jpg" alt="Full-featured Midjourney painting" width="49%">
</p>

#### Reference-image generation

Normal, character-consistent and style-consistent reference images, used alone or combined; upload preview, image type and reference index display.

![Reference-image generation](https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-mj-reference.jpg)

#### Vary Region inpainting

![Vary Region inpainting](https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-mj-vary-region.jpg)

#### Image blending

![Image blending](https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-mj-blend.jpg)

#### DALL·E painting

![DALL·E painting](https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-dalle.jpg)

#### Midjourney HD video

Brand-new Midjourney HD video creation (since `V6.8.6`).

![Midjourney HD video](https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-mj-video-1.jpg)

<p align="center">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-mj-video-2.jpg" alt="Midjourney HD video" width="49%">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-mj-video-3.jpg" alt="Midjourney HD video" width="49%">
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-mj-video-4.jpg" alt="Midjourney HD video" width="49%">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-mj-video-5.jpg" alt="Midjourney HD video" width="49%">
</p>

#### AI gallery square

Includes creator features.

![AI gallery square](https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-gallery-1.jpg)

<p align="center">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-gallery-2.jpg" alt="AI gallery square" width="49%">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-gallery-3.jpg" alt="AI gallery square" width="49%">
</p>

#### AI video generation / video square

Text-to-video and image-to-video.

![AI video generation / video square](https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-video.jpg)

#### Membership package store

Time-limited and permanent packages defined in the admin panel, freely combinable.

<p align="center">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-shop-1.jpg" alt="Membership package store" width="49%">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-shop-2.jpg" alt="Membership package store" width="49%">
</p>

#### Distribution & referral

<p align="center">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-distribution-1.jpg" alt="Distribution & referral" width="49%">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pc-distribution-2.jpg" alt="Distribution & referral" width="49%">
</p>

### 📱 Mobile H5 (partial)

<p align="center">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/h5-01.jpg" alt="Mobile H5" width="32%">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/h5-02.jpg" alt="Mobile H5" width="32%">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/h5-03.jpg" alt="Mobile H5" width="32%">
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/h5-04.jpg" alt="Mobile H5" width="32%">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/h5-05.jpg" alt="Mobile H5" width="32%">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/h5-06.jpg" alt="Mobile H5" width="32%">
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/h5-07.jpg" alt="Mobile H5" width="32%">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/h5-08.jpg" alt="Mobile H5" width="32%">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/h5-09.jpg" alt="Mobile H5" width="32%">
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/h5-10.jpg" alt="Mobile H5" width="32%">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/h5-11.jpg" alt="Mobile H5" width="32%">
</p>

Visit the <a href="https://test.sparkaigc.com" target="_blank" rel="noopener noreferrer">live demo</a> for more.

### 💳 Official WeChat Pay

Supports official WeChat Pay, EasyPay, CodePay, HupiJiao and more, with order status sync, order search and management.

With official WeChat Pay enabled, PC uses Native pay (QR code generated directly):

![WeChat Native pay on PC](https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pay-pc-native.jpg)

Inside the WeChat app, JSAPI pay is used (the WeChat wallet opens directly):

<p align="center">
  <img src="https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/v6/pay-h5-jsapi.jpg" alt="WeChat JSAPI pay on mobile" width="32%">
</p>

### 🛠️ Admin panel

See the <a href="https://test.sparkaigc.com/sparkai/admin" target="_blank" rel="noopener noreferrer">live demo admin panel</a> (test account `admin` / `123456`).

<h2 id="readme-tech">🧱 Architecture & Deployment Environment</h2>

### ✨System Technical Architecture
**System Architecture**

- Front-end: Vite + Vue3 + TypeScript + NaiveUI + TailwindCSS
- Management end: Vite4 + Vue3 + Element-Plus
- Back-end: Node.js + NestJS
- Data support: MySQL5.7(+) / MySQL8 + Redis
- Operating environment: Linux, Windows, macOS (Linux is recommended)
- Data storage: local storage | object storage Alibaba Cloud OSS | object storage Tencent Cloud COS | Chevereto image hosting

### 🛠️Operating Environment
**Operating Environment**

- Linux (recommended)
- Windows
- MacOS Server
- Docker
- Kubernetes
- Supports ARM64 & X86 (32/64) architecture

### 🎯Server Configuration Requirements
**Minimum server configuration requirements are 1C1G (actual memory usage < 500M), and 2C4G or above is recommended for high concurrency.**

<h2 id="readme-license">🛒 Commercial License (Private Independent Deployment)</h2>

The private deployment version is mainly for webmasters and companies planning to build an AI platform. It delivers encrypted source code for the user end | admin end | back end (closed source) + an authorization code.

- 📗 Commercial License introduction: <a href="https://docs.sparkaigc.com/en/pro/" target="_blank" rel="noopener noreferrer">https://docs.sparkaigc.com/en/pro/</a>
- 🗂️ Commercial system introduction and pricing (Feishu): <a href="https://bx5gkpqv57j.feishu.cn/docx/EOWUdQ04no9PoBxyp6Ecg3AAnhf" target="_blank" rel="noopener noreferrer">View</a>
- 🧭 Deployment tutorial: <a href="https://docs.sparkaigc.com/en/deploy/baota/process.html" target="_blank" rel="noopener noreferrer">https://docs.sparkaigc.com/en/deploy/baota/process.html</a>
- 💬 Author WeChat: `DjiMain` · Author QQ: `501439094` (please note `SparkAi` when adding)

![](https://raw.githubusercontent.com/nosqlnull/ChatGPT-SparkAi/main/SystemPreview/Wechat.png)

<h2 id="readme-star-history">⭐ Star History</h2>

<div align="center">

<a href="https://star-history.com/#nosqlnull/ChatGPT-SparkAi&Date" target="_blank" rel="noopener noreferrer">![Star History Chart](https://api.star-history.com/svg?repos=nosqlnull/ChatGPT-SparkAi&type=Date)</a>

</div>

<h2 id="readme-agpl">📜 License</h2>

The public content of this repository (project documentation, system screenshots, etc.) is licensed under the [GNU Affero General Public License v3.0 (AGPLv3)](../../LICENSE).

The SparkAi Commercial License Version (user client / admin console / server) is not included in this repository and is not covered by the license above. A usage license must be obtained through the <a href="https://docs.sparkaigc.com/en/pro/" target="_blank" rel="noopener noreferrer">official Commercial License</a>.

If your organization's policy does not allow AGPLv3-licensed content, or you wish to avoid the open-source obligations of AGPLv3, please email [evenkepler@gmail.com](mailto:evenkepler@gmail.com) or add the author on WeChat: `DjiMain` (note `SparkAi`).
