# 方法来源与整合取舍

核对日期：2026-11-04。以下为方法参考链接，不是运行依赖。仓库今后可能变化。本技能的正文与示例为独立综合写作；没有把第三方技能全文拼接进来。

## Codeywood / screenplay-writer

https://github.com/kaigani/codeywood/blob/main/skills/core/screenplay-writer/SKILL.md

借鉴：从节拍与场景走向正文；用主动、具体的视觉细节写动作；按视觉注意力换段；写完检验动作可呈现、对白可说、情绪可成立。

调整：原有“一段对应一个镜头或时刻”改成按行为、反应或注意力组织段落，不强制等镜头；保留镜头设计后置。当前技能允许在授权范围内重构弱场面，避免只标问题而不修。

## Emma / em-chief-writer

https://github.com/adoria111/emma-screenwriting-skills/blob/main/advanced/story-writing/skills/em-chief-writer/SKILL.md

https://github.com/adoria111/emma-screenwriting-skills/blob/main/advanced/story-writing/skills/em-chief-writer/references/writing-rules.md

借鉴：场内目标、阻碍、行动、回应、后果；关键选择与因果在正文发生；从观众获得信息的角度检验可理解性。

调整：不继承其完整项目流程、特定短剧节奏和额外交付清单；适用于较宽的小说类型与体量。

## Screenwriting Skills / sw-scene-craft

https://github.com/jtydhr88/screenwriting-skills/blob/main/plugins/screenwriting/skills/sw-scene-craft/SKILL.md

借鉴：人物欲望与对抗力量；行动—反应节拍；场面前后状态及转折；环境、道具参与冲突。

调整：场景价值变化作为判断工具，允许铺垫、停顿、余波和过渡。不强制每场翻转，不采用固定场次数、均匀场长或地点数量。

## Kimi-skill-package / screenplay

https://github.com/ZzzTSudio/Kimi-skill-package/blob/main/general-writing/screenplay/SKILL.md

借鉴：可感知的动作；描述自然引导注意力；空间、道具、时间和人物状态的连续性；视觉信息审读。

调整：静音检查改为辅助诊断，允许对白和声音承担关键叙事；不采用打分式质量证明、固定多轮审稿、第三轮强制通过或固定 Word 路径。

## Cinefoundry / screenwriting

https://github.com/hojiahao/cinefoundry/blob/main/.agents/skills/screenwriting/SKILL.md

借鉴：给反应、静默和空间建立留余量；动作遵循观看顺序；台词具有行动目的。

不继承：一句对白等于固定五秒、单人镜头绑定、固定镜头比例，以及对递物、拥抱、打斗、多人和可读文字的普遍限制。这些属于特定生成流水线的选择。

## 本技能新增

- 保核重构作为默认模式；区分故事核心、机制、实现和语言。
- 记录触发、规则反馈、限制与代价、关键选择及铺垫兑现，防止表面改写损坏机制。
- 维护角色与观众的知识边界，区分事实、猜测和新增改编。
- 小说的心理、叙述者和主观经验按具体功能转译，允许有用的声音、独白与文字。
- 长篇分批的阅读范围、改编状态、人物映射、未兑现伏笔与返修承接。
- 默认只输出文学剧本，不自动扩展到分镜、媒体生成或制作流水线。

这些规则是设计取舍，不能单凭来源或格式保证实际成片质量。

## 本轮审查新增参考

核对日期同上。新增参考用于审查与小幅修订，不引入额外运行依赖。

- [eternityspring/shuohao-skills / novel-outline](https://github.com/eternityspring/shuohao-skills/blob/main/skills/novel-outline/SKILL.md) 与 [novel-script](https://github.com/eternityspring/shuohao-skills/blob/main/skills/novel-script/SKILL.md)：借鉴来源定位、抽核后落到场面与上下游引用；不继承固定短剧时长、钩子和台词阈值。
- [suihe1/short-drama-production / novel-script](https://github.com/suihe1/short-drama-production/blob/main/skills/novel-script/SKILL.md)：参考按用户实际任务决定入口和改动范围、按需结构化、区分工具校验与创作判断的做法，不引入其完整工具链。
- [zenstory-ai/drama-skills / short-drama-develop](https://github.com/zenstory-ai/drama-skills/blob/main/skills/short-drama-develop/SKILL.md)：参考故事引擎、功能账本、持续选择与代价；保留本技能直接交付剧本的定位。
- [danjdewhurst/story-skills / adaptation](https://github.com/danjdewhurst/story-skills/blob/main/skills/adaptation/SKILL.md)、[revision-continuity](https://github.com/danjdewhurst/story-skills/blob/main/skills/revision-continuity/SKILL.md)、[reader-panel](https://github.com/danjdewhurst/story-skills/blob/main/skills/reader-panel/SKILL.md)：借鉴场面取舍、改后依赖检查与无剧透模拟审读。普通使用不强制多代理，反馈不冒充真实受众。
- [zoec98/story-skill](https://github.com/zoec98/story-skill/blob/main/story-skill/SKILL.md)：参考仅凭节拍能否重建重要场面的检验；不继承忠实原场序、项目结构和提交约定。

结合实际用户模拟，修订强调：可见的小动作不等于主动策略；效果型返修要有正文中的实际效果；保留谜底的同时交代当前行动所需信息；明显重构需找到核心功能的新落点；用户明确改规则后更新所有受影响场面。

## 采纳后的合并与删减

将来源中的方法落实为三个按需检查：高影响变化用“原功能与来源—新行动—正文结果”对应；关键节拍以能否重建主要行动和因果检验；返修按实际依赖追踪。独立审读只给当前剧本，并区分表达缺口与保留悬念。

删除或放宽：整套字段必填、反复声明同一返修边界、过密的测试专属例子，以及将不可逆代价固定成某种宣告方式。保留原稿的有效声音和视觉意图，不要求已有剧本补写开发文件。没有引入 JSON 工程、量表门槛、固定批次或强制多代理。
