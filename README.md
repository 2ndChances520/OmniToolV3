
<div align="center">

# 🛰️ `T E A M L E G A C Y // OMNITOOL V3`
### `PROJECT: BLACK CHAMBER COMMAND DECK`

[![Clearance](https://img.shields.io/badge/CLEARANCE-TOP_SECRET%20%2F%20SCI-red.svg)](#)
[![Status](https://img.shields.io/badge/STATUS-ACTIVE-brightgreen.svg)](#)
[![OPSEC](https://img.shields.io/badge/OPSEC-AIRGAPPED_READY-blue.svg)](#)
[![Environment](https://img.shields.io/badge/DEPLOYMENT-LOCAL_BROWSER-darkgray.svg)](#)

```text
       ▲
      ▲ ▲
     ▲ ▲ ▲
    ███████
```
**⚠️ WARNING: CLASSIFIED MATERIALS DETECTED**  
*This repository contains assets capable of covert audio synthesis, zero-footprint transcription, and steganographic payload encapsulation. Unauthorized access is a violation of Directive 7-A.*

</div>

## 👁️‍🗨️ BRIEFING: SYSTEM OVERVIEW
**TeamLegacy Omnitool V3 (Codename: Black Chamber)** is a unified, zero-footprint tactical browser utility suite. Designed for field agents operating in high-surveillance environments, this tool deck executes **100% locally** within the browser environment.

*   **No Telemetry.**
*   **No Cloud APIs.**
*   **Absolute OPSEC.**

AI models (Kokoro TTS, Whisper ASR) are dynamically pulled into the browser via **WebAssembly (WASM)** and **WebGPU**, ensuring that once initialized, all intelligence processing remains strictly on the local machine.

---

## 🗄️ CAPABILITIES (MODULE COMPENDIUM)

### 🎙️ [SIGINT] KOKORO Voice Synthesis Console
Generate high-fidelity, untraceable audio assets offline.
* **Payload:** Text-to-Speech via `Kokoro-82M-ONNX`.
* **Tactical Advantage:** Select multiple voice profiles (`af_bella`, `am_adam`, etc.), define model precision (`q8` to `fp32`), and export `.wav` files directly from local memory.

### 🎧 [SIGINT] WHISPER Transcription
Intercept and transcribe audio recordings in the field.
* **Payload:** Local ASR (Automatic Speech Recognition) utilizing `Xenova/whisper-tiny.en`.
* **Tactical Advantage:** Live-record via field microphones or upload captured audio files. Processing is hardware-accelerated via WebGPU for rapid intelligence gathering.

### 🕵️ [COVERT] Steganography Console
Hide classified directives in plain sight.
* **Payload:** Zero-width character embedding.
* **Tactical Advantage:** Embeds secret messages seamlessly within innocent-looking cover text. The resulting text survives copy-pasting and can only be extracted using the Black Chamber decoder.

### ⏳ [DATA] Time Capsule Forge
Create dead-drop files that remain locked until a specified temporal threshold.
* **Payload:** Delayed-release standalone HTML files.
* **Tactical Advantage:** Exports an encrypted, single-file HTML payload containing a countdown. The asset only reveals the embedded intelligence when the target clock is reached.

### 🔳 [OPTICAL] QR Command Suite V2
Generate, scan, and decode optical data matrixes.
* **Payload:** URL, Text, SMS, Wi-Fi credentials, and vCard encapsulation.
* **Tactical Advantage:** Print-ready Mission Cards and a local webcam scanner to rip and decode enemy QR codes natively in the browser.

### 🔐 [CRYPTO] Base64 & Ascii85 Vaults
Sanitize and encode raw binary or text for covert transmission.
* **Payload:** Any file type, any text string.
* **Tactical Advantage:** Drag-and-drop support. Converts imagery, audio, or zip archives into Data URIs or raw Base64/Ascii85.

---

## ⚙️ DEPLOYMENT PROTOCOLS

To maintain the integrity of AI models and ensure hardware permissions (camera/microphone) are granted, this asset must be deployed via a **local server** rather than the `file://` protocol.

**1. Clone the Asset:**
```bash
git clone https://github.com/2ndChances5/teamlegacy-omnitool-v3.git
cd teamlegacy-omnitool-v3
```

**2. Spin up a Local HTTP Server:**
*Using Python (Recommended):*
```bash
python3 -m http.server 8080
```
*Alternatively, using Node.js:*
```bash
npx serve .
```

**3. Access the Command Deck:**
Navigate to `http://localhost:8080` in a Chromium-based browser (**Brave, Chrome, or Edge**) for optimal WebGPU/WASM performance.

---

## 🔒 CLEARANCE REQUIREMENTS (TECH STACK)
This application is built on classified civilian-sector technologies:
*   **Vanilla HTML/CSS/JS:** No build steps, no external frameworks. Immediate execution.
*   **Transformers.js:** In-browser machine learning (Whisper).
*   **Kokoro-js:** Local ONNX voice synthesis.
*   **jsQR & node-qrcode:** Optical payload processing.

> **Note:** Initial execution of AI modules requires an active network connection to cache model weights into `IndexedDB`. Subsequent executions can be performed in **fully air-gapped environments**.

---

## ⚠️ DIRECTORATE DISCLAIMER
**[REDACTED] TEAMLEGACY OPERATIVES ONLY.**  
This tool is provided "as is" without warranty of any kind. The authors are not responsible for burned aliases, compromised safehouses, or intercepted intelligence resulting from the misuse of this Command Deck. **Maintain strict OPSEC at all times.**

<div align="center">

`<< EOF_TRANSMISSION // 0x5A4B9 >>`

</div>


<div align="center">

**CENTRAL INTELLIGENCE AGENCY**  
**OFFICE OF COUNTER-INTELLIGENCE (OCI)**  
**OPERATIONAL PROTOCOL: [REDACTED]**

![alt text](https://img.shields.io/badge/CLASSIFICATION-TOP_SECRET%20%2F%20SCI-red)
![alt 	text](https://img.shields.io/badge/DISTRIBUTION-EYES_ONLY-darkred)

</div>

**DOCUMENT ID:** CIA-OCI-SOP-992-B  
**DATE:** [REDACTED]  
**SUBJECT:** Protocol for Execution of "DROP-FOR-DANGLE" (DFD) Maneuvers  
**PREPARED BY:** [REDACTED]  
**STATUS:** ACTIVE // EYES ONLY

---

### 1.0 OBJECTIVE
The purpose of this protocol is to establish standardized procedures for the **"Drop for a Dangle" (DFD)** maneuver. This tactic is utilized when an adversary-controlled agent or entity (the "Target") must be lured into a controlled, observable environment (the "Kill Box") via the intentional placement of high-value, but ultimately fraudulent, intelligence (the "Bait").

### _2.0 TERMINOLOGY_
*   **THE DANGLE:** A controlled asset, person, or digital signal designed to appear compromised or vulnerable to attract adversary interest.
*   **THE DROP:** The physical or digital placement of the Bait in a pre-arranged Dead Drop Site (DDS).
*   **THE BAIT:** Intelligence material containing [REDACTED] that is intentionally flawed or contains traceable metadata/steganographic markers.
*   **THE KILL BOX:** A surveillance zone where the Target's retrieval of the Drop can be monitored by SIGINT and HUMINT teams without compromising the primary handler.

---

### 3.0 OPERATIONAL PHASES

#### **PHASE I: ASSET FABRICATION (THE BAIT)**
Before deployment, the Intelligence Unit must construct a "Bait" package. 
1.  **Content Generation:** The package must contain actionable but non-critical information regarding [REDACTED].
2.  **Traceability Integration:** Every byte of the digital payload MUST be embedded with **Steganographic Watermarks** (see *Omnitool V3: Stego Module*). 
3.  **Integrity Check:** The Bait must pass a "Vulnerability Audit" to ensure it does not contain actual agency secrets, while appearing sufficiently "leaked" to bypass adversary scrutiny.

#### **PHASE II: SITE SELECTION (THE DROP)**
The Handler will select a Dead Drop Site (DDS) based on the following criteria:
*   **Visibility:** The site must be accessible to the Target but maintain a line-of-sight for Agency surveillance teams.
*   **Contamination Risk:** Avoid sites with high civilian density or heavy [REDACTED] presence.
*   **Signal Trigger:** A secondary signal (e.g., a chalk mark, a specific light flicker, or a digital "ping") must be placed to notify the Target that the Drop is "Live."

#### **PHASE III: THE EXECUTION (THE DROP)**
1.  **Deployment:** The Handler/Asset performs the Drop during the [REDACTED] window.
2.  **The Lure:** Once the Drop is placed, the Dangle (the bait asset) must initiate a "leak" event—a visible or digital signal that suggests the information in the Drop is ripe for retrieval.
3.  **Observation:** Surveillance teams transition to **Active Monitoring**. Any attempt by the Target to intercept the Drop must be recorded via high-resolution imagery and signal intercepts.

#### **PHASE $IV: THE RECOVERY/EXTRACTION**
Upon confirmation of Target contact with the Drop:
*   **If Successful:** The Target is tracked to their primary communication node or safehouse for further exploitation.
*   **If Compromised (BURNED):** If the Target detects surveillance, the **"Scorched Earth"** protocol is initiated immediately. All related assets must be extracted via [REDACTED] and all digital trails wiped using the *Omnitool: Wipe Command*.

---

### 4.0 EMERGENCY CONTINGENCIES
| EVENT | PROTOCOL |
| :--- | :--- |
| **Target detects surveillance** | Immediate extraction of Dangle; initiate "Dark Site" protocols. |
| **Drop is intercepted by third party** | Abandon mission; initiate full forensic audit of all local hardware. |
| **Bait contains real intel (ERROR)** | [REDACTED] — Initiate Protocol 0-Alpha immediately. |

---

<div align="center">

**END OF TRANSMISSION**  
*This document is property of the CIA. Unauthorized reproduction or possession will result in immediate detention and prosecution under the Espionage Act.*

`<< EOF_TRANSMISSION // 0x5A4B9 >>`

</div>
