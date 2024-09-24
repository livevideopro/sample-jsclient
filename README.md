Here is a sample `README.md` for the [LiveVideoPro sample-jsclient repository](https://github.com/livevideopro/sample-jsclient):

---

# LiveVideo Sample For JS Client

[中文版 README 请点击这里](README.zh-CN.md)

This repository contains a sample JavaScript client for testing and demonstrating LiveVideo functionalities, such as video streaming, screen sharing, and end-to-end encryption (E2EE) within a web environment.

## Features

- **WebSocket Connection**: Connect to a WebSocket server for live video communication.
- **End-to-End Encryption (E2EE)**: Secure your communications using E2EE.
- **Simulcast and Dynacast**: Use multiple streams for better performance and adapt based on bandwidth.
- **Adaptive Streaming**: Optimize the stream based on network conditions.
- **Screen Sharing**: Share your screen with participants.
- **Device Controls**: Control microphone, camera, and flip the video feed.
- **Simulated Scenarios**: Test real-world scenarios like node failure, migration, and connection failures.

## Setup

1. Clone the repository:

   ```bash
   git clone https://github.com/livevideopro/sample-jsclient.git
   ```

2. Navigate to the project directory:

   ```bash
   cd sample-jsclient
   ```

3. Install dependencies:

   ```bash
   npm install
   ```

4. Start the development server:

   ```bash
   npm run dev
   ```

5. Open `index.html` in your browser and configure the WebSocket URL, Token, and other options for connecting to the server.

## Usage

### Connecting to LiveVideo

1. **LiveVideo URL**: Enter the WebSocket server URL (e.g., `ws://localhost:7880`).
2. **Token**: Provide a valid authentication token if needed.
3. **E2EE Key**: Enter the encryption key for E2EE.

### Stream Options

- **Publish**: Enable or disable publishing your stream.
- **Simulcast/Dynacast**: Select whether to use simulcast or dynacast.
- **Force TURN**: Use the TURN server for relaying media.
- **Auto Subscribe**: Automatically subscribe to other participants' streams.
- **Enable E2EE**: Turn on end-to-end encryption.

### Actions

- **Connect**: Establish a connection to the LiveVideo server.
- **Enable Mic/Camera**: Toggle audio and video input.
- **Flip Camera**: Switch between front and rear camera.
- **Share Screen**: Start sharing your screen with other participants.
- **Enable E2EE**: Toggle encryption during the call.

## Simulated Scenarios

You can simulate different connection scenarios such as node failures, reconnections, and server boot. Use the dropdown menu in the UI to choose the scenario you want to test.
