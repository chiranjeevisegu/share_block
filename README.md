BlockShare
A secure, decentralized file sharing application that uses client-side encryption and simulates blockchain concepts for ultimate privacy.

🚀 Demo
A screenshot of the BlockShare application interface.
Since this is a local-only version, there is no live demo link. Users can run it by following the installation instructions below.

✨ Features
Client-Side Encryption: Files are encrypted in the browser using AES. Your private files and password never leave your machine.
Time-Locked Access: Set files to "self-destruct" after a specific duration (1 hour, 1 day, or 1 week), making them permanently inaccessible after the time expires.
Proof of Existence: Generates a digital notary certificate with a timestamp and a unique SHA-256 hash, providing cryptographic proof that your file existed at a specific time.
No Backend Required: The local version runs entirely in the browser with zero dependencies, making it incredibly portable and private.

🛠️ Technology Stack
Frontend: HTML5, Tailwind CSS, JavaScript (ES6+)
Libraries: CryptoJS
Deployment: Runs locally in any modern web browser.

⚙️ Installation
Getting this project running is simple.
Clone the repository:
git clone https://github.com/chiranjeevisegu/share_block.git
Navigate to the project directory:
cd share_block
Open the blockshare.html file:
No further installation is needed. Simply open the main HTML file in your favorite web browser.

Usage
Drag and drop a file into the upload area or click to select it.
Enter a secure password and select an optional access duration from the dropdown.
Click "Encrypt & Notarize".
Copy the generated Transaction ID from the activity log.
Share the Transaction ID and your password with the person you want to give access to.
Note: In this local version, all generated links are stored in the browser's memory and will be lost if you close or refresh the page.

🤝 Contributing
Contributions are always welcome! If you have ideas for improvements or find a bug, please feel free to:
Fork the Project
Create your Feature Branch (git checkout -b feature/AmazingFeature)
Commit your Changes (git commit -m 'Add some AmazingFeature')
Push to the Branch (git push origin feature/AmazingFeature)
Open a Pull Request

📄 License
This project is licensed under the MIT License. See the LICENSE file for details.

📧 Contact
Chiranjeevi Segu - @chiranjeevisegu

Project Link: https://github.com/chiranjeevisegu/share_block
