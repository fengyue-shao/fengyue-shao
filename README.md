# Hi, I'm fengyue 👋

学生开发者，主要使用 **C++20、Qt 6 与 QML**，关注 **Windows 桌面工程、系统接口与 Agent**。

喜欢从真实问题出发，把系统能力做成能日常使用的工具。从界面交互、线程与异步生命周期，到插件边界和结果验证，都是项目的一部分。

## 正在做的事

- 持续开发 **Windows Sidebar**，将系统监控、设备控制与桌面交互整合到一个应用中。
- 探索 **本地模型与 Agent 工作流**，实践模型服务、工具调用与执行结果验证。
- 设计 **C++ Agent 运行时与桌面插件的接入方式**，重点考虑权限、状态管理和验收；这部分仍在规划与实验中。
- 围绕项目学习现代 C++、Windows API、OpenCV 与端侧系统开发。

## 主要项目

### Windows Sidebar

一个基于 **C++20 / Qt 6 / QML** 的 Windows 桌面控制应用，也是持续迭代的主要项目。

最初从侧边监控栏起步，目前以顶部悬停唤出的控制栏为主要交互，整合系统状态、音频与媒体、网络设备、通知、剪贴板和专注工具。

- **桌面交互**：精简 / 展开控制栏、自动隐藏、多屏选择、主题与模块设置。
- **系统集成**：Win32 / WinRT / Core Audio、媒体会话控制、通知与设备操作。
- **活动展示**：灵动岛汇总持续活动、提醒与操作结果；自由桌面卡片仍为可选开发预览。
- **插件架构**：具体插件独立进程运行，通过受限 JSON 协议与宿主协作，主体不加载插件 UI 代码。

后续希望让用户和 Agent 都能通过明确的能力和权限边界使用桌面工具。Agent 接入仍在设计中；当前源码暂未公开。

### 本地模型与 Agent 实验

- 使用 **llama.cpp** 运行本地模型，验证模型服务与工具调用。
- 实验 **RAG / NL2SQL**，探索自然语言问题、数据关系与数据库查询的衔接。
- 研究任务描述、执行证据、结果验收，以及人与 Agent 的协作流程。

### 视觉、图形与嵌入式实践

- **OpenCV**：棋盘格标定、去畸变、Harris 角点、ArUco 与 `solvePnP`。
- **Vulkan**：使用 Vulkan-Hpp RAII 与 GLFW 实践基础渲染流程。
- **Raspberry Pi Pico 2 W**：使用 C/C++ 与 I²C 驱动 OLED。

## 技术与实践

| 方向 | 主要使用或实践内容 |
| --- | --- |
| 语言 | C++17/20、C、Python |
| 桌面与系统 | Qt 6、Qt Quick / QML、Win32、C++/WinRT、Core Audio |
| 工程工具 | CMake、MSVC、Git、Docker、Visual Studio、VS Code |
| AI 与数据实验 | llama.cpp、LLM 工具调用、RAG、NL2SQL、PostgreSQL |
| 视觉与图形实验 | OpenCV、相机标定、ArUco、Vulkan、GLFW |
| 嵌入式实验 | Raspberry Pi Pico SDK、I²C、OLED |

## 学习方式

从项目中的具体问题出发，先建立能解释“为什么、怎么做”的思路，再用代码验证，按需要深入。近期主线是 **C++ 系统开发与 Agent 工程**，持续关注可靠的工具调用、权限边界和自然的桌面体验。

> I build to understand — from the system boundary to the user experience.
