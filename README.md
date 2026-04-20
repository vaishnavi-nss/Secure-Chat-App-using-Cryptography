🔐 END-TO-END ENCRYPTED REAL-TIME CHAT SYSTEM (AES + DIFFIE-HELLMAN)

A secure, real-time chat application designed with a focus on end-to-end encryption, secure key exchange, and network-level validation. This system implements cryptographic protocols from scratch and verifies message confidentiality using packet inspection tools.

🔍 Overview

This project demonstrates how secure communication systems are built by combining cryptography, networking, and real-time messaging.

Key Objectives:

1. Enable secure peer-to-peer communication
2. Ensure confidentiality of messages over insecure networks
3. Validate encryption using real network traffic analysis

🧠 System Design
1. 🔑 Encryption Flow
2. Clients establish a shared secret using Diffie-Hellman key exchange
3. A symmetric session key is derived
4. Messages are encrypted using AES before transmission
5. Encrypted data is sent over sockets
6. Receiver decrypts using the shared key

⚙️ Tech Stack

Layer	Technology | 
Frontend	HTML, CSS, JavaScript  | 
Backend	Python (Socket Programming) | 
Encryption	AES (PyCryptodome), Diffie-Hellman | 
Networking	TCP Sockets | 
Security	Wireshark, Custom Packet Sniffer

🚀 Features
1. 🔐 End-to-End Encryption
2. Diffie-Hellman for secure key exchange
3. AES for fast and secure message encryption
4. ⚡ Real-Time Messaging
5. Low-latency communication using TCP sockets
6. 🌐 Web-Based Interface
7. Lightweight and responsive chat UI
8. 🧪 Security Validation
9. Verified encrypted traffic using Wireshark
10. Built a custom Python packet sniffer to inspect raw packets
11. 🗃️ Encrypted Message Storage
12. Optional local storage of encrypted chat history

🧪 Security Validation

To ensure message confidentiality:

1. Network traffic was captured using Wireshark
2. A custom packet sniffer was implemented to inspect transmitted data
3. Verified that no plaintext messages are exposed over the network

📊 Key Engineering Decisions
1. AES over RSA for message encryption: Faster and more suitable for real-time communication
2. Diffie-Hellman for key exchange: Eliminates need to transmit encryption keys directly
3. Socket-based communication: Provides full control over message transmission

⚠️ Limitations
1. No authentication (vulnerable to MITM attacks)
2. Single-room chat (no group communication)
3. Not deployed (local environment only)
   
🚧 Future Improvements

1. Add user authentication and identity verification
2. Implement group chat with secure key distribution
3. Introduce TLS layer for additional transport security
4. Deploy using cloud platforms for real-world usage


📁 Project Structure

secure-chat-app/

├── frontend/

│   ├── index.html

│   ├── style.css

│   └── script.js

├── server.py                 # Handles socket connections

├── client.py                 # Client-side communication

├── encryption/

│   ├── aes.py                # AES encryption logic

│   └── diffie_hellman.py     # Key exchange implementation

├── utils/

│   └── packet_sniffer.py     # Network packet inspection

└── README.md

🖥️ How to Run
1. Clone the Repository
git clone https://github.com/vaishnavi-nss/Secure-Chat-App-using-Cryptography.git
cd Secure-Chat-App-using-Cryptography
2. Start the Server
python server.py
3. Launch the Client
Open index.html in a browser (or use a local server)
Run client.py or open another instance for a second user
