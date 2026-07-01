# 灵启 Skill 开发项目

## 项目目的

本项目用于灵启（lingqi）skill 的修改、调试、测试。

## 目录结构

```
lingqi/
├── SKILL.md              # 核心技能定义
├── README.md             # 使用说明
├── AGENTS.md             # 项目规范（本文件）
├── agents/               # 模型配置
│   └── openai.yaml
├── references/           # 参考文档
│   ├── agent-prompts.md
│   ├── anti-patterns.md
│   ├── eval-design.md
│   ├── model-adapters.md
│   ├── output-modes.md
│   └── testing-and-qa.md
└── scripts/              # Python 工具脚本
    ├── check_prompt_artifact.py
    └── score_prompt_shape.py
```

## 工作规则

1. 所有灵启 skill 的开发工作在此项目进行
2. 修改前先在当前会话中梳理思路和校验项
3. 修改完成后必须运行 `check_prompt_artifact.py` 和 `score_prompt_shape.py` 验证
4. 提交前确认：只改了必要的，不碰无关代码
