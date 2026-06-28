# 前情提要 · SKZJ 新窗口（CODEX 执行：001水杯 逐卡落盘）

> 贴进 SKZJ/CODEX 新窗口开场用。你是 CODEX——执行代理，**所有落盘与 git 在你这**。本窗任务：接 SK 出的逐卡推敲工单，落盘 + 补引擎层 + 接资产 + 回执。看板是状态权威，开场先读盘核对。

## 开场动作（先做）
- 确认可达 `D:\KAIROS第一人称自传\SKZJ`（远程 github.com/MRYGP/SKZJ）与 `D:\sk`。
- 读 `AGENTS.md`（你的执行规则）+ `D:\sk\ops\项目看板\KAIROS项目看板.md`（状态权威）。
- **读盘才断言**：落盘前先读现行文件，禁凭记忆或路径名脑补。

## 当前态（commit 14f5501 第一可跑版已落；2026-06-25 已同步停顿〇 v1.3 + 第三幕 v1.4）
- `副本-杨2011决断\h5\index.html` ＝ v1.1 第一可跑版骨架：卡1-22 + card-15b；停顿〇已改为两身体声音触发键（点任一键→交替二次→卡住→卡11；无反馈、不判对错）；第三幕卡16-20已同步为 v1.5 七卡决策链；音频引擎 `bedAudio/bgmAudio/activeAudio(旁白)/silent` + `unlockAudio()` 微信解锁 + pause/resume 同步全层；每卡 `bg` 走 CSS 渐变 class；卡22 止（无第二阶段）。
- 卡21：`type:photo` + `audio: assets/audio/card21-mother-20260620.m4a`（未剪母本占位）+ `img: assets/img/card21-placeholder.png`，`fixed:90000`（降级时长占位）。
- 占位资产路径：`assets/audio/bed-fan-placeholder.m4a`、`bed-street-placeholder.m4a`、`bgm-warm-placeholder.m4a`、`card21-mother-20260620.m4a`；`assets/img/card21-placeholder.png`。
- 旧版备份 `h5\index-v0.9.html`；spec 在仓：`H5-v1.1技术员指导与CODEX工单.md`（顶有覆盖横幅）、`H5-v1.1实现补充工单.md`。

## 你要落的（接 SK 工单，按落盘靶）
| SK 推敲卡格 | 落到 |
|---|---|
| 画面 prompt/排版 | `h5\assets\出图记录.md` → 重生成 **v1.1**（现停 v0.6/29卡） |
| 声音 + 旁白 | `h5\assets\配音稿.md` → 重生成 **v1.1**（现停 v0.6，头部自标须重做） |
| 时长/停顿 | `index.html` 的 `cards` 数组 |
| 判真锁状态 | `制作清单-v1.1.md` 新开"判真锁账本"一节（常驻可审） |

## 要补的引擎层（SK 工单触到就做，否则资产放不出）
1. **sfx 一次性音效层**：现在只有 bed 连续底噪。加卡级 `sfx[]` 叠播（进卡播一次、不循环），供收摊/开工三重奏、QQ滴滴、卡18单音、卡19笔尖、卡20纸币脆响。
2. **bg 真图层**：现在 `bg` 是 CSS 渐变。加图片底图层（full-bleed + 暗角/渐变保字），**缺图回退渐变**。
3. **卡2-20 旁白接入**：引擎已支持每卡 `audio`（卡21在用）；SK 给 TTS 后加 `audio` 路径即接。
4. **bed 无缝循环**：先 `<audio loop>`，真机听接缝；咔哒才给 bed 单独上 Web Audio（**不预建整套**）。
5. **卡21 精剪后**：`fixed` 从 90000 改实际时长。

## 纪律
- **回执三段式**：做了什么/没做什么及原因/commit 号。关键声明可被抽查读盘，回执≠事实。
- 工单零上下文可执行才动手；不自执行"建议"、不改判断层、不写系统指令。
- 文件名与工单声明一致（避免 v0.9/v1.1 那类不一致）；升版三查（旧版横幅/全仓旧指针 grep/README+前情提要清单行）。
- 落盘范围：**这版只到正片卡1-22**；不做 MediaRecorder/共塑金句/评论区/动态视频。

## 路径
主仓 `D:\KAIROS第一人称自传\SKZJ\`；运营仓 `D:\sk\`（看板/工单）。流程详见《001水杯·逐卡打磨执行步骤》。
