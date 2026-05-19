<div align="center">

# `T E A M L E G A C Y // OMNITOOL V3`
### `PROJECT: BLACK CHAMBER COMMAND DECK`

[![Clearance](https://img.shields.io/badge/CLEARANCE-TOP_SECRET%20%2F%2F%20SCI-red.svg)](#)
[![Status](https://img.shields.io/badge/STATUS-ACTIVE-brightgreen.svg)](#)
[![OPSEC](https://img.shields.io/badge/OPSEC-AIRGAPPED_READY-blue.svg)](#)
[![Environment](https://img.shields.io/badge/DEPLOYMENT-LOCAL_BROWSER-darkgray.svg)](#)

```text
       ▲
      ▲ ▲
     ▲ ▲ ▲
    ███████


👁️‍🗨️ BRIEFING: SYSTEM OVERVIEW
TeamLegacy Omnitool V3 (Codename: Black Chamber) is a unified, zero-footprint tactical browser utility suite. Designed for field agents operating in high-surveillance environments, this tool deck executes 100% locally within the browser environment.
No telemetry. No cloud APIs. Absolute OPSEC.
AI models (Kokoro TTS, Whisper ASR) are dynamically pulled into the browser via WebAssembly (WASM) and WebGPU, ensuring that once initialized, all intelligence processing remains on the local machine.
🗄️ CAPABILITIES (MODULE COMPENDIUM)
1. [SIGINT] KOKORO Voice Synthesis Console
Generate high-fidelity, untraceable audio assets offline.
Payload: Text-to-Speech via Kokoro-82M-ONNX.
Tactical Advantage: Select multiple voice profiles (af_bella, am_adam, etc.), define model precision (q8 to fp32), and export .wav files directly from local memory without ever contacting a server.
2. [SIGINT] WHISPER Transcription
Intercept and transcribe audio recordings in the field.
Payload: Local ASR (Automatic Speech Recognition) utilizing Xenova/whisper-tiny.en.
Tactical Advantage: Live-record via field microphones or upload captured audio files. Processing is hardware-accelerated via WebGPU/WASM for rapid intelligence gathering.
3. [COVERT] Steganography Console
Hide classified directives in plain sight.
Payload: Zero-width character embedding.
Tactical Advantage: Embeds secret messages seamlessly within innocent-looking cover text. The resulting text survives copy-pasting across standard communication channels and can only be extracted using the Black Chamber decoder.
4. [DATA] Time Capsule Forge
Create dead-drop files that remain locked until a specified temporal threshold.
Payload: Delayed-release standalone HTML files.
Tactical Advantage: Exports a heavily encrypted, single-file HTML payload containing a countdown. The asset will only reveal the embedded intelligence when the target clock is reached.
5. [OPTICAL] QR Command Suite V2
Generate, scan, and decode optical data matrixes.
Payload: URL, Text, SMS, Wi-Fi credentials, and vCard encapsulation.
Tactical Advantage: Print-ready Mission Cards, center-branded payloads, and a local webcam scanner to rip and decode enemy QR codes natively in the browser.
6. [CRYPTO] Base64 & Ascii85 (Base85) Vaults
Sanitize and encode raw binary or text for covert transmission.
Payload: Any file type, any text string.
Tactical Advantage: Drag-and-drop file support. Converts imagery, audio, or zip archives into Data URIs or raw Base64/Ascii85. Validate data integrity with built-in roundtrip testing.
⚙️ DEPLOYMENT PROTOCOLS
To maintain the integrity of the AI models and ensure camera/microphone hardware permissions are granted by the browser, this asset must be deployed on a local server rather than opened via the file:// protocol.
Initialization Sequence:
Clone the Asset:
code
Bash
git clone https://github.com/YourAlias/teamlegacy-omnitool-v3.git
cd teamlegacy-omnitool-v3
Spin up a Local HTTP Server:
Using Python (recommended):
code
Bash
python3 -m http.server 8080
Alternatively, use Node.js:
code
Bash
npx serve .
Access the Command Deck:
Navigate to http://localhost:8080 in a Chromium-based browser (Brave, Chrome, Edge) for optimal WebGPU/WASM performance.
🔒 CLEARANCE REQUIREMENTS (TECH STACK)
This application is built on classified civilian-sector technologies:
Vanilla HTML/CSS/JS: No build steps, no external frameworks. Immediate execution.
Transformers.js: In-browser machine learning (Whisper).
Kokoro-js: Local ONNX voice synthesis.
jsQR & node-qrcode: Optical payload processing.
Note: Initial execution of AI modules requires an active network connection to cache the model weights into IndexedDB. Subsequent executions can be performed in fully air-gapped environments.
⚠️ DIRECTORATE DISCLAIMER
[REDACTED] TEAMLEGACY OPERATIVES ONLY.
This tool is provided "as is" without warranty of any kind. The authors are not responsible for burned aliases, compromised safehouses, or intercepted intelligence resulting from the misuse of this Command Deck. Maintain strict OPSEC at all times. End of transmission.
