# workwork — Flow 保活工具（驱动版，v1.4）

## 下载

👉 **[点击下载 workwork.zip](https://github.com/mathplayer001/download/raw/main/workwork.zip)**

## 这是什么

Flow 会用底层键盘/鼠标钩子检测“是否是真人操作”。普通模拟软件（SendInput）产生的信号会被标记成“注入的”，Flow 直接忽略，所以你照样被踢。

这个工具改装了 **Interception 内核驱动**，从驱动层伪造键盘信号，Flow 会当成真实硬件输入，因此能通过检测。

## 新功能（v1.4）

- **随机切换软件窗口**：Alt+Tab 不再只在前两个窗口之间来回跳，而是每次随机跳 1~N-1 个窗口，让 Flow 看到你在不同页面间来回切换。
- **随机切换 Chrome 标签页**：Ctrl+Tab 每次随机跳 1~N-1 个标签，不再只切前两个标签。

## 使用方法

1. 下载 `workwork.zip`，**完整解压**（不要只把 zip 里的单个文件拖出来）。
2. 双击文件夹里的 **安装驱动.bat** → 弹出窗口点「是」→ 装完**重启电脑**。
3. 双击 **workwork.exe**（标题应为 workwork v1.4）。
4. 勾选需要的功能，点 **Start**。
5. 看到 **Feature enabled: Yes** 就说明在跑，窗口别关。

详细说明（含常见问题）在 zip 里的 `使用说明.txt`（英文）。

## 注意

- 只注入键盘/鼠标信号，不读取任何数据。
- 驱动来源：[oblitum/Interception](https://github.com/oblitum/Interception)（开源）。
- 请按平台规定合理使用。
