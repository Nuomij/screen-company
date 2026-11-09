# 面试前公司筛查

输入公司名称，从业务、经营变化、竞争位置、雇主风险和岗位关联五个方面，整理有来源的初步判断与3—5个面试追问。

## 安装

在支持 Node.js / npx 的终端使用 skills CLI：

```bash
npx skills add https://github.com/Nuomij/screen-company --skill screen-company
```

技能位于 `skills/screen-company/`，请安装完整目录，保留 references 文件。需要所用 AI 客户端提供联网搜索和网页读取能力；不要求特定付费接口。

## 使用

> 帮我在面试前筛查一下【公司名称】。

也可以附上岗位JD、工作城市和最在意的条件：

> 帮我筛查【公司名称】，岗位是【岗位名称】，地点在【城市】，我最关心稳定性。下面是JD：……

只有名称也能开始；名称不明确时先确认候选公司。需要补充时会说明问题总数，非必要信息可跳过。不要求先提供简历。

## 输出

- 五行筛查表：事实、求职意义、待核实事项。
- 值得继续了解的理由与主要疑点，各最多3项。
- 3—5个面试追问，并说明适合问谁。

关键判断附来源与日期；区分事实、推断、匿名线索和未知。不能联网时明确降级为基于所提供材料的分析。不把集团数字套给子公司，不将负面评论直接当事实，不给伪精确分数，也不保证公司稳定或岗位适合。

## 文件

- `skills/screen-company/SKILL.md`：入口与工作流程。
- `skills/screen-company/references/research-rules.md`：检索、核验、冲突和不同公司类型的处理。
- `skills/screen-company/references/report-template.md`：简报模板。
- `skills/screen-company/agents/openai.yaml`：支持此元数据的客户端显示信息。

采用通用 SKILL.md 格式。不同客户端的安装与调用入口可能不同；不声称已在豆包、WorkBuddy等每个客户端实测。

本仓库只分发技能文件，不收集简历或公司内部资料；使用时无需将个人材料提交到GitHub。
