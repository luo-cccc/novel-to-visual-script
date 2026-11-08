# 方法来源与整合取舍

以下为既有方法参考，不是运行依赖。正文与示例由本项目综合编写；执行规则以 [SKILL.md](../SKILL.md) 及其参考文件为准。

## 参考方法

| 来源 | 采用的方法 |
| --- | --- |
| [Codeywood / screenplay-writer](https://github.com/kaigani/codeywood/blob/main/skills/core/screenplay-writer/SKILL.md) | 从节拍与场景落到正文；用具体动作引导注意力，检查动作、对白和情绪是否成立。 |
| Emma / [em-chief-writer](https://github.com/adoria111/emma-screenwriting-skills/blob/main/advanced/story-writing/skills/em-chief-writer/SKILL.md)、[writing-rules](https://github.com/adoria111/emma-screenwriting-skills/blob/main/advanced/story-writing/skills/em-chief-writer/references/writing-rules.md) | 场内目标、阻碍、行动、回应与后果；从观众获得信息的角度检查因果。 |
| [Screenwriting Skills / sw-scene-craft](https://github.com/jtydhr88/screenwriting-skills/blob/main/plugins/screenwriting/skills/sw-scene-craft/SKILL.md) | 人物欲望与对抗力量、行动与反应、场面状态变化，以及环境和道具参与冲突。 |
| [Kimi-skill-package / screenplay](https://github.com/ZzzTSudio/Kimi-skill-package/blob/main/general-writing/screenplay/SKILL.md) | 可感知动作、视觉注意力，以及空间、道具、时间和人物状态的连续性。 |
| [Cinefoundry / screenwriting](https://github.com/hojiahao/cinefoundry/blob/main/.agents/skills/screenwriting/SKILL.md) | 按观看顺序写动作，为反应、静默和空间建立留余量，让对白具有行动目的。 |
| shuohao-skills / [novel-outline](https://github.com/eternityspring/shuohao-skills/blob/main/skills/novel-outline/SKILL.md)、[novel-script](https://github.com/eternityspring/shuohao-skills/blob/main/skills/novel-script/SKILL.md) | 来源定位、提取核心后落到场面，以及上下游依赖追踪。 |
| [short-drama-production / novel-script](https://github.com/suihe1/short-drama-production/blob/main/skills/novel-script/SKILL.md) | 按实际任务决定入口和改动范围，按需结构化，区分工具校验与创作判断。 |
| [drama-skills / short-drama-develop](https://github.com/zenstory-ai/drama-skills/blob/main/skills/short-drama-develop/SKILL.md) | 故事引擎、功能账本、持续选择与代价。 |
| story-skills / [adaptation](https://github.com/danjdewhurst/story-skills/blob/main/skills/adaptation/SKILL.md)、[revision-continuity](https://github.com/danjdewhurst/story-skills/blob/main/skills/revision-continuity/SKILL.md)、[reader-panel](https://github.com/danjdewhurst/story-skills/blob/main/skills/reader-panel/SKILL.md) | 场面取舍、返修后的依赖检查，以及不提前提供答案的模拟审读。 |
| [zoec98 / story-skill](https://github.com/zoec98/story-skill/blob/main/story-skill/SKILL.md) | 检查关键节拍是否足以重建重要场面的行动与因果。 |
| [write-screenplay-skill](https://github.com/egguy886/write-screenplay-skill) | 台词禁区、语言档案与遮名测试、信息差四种用法与三个时间点、封死退路、反派自保、场间“于是/但是”、三次法则与前移。 |
| [chinese-novelist-skill](https://github.com/PenglongHuang/chinese-novelist-skill) | 潜台词四式、对话权力信号、信息差被打破时须有后果、虚假悬念禁忌。 |
| [short-dramas](https://github.com/dingmike/short-dramas) | 压抑与释放、强度递增、喘息集带新信息、中途的真实失败。 |
| [chinese-webnovel-skills](https://github.com/tance-mang/chinese-webnovel-skills)、[bookflow-skill](https://github.com/LanyXiaosheng/bookflow-skill)、[Distilled-Novel-Toolbox](https://github.com/dama-cyber/Distilled-Novel-Toolbox) | 情绪外显、二次动作、惯用反应限频、围观只做余波、拒绝假压力。 |
| [creative-writing-skills](https://github.com/haowjy/creative-writing-skills) | 生成式写作的失败模式；词表只是审美偏好，不作检测依据。 |
| [thriller](https://github.com/pajama-studio/thriller) | 场次进出的知识状态记录、谎言的构成。 |
| [natural-voice](https://github.com/xielingyuan89-prog/natural-voice) | 开口前定位关系、目的、所知等七项；不按角色平均添加口头禅；人物不回应未听见的台词；“可以不改”的反例。 |
| [screenwriting-skills / sw-dialogue](https://github.com/jtydhr88/screenwriting-skills) | 对白即行动、换人测试、引入第三方、句尾放重心。 |
| [novel-to-screenplay-skill](https://github.com/zq940222/novel-to-screenplay-skill)、[movieScriptSkill](https://github.com/FelixFengDui/movieScriptSkill) | 提炼与视觉替代；晚进早出、“绝不会说的话”、用破折号标打断。 |

## 本项目自建的部分

以下内容不是从上表来源继承的，而是本项目针对“保核重构”这一任务自行约定的，改动时需同时更新对应用例：

- 四层保留项（锁定项 / 核心 / 机制 / 实现，见 [mechanism-contract.md](mechanism-contract.md)）与 A–D 改编档位（见 [SKILL.md](../SKILL.md)）。
- 去标签比较的四个维度：决定节点、关系网、信息揭示、解决方式与结尾。
- 核心类型与必保条件表，用于把“核心吸引力”转成可操作判断。
- 写前改编卡、方向确认点、[承接记录](adaptation-state.md) 结构。
- 权属前提与规避请求的处理方式：情节的选择安排与人物关系组合同样可能受保护，因此 C、D 档只保留类型、机制、情感作用这类较抽象的部分，重做人物关系网、情节组合与表达。
- [回归评测集](../evals/README.md)，用于改动后对比行为。

## 整合取舍

- 保留场面、因果和观众视角的判断方法，不继承各来源的完整项目流程、固定短剧节奏、场数、镜头比例或对白秒数换算。
- 对白与去 AI 味只吸收能在场面里判断功能的方法，不采用全文硬禁词、字数配额、钩子类型轮换表、爽点占比、运镜术语或规避平台检测的做法；“模型常见失败”是审读提示，不是禁词表。
- 按行为、反应和注意力组织段落，镜头设计后置；静音检查只辅助诊断，声音、独白和必要文字仍可承担关键叙事。
- 用正文缺口与实际依赖指导返修，不采用质量打分、固定审稿轮数或强制通过。模拟阅读用于发现表达问题，不作为真实受众数据。
- 载体弹性要求（[medium-profiles.md](medium-profiles.md)）只在用户指定载体时启用，默认不套用任何固定节奏；“爽点与集尾”例外，按核心类型启用。

本项目在这些方法上建立保核重构的约定，重点维护必要机制条件、知识边界与长篇承接。具体要求分别见 [重构边界](mechanism-contract.md)、[场面写作](visual-scene-craft.md) 和 [交付格式](script-format.md)。
