# OpenVape

OpenVape 本地实验环境的单文件启动器。

把 Loader、注入器、原生 DLL 打包成一个 exe，双击即可使用，同时保留原注入器的全部命令行接口。

---

## 功能

- **GUI 模式** —— 双击打开 Loader，登录、选进程、注入
- **便携优先** —— 优先解包到 exe 同目录，不可写时才退回 `%LOCALAPPDATA%`

---

## 快速开始

### 方式一：GUI（推荐）

双击 `OpenVape.exe`，会弹出 Loader 窗口：

1. 输入任意用户名 → 登录
2. 从列表选中 Minecraft 进程
3. 等待加载完成

### 方式二：命令行

# 打开 Loader GUI
.\OpenVape.exe

# 注入指定进程（自动补内嵌 DLL 路径）
.\OpenVape.exe <pid>

# 原样转发给注入器
.\OpenVape.exe <pid> <dll>

# 注入器的方向键选择器
.\OpenVape.exe <dll>
