
# LiveVideo 客户端 Demo

本项目是一个用于演示和测试 LiveVideo 功能的示例 JavaScript 客户端，支持视频流、屏幕共享以及端到端加密（E2EE）等功能。

## 功能特性

- **WebSocket 连接**：通过 WebSocket 服务器进行实时视频通信。
- **端到端加密 (E2EE)**：确保视频通信安全。
- **Simulcast 与 Dynacast**：支持多路流媒体，优化带宽使用。
- **自适应流媒体**：根据网络状况动态调整流媒体质量。
- **屏幕共享**：支持与其他参与者共享屏幕。
- **设备控制**：启用/禁用麦克风、摄像头，以及切换摄像头。
- **模拟场景**：支持模拟诸如节点故障、迁移、断线重连等实际场景。

## 安装步骤

1. 克隆此仓库：

   ```bash
   git clone https://github.com/livevideopro/sample-jsclient.git
   ```

2. 进入项目目录：

   ```bash
   cd sample-jsclient
   ```

3. 安装依赖：

   ```bash
   npm install
   ```

4. 启动开发服务器：

   ```bash
   npm run dev
   ```

5. 打开 `index.html` 文件，在浏览器中配置 WebSocket URL、Token 以及其他选项。

## 使用说明

### 连接到 LiveVideo

1. **LiveVideo URL**：输入 WebSocket 服务器地址（例如 `ws://localhost:7880`）。
2. **Token**：如果需要，提供有效的身份验证 Token。
3. **E2EE Key**：输入用于端到端加密的密钥。

### 流媒体选项

- **发布**：选择是否发布您的视频流。
- **Simulcast / Dynacast**：选择是否启用 Simulcast 或 Dynacast。
- **强制使用 TURN**：通过 TURN 服务器转发媒体流。
- **自动订阅**：自动订阅其他参与者的流。
- **启用 E2EE**：打开视频通话中的端到端加密。

### 操作按钮

- **连接**：连接到 LiveVideo 服务器。
- **启用麦克风 / 摄像头**：切换音频和视频输入。
- **切换摄像头**：在前置摄像头和后置摄像头之间切换。
- **共享屏幕**：与其他参与者共享屏幕。
- **启用 E2EE**：在通话过程中启用加密功能。

## 模拟场景

您可以通过界面中的下拉菜单模拟各种连接场景，例如节点故障、重连和服务器故障等。选择场景后，系统会自动模拟相应的网络情况，帮助您进行测试。
