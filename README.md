File Crypto Python Project

Overview

file_crypto.py is a Python-based file encryption and decryption tool using the Fernet symmetric encryption module from the cryptography library. It allows you to:
	•	Generate a secure encryption key
	•	Encrypt any file
	•	Decrypt encrypted files

This is useful for securing sensitive files locally.

⸻

Features
	•	Key Generation: Generates a secret key (secret.key) for encryption and decryption.
	•	File Encryption: Encrypts any file into a .enc encrypted format.
	•	File Decryption: Decrypts previously encrypted files using the correct key.
	•	Exception Handling: Handles invalid keys or corrupted files gracefully.

⸻

Requirements
	•	Python 3.x
	•	cryptography library

Install required packages:

pip install cryptography


⸻

Usage
	1.	Run the script

python file_crypto.py

	2.	Options

1. Generate Key
2. Encrypt File
3. Decrypt File

	3.	Examples

	•	Generate Key

Choose an option: 1
Key generated and saved as secret.key

	•	Encrypt File

Choose an option: 2
Enter file name to encrypt: note.txt
note.txt encrypted successfully! (Output: note.txt.enc)

	•	Decrypt File

Choose an option: 3
Enter file name to decrypt: note.txt.enc
note.txt.enc decrypted successfully! (Output: note.txt)


⸻

Security Note
	•	Keep secret.key safe. Losing the key will make decryption impossible.
	•	Do not push secret.key to public repositories. Add it to .gitignore:

secret.key


⸻

Project Structure

file-crypto/
├── file_crypto.py
├── README.md
└── .gitignore  # contains secret.key

