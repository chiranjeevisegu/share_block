BlockShare: Secure Decentralized File Sharing
BlockShare is a web-based application that demonstrates the principles of secure, blockchain-inspired file sharing. It allows users to encrypt files with a password, generate a unique transaction ID, and share them securely. The application simulates key blockchain concepts like cryptographic hashing for file integrity and time-locked access without requiring a complex backend.

Key Features
Client-Side Encryption: All files are encrypted and decrypted directly in your browser using the powerful AES algorithm via CryptoJS. Your unencrypted files and passwords are never sent to any server.

Time-Locked Files: Set an expiration time for your shared files (e.g., 1 hour, 1 day, 1 week). After the duration passes, the file becomes inaccessible, mimicking a self-destructing smart contract.

Digital Notary Certificate: Upon upload, the app generates a "Proof of Existence" certificate. This certificate includes the file's unique SHA-256 hash, a timestamp, and the transaction ID, providing undeniable proof that a specific version of the file existed at that moment.

Modern & Responsive UI: A clean, dark-themed interface built with Tailwind CSS that works seamlessly on both desktop and mobile devices.

Zero Dependencies (Local Version): The local version runs entirely from a single HTML file with no need for installation, servers, or external databases.

How It Works
The application simulates a secure file notarization and sharing process:

File Selection: The user selects a file from their local machine.

Client-Side Reading: The file is read into the browser's memory using the JavaScript FileReader API.

Encryption: The file's content is encrypted using the password provided by the user with AES encryption.

Hashing: A unique SHA-256 hash of the original, unencrypted file is generated. This hash acts as the file's unique fingerprint on the simulated blockchain.

Transaction Simulation: A random, unique Transaction ID (txId) is generated.

In-Memory Storage: The encrypted file data and its metadata (original filename, hash, timestamp, expiry) are stored in a JavaScript object in the browser's memory, linked by the txId.

Retrieval & Decryption: To download, the user provides the txId and password. The application looks up the encrypted data, decrypts it with the password, and verifies that the hash of the decrypted file matches the hash stored in the metadata, ensuring the file has not been tampered with.

How to Use (Local Version)
This version is designed to be incredibly simple to run.

Save the Code: Save the provided code as an HTML file (e.g., blockshare.html).

Open in Browser: Open the blockshare.html file in any modern web browser like Chrome, Firefox, or Edge.

Share Files:

Drag and drop a file or click to select it.

Enter a strong password and choose an access duration.

Click "Encrypt & Notarize".

Copy the generated "File Transaction ID" and share it along with the password with your recipient.

Retrieve Files:

Paste the Transaction ID and enter the correct password.

Click "Decrypt & Download".

Note: Since this version runs without a database, all shared links will be lost when the browser tab is closed or refreshed.

Technology Stack
HTML5: For the core structure of the web page.

Tailwind CSS: For modern, utility-first styling and a responsive layout.

JavaScript (ES6+): For all application logic, including DOM manipulation and event handling.

CryptoJS: A powerful JavaScript library used for the client-side AES encryption and SHA-256 hashing.
