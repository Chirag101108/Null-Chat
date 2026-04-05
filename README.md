NullChat ⛓️

Minimal · Encrypted · Peer-to-Peer

🧠 Overview

NullChat is a lightweight, browser-based peer-to-peer chat application focused on secure communication with minimal infrastructure.

It establishes a direct encrypted channel between two peers using modern cryptography and WebRTC — no servers, no storage, no intermediaries.

⚙️ Features
🔐 End-to-End Encrypted Messaging
🤝 Direct Peer-to-Peer Communication
🔑 ECDH (P-256) Key Exchange
🛡️ AES-256-GCM Encryption
🖼️ Image Sharing
📁 File Transfer (chunked + encrypted)
⚡ Zero message storage
🏗️ Tech Stack
WebRTC (DataChannels)
Web Crypto API
ECDH (Elliptic Curve Diffie-Hellman)
AES-256-GCM
🚀 How It Works
Each peer generates a cryptographic key pair
Public keys are exchanged during connection setup
A shared secret is derived using ECDH
Messages are encrypted with AES-GCM
Data flows directly between peers via WebRTC
🧪 How to Use
1. Open the App

Open the HTML file in a modern browser (Chrome / Brave recommended).

2. Choose a Role
Initiator → starts the connection
Responder → joins using an offer
3. Establish Connection
Initiator:
Click Initiator
Copy the generated offer
Share it with the other user
Responder:
Paste the offer
Click Generate Answer
Copy the answer
Initiator:
Paste the answer
Click Connect
4. Start Messaging

Once connected:

Send messages
Share files or images
All communication is encrypted 🔒
⚠️ Security Notice

This project is experimental and not audited.

Limitations:

No identity verification (susceptible to MITM attacks)
No forward secrecy (single session key)
Metadata (IP, timing, size) is exposed

⚠️ Do not rely on this for sensitive or high-risk communication.
