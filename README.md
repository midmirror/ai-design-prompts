# AI 生图提示词精选 · 产品设计 / UX 设计向

从 X（Twitter）近一年（2025-10-28 至 2026-10-28）的设计类内容里筛出的 **59 条提示词/方法论案例 + 125 张效果图**，按设计工作场景分 8 类。

## 目录结构

```
ai-design-prompts/
├── README.md                 ← 本文件，全部案例索引
├── 01-app-ui/                ← 每类一个文件夹：<作者>-<点赞数>.md + images/
├── 02-wireframe-to-hifi/
├── 03-web-landing/
├── 04-brand-logo/
├── 05-icon-illustration/
├── 06-infographic-ppt/
├── 07-method-workflow/
├── 08-product-render/
└── data/
    ├── selected.json         ← 精选案例的元数据
    └── tweets-raw.json       ← 原始候选池 410 条（可自行再挖）
```

每个 `.md` 卡片包含：作者与原帖链接、发布时的赞/浏览数、所用模型、提示词原文（代码块内可直接复制）、效果图。

## 怎么用

1. **先读 07-method-workflow**。那一类讲的是"为什么 AI 出的图一眼假"，看完再抄具体提示词，命中率高很多。
2. 抄提示词时替换方括号/中文书名号里的变量（城市名、品牌名、产品名），其余结构别动——这些提示词的价值在骨架，不在形容词。
3. 同一提示词至少换 3 次风格词（写实/等距/手绘）再判断好坏，单次出图不代表提示词质量。
4. 卡片里除了「原文」，还有一节「作者补充的提示词」——原帖正文写不下时，作者会把完整提示词发在自己评论区，这个工具已经自动抓回来了（近半数案例有）。标「配图内文字」的才是真需要看图抄的。

## 分类索引

### 01-app-ui　`App / 移动端界面与组件`

把「界面」当成一种构图来写提示词：先锁定画幅与视角（如 9:16 竖版、45° 俯视），再定义组件层级（顶部图标、日期、温度、城市名），最后指定素材质感（PBR / 拟物 / 玻璃）。

| 案例 | 作者 | 日期 | 赞 | 模型 | 提示词位置 | 图 |
|---|---|---|---|---|---|---|
| [nano banana pro prompt (with gemini)](01-app-ui/dotey-2551.md) | @dotey | 2025-11-26 | 2551 | Nano Banana Pro | 推文正文 | 4 |
| [Nano Banana Pro 提示词](01-app-ui/op7418-529.md) | @op7418 | 2025-11-27 | 529 | Nano Banana Pro | 推文正文 | 1 |
| [nano banana prompt](01-app-ui/dotey-411.md) | @dotey | 2025-12-01 | 411 | Nano Banana Pro | 推文正文 | 1 |
| [天呐，gpt-6 astra 真的可以操作 Figma 设计 UI 了！](01-app-ui/LinearUncle-337.md) | @LinearUncle | 2026-09-06 | 337 | GPT-6 | 推文正文 | 3 |
| [Opus 5.5 生成 svg 的效率实在太高，让他给  生成了一组以 UI 线框为主体](01-app-ui/Kubai087-218.md) | @Kubai087 | 2026-10-24 | 218 | Opus 5.5 / Claude | 推文正文 | 1 |
| [I used @givros his awesome prompt to get thi](01-app-ui/bas_fijneman-72.md) | @bas_fijneman | 2026-05-04 | 72 | GPT Image 2 | 推文正文 | 4 |
| [GPT image 2.5](01-app-ui/Naiknelofar788-33.md) | @Naiknelofar788 | 2026-10-25 | 33 | GPT Image 2 | 推文正文 | 2 |
| [一个 6B 的国产开源图片模型，一出来就登顶 AA UI/UX Design 开源第一。](01-app-ui/sven_ai-9.md) | @sven_ai | 2026-10-04 | 9 | 未标注 | 推文正文 | 3 |

### 02-wireframe-to-hifi　`低保真原型 → 高保真设计稿`

这一类的价值不在"生成一张好看的图"，而在把已有结构（线框、草图、竞品截图）当作输入，让模型只负责风格与细节。适合在提案阶段把低保真快速抬成可评审稿。

| 案例 | 作者 | 日期 | 赞 | 模型 | 提示词位置 | 图 |
|---|---|---|---|---|---|---|
| [3 cases of using Nano Banana Pro for Product](02-wireframe-to-hifi/101babich-202.md) | @101babich | 2025-11-21 | 202 | Nano Banana Pro | 推文正文 | 4 |
| [哇！这执行准确度！](02-wireframe-to-hifi/ZHO_ZHO_ZHO-63.md) | @ZHO_ZHO_ZHO | 2025-11-26 | 63 | Nano Banana Pro | 正文只提到提示词（原文在配图/评论） | 1 |
| [很多人以为 GPT-Image-2 最厉害的，是“从零画一张图”。](02-wireframe-to-hifi/derek_wall90176-47.md) | @derek_wall90176 | 2026-07-08 | 47 | GPT Image 2 | 推文正文 | 4 |
| [I literally designed the landing page for a ](02-wireframe-to-hifi/WoCStreet-5.md) | @WoCStreet | 2026-01-05 | 5 | Nano Banana | 推文正文 | 1 |

### 03-web-landing　`网页 / 落地页 / 官网`

网页类提示词要同时约束四件事：布局骨架（hero / 功能区 / 页脚）、视觉风格命名（报纸风、包豪斯、Glassmorphism）、字体与配色规则、以及"不要什么"（避免 AI 味的紫渐变 + 圆角卡片）。

| 案例 | 作者 | 日期 | 赞 | 模型 | 提示词位置 | 图 |
|---|---|---|---|---|---|---|
| [how to improve GPT-6 Astra / Codex's ability](03-web-landing/shannholmberg-860.md) | @shannholmberg | 2026-09-21 | 860 | GPT Image / GPT-6 | 推文正文 | 1 |
| [发现一个设计神器！](03-web-landing/ttmouse-348.md) | @ttmouse | 2025-12-15 | 348 | 未标注 | 推文正文 | 1 |
| [Usei o mesmo processo pra criar essa landing](03-web-landing/brunobertolini-188.md) | @brunobertolini | 2026-03-27 | 188 | Nano Banana | 推文正文 | 1 |
| [宝藏网站，专门做 AI 设计风格提示词的](03-web-landing/ianneo_ai-141.md) | @ianneo_ai | 2026-03-26 | 141 | 未标注 | 推文正文 | 4 |
| [让 AI 做个页面，经常是同一套模样，渐变紫、居中大标题、三张圆角卡片，一眼就能认出是 ](03-web-landing/GitHub_Daily-61.md) | @GitHub_Daily | 2026-10-06 | 61 | 未标注 | 配图内文字（正文没写，需看图抄） | 1 |

### 04-brand-logo　`Logo · 品牌识别 · VI`

品牌类提示词普遍带一个"上传参考图 → 输出系统"的 trigger：给一个 Logo，让模型外延出 VI 板、名片、包装、社媒模板。学习重点是"从单点标识生成整套识别系统"这一套写法。

| 案例 | 作者 | 日期 | 赞 | 模型 | 提示词位置 | 图 |
|---|---|---|---|---|---|---|
| [目前看到的最猛 AI Logo 工具「Rikyu」。](04-brand-logo/awe0_io-7877.md) | @awe0_io | 2026-10-27 | 7877 | GPT Image / Midjourney | 配图内文字（正文没写，需看图抄） | 4 |
| [这个 Skill 一出，Logo设计师可以下岗了！](04-brand-logo/0xAllen-1827.md) | @0xAllen | 2026-03-03 | 1827 | 未标注 | 配图内文字（正文没写，需看图抄） | 1 |
| [GPT Image 2](04-brand-logo/Just_sharon7-1198.md) | @Just_sharon7 | 2026-05-02 | 1198 | GPT Image 2 | 推文正文 | 1 |
| [nano banana pro prompt](04-brand-logo/dotey-1026.md) | @dotey | 2025-12-03 | 1026 | Nano Banana Pro | 推文正文 | 4 |
| [真是挖到宝了！！](04-brand-logo/yyyole-448.md) | @yyyole | 2026-10-10 | 448 | 未标注 | 推文正文 | 1 |
| [Bold visuals. Clean design. Stories that sta](04-brand-logo/Naiknelofar788-424.md) | @Naiknelofar788 | 2026-05-02 | 424 | GPT Image 2 | 推文正文 | 2 |
| [Nano Banana branding prompt:](04-brand-logo/AmirMushich-257.md) | @AmirMushich | 2026-03-05 | 257 | Nano Banana | 正文只提到提示词（原文在配图/评论） | 1 |
| [我一直觉得用 AI 画 Logo 最大的毛病是画得太满，细节一多，缩成 App 图标就糊](04-brand-logo/GitHub_Daily-106.md) | @GitHub_Daily | 2026-09-26 | 106 | Nano Banana Pro / GPT Image 2 | 配图内文字（正文没写，需看图抄） | 1 |

### 05-icon-illustration　`图标与插画`

图标提示词的关键是约束几何复杂度：形状数量、主色数量、线条删减规则。写得越"少"，缩到 24px 越不糊。

| 案例 | 作者 | 日期 | 赞 | 模型 | 提示词位置 | 图 |
|---|---|---|---|---|---|---|
| [Opus 5.5 让你实现 App Icon 设计自由](05-icon-illustration/dotey-685.md) | @dotey | 2026-09-27 | 685 | Opus 5.5 / Claude | 推文正文 | 4 |
| [据说把这张图喂给 AI，然后使用下面的提示词，你将得到一个有高级感的 app 图标。](05-icon-illustration/LuoSays-151.md) | @LuoSays | 2026-05-20 | 151 | 未标注 | 正文只提到提示词（原文在配图/评论） | 1 |
| [不求设计师！Codex一句话生成App图标，加快项目开发速度。](05-icon-illustration/vista8-134.md) | @vista8 | 2026-06-21 | 134 | 未标注 | 配图内文字（正文没写，需看图抄） | 1 |
| [哈哈哈，都被Spotify 的迪斯科Logo晃瞎眼了。](05-icon-illustration/vista8-53.md) | @vista8 | 2026-05-18 | 53 | GPT Image 2 / Kling | 推文正文 | 4 |
| [一整篇文章丢过去，让Codex或ChatGPT生图解读。](05-icon-illustration/vista8-49.md) | @vista8 | 2026-07-04 | 49 | 未标注 | 正文只提到提示词（原文在配图/评论） | 1 |

### 06-infographic-ppt　`信息图 · 图表 · PPT/幻灯片`

信息图/PPT 类提示词几乎都会显式声明"文字必须可读、可改"，并给出画幅、背景材质、信息层级。中文科技封面那类会长篇定义编辑人格（"你是一名顶级科技媒体视觉设计师"）。

| 案例 | 作者 | 日期 | 赞 | 模型 | 提示词位置 | 图 |
|---|---|---|---|---|---|---|
| [预订本年度最有价值提示词 —— 生成既有质感，又能随意修改文字的完美 PPT](06-infographic-ppt/dotey-2000.md) | @dotey | 2025-12-21 | 2000 | 未标注 | 正文只提到提示词（原文在配图/评论） | 1 |
| [nano banana pro prompt](06-infographic-ppt/dotey-1283.md) | @dotey | 2025-12-03 | 1283 | Nano Banana Pro | 推文正文 | 4 |
| [Nano Banana Pro PPT 生成提示词](06-infographic-ppt/op7418-947.md) | @op7418 | 2025-11-29 | 947 | Nano Banana Pro | 推文正文 | 1 |
| [nano banana pro prompt](06-infographic-ppt/dotey-689.md) | @dotey | 2025-11-26 | 689 | Nano Banana Pro | 推文正文 | 1 |
| [找到了一种非常喜欢的nano banana pro玩法：用等角透视像素画风格打造某一领域](06-infographic-ppt/sundyme-607.md) | @sundyme | 2025-11-29 | 607 | Nano Banana Pro | 正文只提到提示词（原文在配图/评论） | 1 |
| [一个提示词修复Notebooklm幻灯片中文字体崩坏。](06-infographic-ppt/sundyme-465.md) | @sundyme | 2025-12-20 | 465 | 未标注 | 推文正文 | 2 |
| [nano banana pro 的知识漫画 太牛了！！！](06-infographic-ppt/howie_serious-442.md) | @howie_serious | 2025-11-28 | 442 | Nano Banana Pro | 推文正文 | 4 |
| [nano banana pro prompt](06-infographic-ppt/dotey-286.md) | @dotey | 2025-12-03 | 286 | Nano Banana Pro | 推文正文 | 1 |
| [GPT Image 2 Prompt：中文科技新闻爆款封面生成器](06-infographic-ppt/dotey-227.md) | @dotey | 2026-05-09 | 227 | GPT Image 2 | 推文正文 | 4 |
| [GPT Image 2 Prompt：one-page hand-drawn educa](06-infographic-ppt/dotey-158.md) | @dotey | 2026-04-24 | 158 | GPT Image 2 | 推文正文 | 1 |

### 07-method-workflow　`设计提示词方法论与工作流`

这一类不是可直接复制的提示词，而是"怎么让 AI 做出不像 AI 的设计"的方法论：设计系统文件（DESIGN.md）、风格先选后做、反 AI 味清单、提示词写法原则。值得先读完再看前面几类的具体提示词。

| 案例 | 作者 | 日期 | 赞 | 模型 | 提示词位置 | 图 |
|---|---|---|---|---|---|---|
| [之所以研究 Claude Design，是因为最近摸索出一套不错的开发模式：](07-method-workflow/dotey-943.md) | @dotey | 2026-06-07 | 943 | 未标注 | 推文正文 | 4 |
| [分享 10 条优化界面 UI 的提示词，其中一些可能带有个人经验，发送给你的 Codex](07-method-workflow/ZaynHao-932.md) | @ZaynHao | 2026-10-23 | 932 | 未标注 | 推文正文 | 2 |
| [90% of apps look vibe coded:](07-method-workflow/Hartdrawss-604.md) | @Hartdrawss | 2026-02-28 | 604 | Midjourney / Flux | 推文正文 | 1 |
| [我去，著名产品人Lenny这篇文章的含金量太高了！](07-method-workflow/vista8-500.md) | @vista8 | 2026-09-04 | 500 | 未标注 | 正文只提到提示词（原文在配图/评论） | 1 |
| [The 2 ways I actually use AI in my design pr](07-method-workflow/poistudioltd-398.md) | @poistudioltd | 2026-08-08 | 398 | Midjourney | 推文正文 | 4 |
| [A good agent can still give you a bad logo. ](07-method-workflow/Sonofpeace0001-273.md) | @Sonofpeace0001 | 2026-10-22 | 273 | 未标注 | 推文正文 | 1 |
| [前端 UI 设计怎么避免"AI 味" ？](07-method-workflow/shao__meng-247.md) | @shao__meng | 2026-08-24 | 247 | 未标注 | 推文正文（方法论长文） | 1 |
| [跟 Claude 学习怎么写 Prompt 来提升 UI 设计质量](07-method-workflow/shao__meng-191.md) | @shao__meng | 2025-11-23 | 191 | 未标注 | 推文正文 | 1 |
| [对抗 AI 设计 Slop：来自前 Figma 工程师的七条方法论](07-method-workflow/shao__meng-129.md) | @shao__meng | 2026-08-27 | 129 | 未标注 | 推文正文 | 1 |
| [Awesome Claude Design](07-method-workflow/shao__meng-125.md) | @shao__meng | 2026-04-19 | 125 | 未标注 | 推文正文 | 1 |
| [前端设计 Skills 分享] Impeccable  66K 🌟](07-method-workflow/shao__meng-25.md) | @shao__meng | 2026-09-07 | 25 | 未标注 | 推文正文 | 1 |
| [95% of developers using AI for frontend are ](07-method-workflow/0xPixelMind-0.md) | @0xPixelMind | 2026-10-24 | 0 | 未标注 | 推文正文 | 1 |

### 08-product-render　`产品渲染 · 包装 · Mockup`

产品渲染/包装类提示词重在摄影语言：镜头、光比、材质、场景道具、品牌植入位置。也常用于把一个产品的概念快速可视化，用于内部对齐。

| 案例 | 作者 | 日期 | 赞 | 模型 | 提示词位置 | 图 |
|---|---|---|---|---|---|---|
| [nano banana prompt](08-product-render/dotey-2331.md) | @dotey | 2025-11-30 | 2331 | Nano Banana Pro | 推文正文 | 4 |
| [nano banana pro Prompt](08-product-render/dotey-856.md) | @dotey | 2025-12-07 | 856 | Nano Banana Pro | 推文正文 | 4 |
| [new TREND in Nano Banana Pro](08-product-render/gudanglifehack-729.md) | @gudanglifehack | 2026-03-29 | 729 | Nano Banana Pro | 正文只提到提示词（原文在配图/评论） | 4 |
| [Nano Banana smart prompt:](08-product-render/AmirMushich-141.md) | @AmirMushich | 2026-03-13 | 141 | Nano Banana | 正文只提到提示词（原文在配图/评论） | 1 |
| [Nano Banana 2 on Gemini](08-product-render/Sheldon056-102.md) | @Sheldon056 | 2026-07-08 | 102 | Nano Banana 2 | 推文正文 | 4 |
| [Gemini nano banana 2](08-product-render/Goodmanprotocol-79.md) | @Goodmanprotocol | 2026-03-31 | 79 | Nano Banana 2 | 推文正文 | 2 |
| [AI绘画每日一词】品牌视觉套件](08-product-render/derek_wall90176-62.md) | @derek_wall90176 | 2026-07-05 | 62 | 未标注 | 推文正文 | 4 |

## 采集口径（可复现）

- 工具：`x` / twitter-cli（`twitter search`），走直连，无代理。
- 时间窗：`--since 2025-10-28`，抓取日 2026-10-28。
- 查询词 24 条：nano banana prompt UI design / app design / landing page / wireframe / design system / UX / mobile app screen / packaging / icon set / moodboard / user persona journey map / GPT image prompt UI design / AI prompt logo design / AI image prompt dashboard design / AI 生图 提示词 UI 设计 / nano banana 提示词 设计 / AI 提示词 界面设计 / AI 生图 提示词 产品设计 / nano banana prompt icon / AI icon set prompt design / app icon prompt nano banana / 图标 提示词 AI 生成 / prompt generate icon set design / AI 生成 icon 提示词 设计 / nano banana prompt mobile app screen / 等。
- 粗筛：24 次查询去重后 533 条 → 带图 531 条 → 命中设计语义并去重成候选池 410 条 → 人工挑选 59 条。
- 排除：成人内容关键词（nsfw/porn/nude/…）在粗筛阶段剔除；同时剔除二次元手办、人物写真、食物摄影等与产品/UX 设计无关的类别（原始池里仍保留，可自行查看 `data/tweets-raw.json`）。
- 排序依据：点赞数为主，兼顾"正文是否直接给出可复制提示词"。

> 说明：赞数与浏览数是抓取时的快照，会随时间变化。提示词与效果图的版权归各原作者，本仓库仅做整理、翻译与索引，署名与删除政策见 [NOTICE.md](NOTICE.md)。

## 许可

本仓库的整理、翻译、索引部分以 [CC BY 4.0](LICENSE) 授权；收录的提示词原文与效果图版权归各原作者。转载卡片内容时请保留作者与原帖链接。
