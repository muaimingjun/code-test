## 功能特性：

- 主体为 Pydantic AI 智能体，并将另一个 Pydantic AI 智能体作为工具集成。
- 主代理为研究代理，子代理为邮件草稿代理。
- 提供 CLI 命令行界面与智能体交互。
- 邮件草稿代理集成 Gmail，研究代理集成 Brave API。

## 示例说明：

在 `examples/` 文件夹下有一个 README，建议先阅读以了解示例的整体思路，并参考其结构来编写你自己的功能文档。

- `examples/cli.py` —— 可作为创建 CLI 的模板参考
- `examples/agent/` —— 阅读此目录下所有文件，了解如何实现支持多种 LLM 提供商、处理智能体依赖、为智能体添加工具等最佳实践。

请勿直接复制这些示例代码，它们属于另一个项目，仅供借鉴和学习最佳实践。

## 文档资料：

Pydantic AI 官方文档：https://ai.pydantic.dev/

## 其他注意事项：

- 项目需包含 .env.example 文件，以及包含 Gmail 和 Brave 配置说明的 README。
- 在 README 中列出项目结构。
- 虚拟环境已预先配置好所有依赖。
- 环境变量请使用 python_dotenv 并通过 load_env() 加载。
