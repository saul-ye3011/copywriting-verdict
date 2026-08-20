# Copywriting Verdict

## 文案大师：把一句话送进战场、记忆和行动

`copywriting-verdict` 是一个用于商业文案创作、鉴赏、诊断、改写和比较的 Codex / Claude Skill。

它不把文案当作「更顺口的句子」，也不把鉴赏降格成形容词评分。每一句标语都要回答三个问题：它在跟谁打？它凭什么进入大脑？它如何让人记住并采取行动？

## 核心方法

当前 Skill 以五维实战鉴赏体系为固定裁决引擎，并在执行层补充场景诊断、写作流程、场景权重、批评量表和熔断检查。

| 维度 | 核心问题 | 解决什么 |
| --- | --- | --- |
| 战略锚定与博弈 | 你在跟谁打？战场在哪里？ | 生存权与排他性 |
| 认知物理与降噪 | 大脑处理这句话需要几卡路里？ | 进入大脑 |
| 人性暗门与欲望 | 你按下了哪个原始按钮？ | 冲动与购买许可 |
| 语言工程与声学 | 读起来像诗，还是像说明书？ | 记忆与传播 |
| 逻辑回环与场景 | 逻辑是否闭环？场景是否落地？ | 可信度与行动 |

五维之上还有一套「熔断机制」：僵尸词、自嗨、翻译坍塌、竞品替换、抽象堆叠、无证据承诺、视觉复述等问题，触发即删除或重写。

## 它能做什么

- 写 slogan、tagline、品牌宣言、广告标题、卖点和网站 Hero 文案
- 鉴赏并裁决已有文案，指出决定性缺陷
- 改写包装、社交媒体、视频说明和视觉导向文案
- 比较多个方向，保留最强候选而非堆砌相似选项
- 把视觉已经传达的内容转化为观众尚未获得的理解、价值或行动

## 标准工作流

```text
商业情境 → 战场诊断 → 主攻角度 → 多方向试写 → 熔断淘汰 → 最终交付
```

写作任务默认输出情境判断、主攻角度、候选文案、淘汰理由、最终推荐和必要的钩子-证据-行动建议。鉴赏任务先给裁决，再解释核心原因，最后决定是否改写。

## 快速安装

下载 [`dist/copywriting-verdict.skill`](./dist/copywriting-verdict.skill)，导入支持 `.skill` 的 Codex / Claude Skill 管理器。

也可以将 [`versions/01-copywriting-verdict/`](./versions/01-copywriting-verdict/) 目录复制到本地 skills 目录。

## 从源代码共创

1. Fork 或克隆本仓库。
2. 修改 `versions/01-copywriting-verdict/` 中的规则或参考资料。
3. 为新增行为补充 `evals/evals.json`。
4. 在 `VERSION_HISTORY.md` 记录版本变化、动机和影响。
5. 提交 Pull Request，并说明哪些维度被保留、改变或新增。

五维体系是裁决核心。执行器可以进化，但不能用泛化的营销建议替代它，也不能把新增规则堆成与核心重复的条款。

## 版本与来源

- [`v0 · 原始五维实战鉴赏体系`](./versions/00-original-prompt/original-prompt.md)：项目最早的理论与实操内核。
- [`历史补充 · 小丰角色提示词`](./versions/00-original-prompt/historical-xiaofeng-prompt.md)：后续出现的角色化提示词，保留作演化材料，不作为项目起源。
- [`v1 · copywriting-verdict`](./versions/01-copywriting-verdict/)：当前可运行 Skill。
- [`VERSION_HISTORY.md`](./VERSION_HISTORY.md)：版本边界、来源和缺失记录。

## 项目状态

当前仓库为 GitHub Private Repository。获得仓库权限的人可以安装、查看源码、提交 Issue 和参与共创。

## License

见 [`LICENSE`](./LICENSE)。本项目用于私下安装与协作，未经作者许可不得公开转载或再分发。
