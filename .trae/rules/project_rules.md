---
description: 当用户提到期末速成、期末复习、考试冲刺、考前突击、考前速成、快速备考、/cram、速成某门课时，激活期末速成引擎的四阶段教学流水线
alwaysApply: false
---

# 期末速成引擎规则

## 触发后行为

当检测到用户需要期末速成时，自动激活 `cram-engine` skill。

如果 skill 未自动激活，手动引导用户：
"检测到你需要期末速成。请确认：你是想用四阶段速成流水线来备考吗？如果是，我会启动期末速成引擎。"

## 适用课程类型

- ✅ 所有文科：文史哲、法学、教育学、新闻传播、社会学、政治学、经管类
- ✅ 考试以理解和论述为主的课程
- ❌ 纯定量课不适用：高等数学、概率论、计量经济学

## 引擎文件位置

- 阶段指令：`stages/stage1-deconstruct.md` → `stage2-teach.md` → `stage3-test.md` → `stage4-remediate.md`
- 配置模板：`configs/example.yaml`
- 进度存储：`~/.cram-engine/`
