# LinkedIn Optimizer

[English](README.md) | 简体中文

一个适用于 Codex 和 Claude Code 的 LinkedIn 优化 skill。根据简历、个人主页、论文列表及目标岗位，调整个人资料，并通过浏览器完成修改和验证。主要面向寻找研究类行业岗位的计算机科学博士生和 AI 研究人员。

## 安装

### 让 agent 根据链接安装

把下面这句话发给你的 agent：

```text
请读取 https://github.com/Flitternie/linkedin-optimizer 的 README，将 linkedin-optimizer 安装到你当前使用的工具中，并验证安装成功。
```

供安装 agent 使用的步骤：

1. 下载仓库，找到 `skills/linkedin-optimizer/`，确认 `SKILL.md` 中的名称为 `linkedin-optimizer`。
2. 将整个 skill 文件夹复制到下表中对应的个人安装目录。Codex 也可以使用 `$skill-installer`。
3. 更新时保留本地修改，仅更新本 skill 的文件。
4. 检查文件和参考链接，并确认工具能识别该 skill；必要时请用户重启。浏览器连接在实际使用时配置。

### 手动安装

将 `skills/linkedin-optimizer/` 复制到对应目录：

| 工具 | 个人安装目录 | 项目安装目录 |
|---|---|---|
| Codex | `~/.agents/skills/linkedin-optimizer/` | `.agents/skills/linkedin-optimizer/` |
| Claude Code | `~/.claude/skills/linkedin-optimizer/` | `.claude/skills/linkedin-optimizer/` |

保留 `SKILL.md` 和 `references/browser-setup.md`。`agents/openai.yaml` 是可选的 Codex 界面配置，Claude Code 无需使用。安装后如果未显示，开启新会话或重启工具。

官方说明：[Codex skills](https://developers.openai.com/codex/skills)、[Claude Code skills](https://code.claude.com/docs/en/skills)。

## 使用

在 Codex 中：

```text
请使用 $linkedin-optimizer，根据我的简历优化 LinkedIn，目标是 Research Scientist 岗位。需要时帮我配置浏览器连接，完成资料修改并验证保存结果。
```

在 Claude Code 中：

```text
/linkedin-optimizer 根据我的简历优化 LinkedIn，目标是 Research Scientist 岗位。需要时帮我配置浏览器连接，完成资料修改并验证保存结果。
```

可以提供简历、个人主页、Google Scholar 链接、作品集或直接填写背景信息。简历不是必需项；材料不足时，agent 会主动询问。提供当前 LinkedIn 链接和目标岗位类型，方便针对性调整。

意向职位的 JD 或岗位链接是可选项。提供后，agent 会结合实际经历调整定位、关键词、项目重点和技能排序；没有 JD 时，按目标岗位类型继续。

## 浏览器连接

- **默认流程：**通过浏览器检查 LinkedIn，准备并应用授权范围内的修改，再验证保存结果。浏览器是必需的，仅提供文字建议不算完成。
- **连接问题：**agent 会主动排查，并在权限允许时配置浏览器集成或必要客户端。可使用浏览器 MCP、Playwright、CDP 或桌面浏览器集成，无需提前配好连接。
- **只审阅或只写草稿：**明确提出这一要求，agent 会按该范围处理。

agent 会使用当前环境可用的工具建立浏览器连接；你可能需要授予权限、重启工具或完成登录。详见[浏览器说明](skills/linkedin-optimizer/references/browser-setup.md)。

需要启动 Chrome 或 Playwright 时，agent 会打开可见的浏览器窗口，让你能看到修改过程，并直接在窗口中登录。登录、修改和验证使用同一个会话。

请在浏览器中自行输入登录信息、完成身份验证。资料修改不包含发送消息、投递岗位或发布帖子。

## 本地文件与许可证

简历等材料、修改前原文及执行进度保存在用户工作目录的 `.linkedin-optimizer-work/` 中，与安装的 skill 分开。在本仓库内工作时，`.gitignore` 会忽略该目录及约定的本地浏览器状态文件。

本项目采用 [MIT 许可证](LICENSE)。
