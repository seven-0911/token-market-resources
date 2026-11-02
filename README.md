# TOKEN超市 行业 MCP 与 Skills

用于 TOKEN超市 AI一键助手的行业资源目录。小程序只携带界面，MCP 便携包在点击安装后从本仓库 Releases 下载。

## 在助手中使用

1. 打开“行业资源”。
2. 来源选择“我的 GitHub 仓库”，填写 `seven-0911/token-market-resources`，点击“读取目录”。
3. 选择“建筑设计”，点击名称查看功能和使用条件，再点击“安装”。

当前收录 SU / SketchUp MCP、CAD MCP，以及两个基础示例 Skill。

SU / CAD 的便携包仅支持 Windows x64，自带 Python 3.11 与依赖。SU 安装前请先关闭 SketchUp；安装后重开 Codex / SketchUp，并在扩展菜单启动 MCP 的 Start Server。CAD 需要已有支持 COM 的 CAD 桌面软件，与 Codex 使用同一 Windows 用户及相同权限。安装器不提供 CAD/SketchUp 本体或许可证。

首次安装建筑 MCP 需下载约 59 MB；下载后校验 SHA256 并缓存，安装另一项时复用缓存。小程序下载包本身保持几 MB。Mac/Windows ARM64 可浏览此目录和使用支持平台的 Skill，不能安装这份 Windows x64 便携包。

## 维护资源

分类、中文名称、功能说明与使用条件在 `industry-catalog.json`。修改后，用户重新读取目录即可看到。添加普通 Skill 时放进 `skills/技能名/SKILL.md`，并在清单中增加条目。普通 MCP 的接入方式见“仓库维护说明.md”。

大型二进制资源放在 Releases，避免每次读取目录时下载整个便携包。现有建筑 MCP 包固定版本 `industry-20261102`，SHA256：`12e6415a7824ed7dbc73b06776bbb6acc3343d8a10c902c904b89d2c8453833c`。

资源含第三方组件，相关来源、许可和说明保留在原始 ZIP 中。各资源的权利以其原有声明为准，本仓库不作统一重新授权。工具初始化和安装成功不代表已连通目标电脑的 CAD/SU。

本仓库不包含用户 API、聊天记录、账号配置或助手源码。
