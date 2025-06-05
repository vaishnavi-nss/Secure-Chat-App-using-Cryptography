# Secure-Chat-App-using-Cryptography

# 🔐 Secure Chat App Using AES & Diffie-Hellman

A secure, end-to-end encrypted web-based chat application built with **HTML, CSS, JavaScript** for the frontend and **Python (socket programming)** on the backend. This app ensures secure messaging using **AES symmetric encryption** and **Diffie-Hellman key exchange**, with additional security validation using **Wireshark** and a custom-built Python packet sniffer.

## 🚀 Features

* 🔐 **End-to-End Encryption** using:

  * **Diffie-Hellman** for secure key exchange.
  * **AES** (Advanced Encryption Standard) for message encryption.
* 🌐 **Web-based Interface**: Clean, responsive chat UI using HTML/CSS/JS.
* 🔄 **Real-time Communication** via sockets.
* 🧪 **Network Security Validation**:

  * Used **Wireshark** and custom **Python packet sniffer** to inspect and verify encrypted traffic.
* 🗃️ **Chat History**: Optionally store encrypted messages in a local file or JSON.

## 🛠️ Tech Stack

| Component        | Technology                         |
| ---------------- | ---------------------------------- |
| Frontend         | HTML, CSS, JavaScript              |
| Backend          | Python (socket programming)        |
| Encryption       | AES (PyCryptodome), Diffie-Hellman |
| Security Testing | Wireshark, Python sniffer          |

## 🖼️ UI Screens

* Dual-panel chat interface
* Message bubbles for each user
* Live, encrypted messaging in a single-page layout

## 📦 How to Run

1. **Clone the repository**

   ```bash
   git clone https://github.com/your-username/secure-chat-app.git
   cd secure-chat-app
   ```

2. **Run the server**

   ```bash
   python server.py
   ```

3. **Open the frontend**
   Open `index.html` in your browser or host it using a local server like Live Server (VS Code extension).

4. **Open client**
   Run `client.py` or open another browser tab for a second user.

## 🔍 Security Tools Used

* **Wireshark**: Verified that messages were encrypted on the wire.
* **Python Packet Sniffer**: Custom script to monitor raw socket traffic and confirm encryption.

## 📁 Project Structure

```
secure-chat-app/
├── frontend/
│   ├── index.html
│   ├── style.css
│   └── script.js
├── server.py
├── client.py
├── encryption/
│   ├── aes.py
│   └── diffie_hellman.py
├── utils/
│   └── packet_sniffer.py
└── README.md
```

## ✅ Future Enhancements

* User authentication
* Group chat support
* Message delivery status
* Deployment to a hosting service (e.g., Render, Vercel, or Netlify)

---
