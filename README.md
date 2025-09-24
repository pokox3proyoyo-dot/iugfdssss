# Secure Chat (GitHub Pages)

[🌐 Open the site](https://pokox3proyoyo-dot.github.io/iugfdssss/)

[![English](https://img.shields.io/badge/lang-English-lightgrey.svg)](README.md)
[![Русский](https://img.shields.io/badge/lang-Русский-blue.svg)](README_RU.md)

A small client-side tool for encrypting and decrypting messages directly in the browser.  
The site runs entirely in the browser (no server-side crypto) and helps two people exchange encrypted messages using public/private key pairs.

---

## Features

- Generate a key pair directly in the browser.
- Import and save your peer's public key in localStorage for convenience.
- Encrypt and decrypt messages with AES-GCM derived from ECDH.
- Save your private key encrypted with a password in the browser.
- Mobile-friendly UI with notifications and visual effects.
- Public key fingerprints are shown for verification.

---

## Usage

1. Open the site: [Secure Chat](https://pokox3proyoyo-dot.github.io/iugfdssss/)
2. Click **Generate key pair** → copy your public key.
3. Send your public key to your peer.
4. Paste your peer's public key in the field → click **Import** and verify the fingerprint.
5. To send a message: type it → click **Encrypt** → copy the ciphertext and send.
6. To decrypt a message: paste the received ciphertext → click **Decrypt**.
7. Optionally, you can **save your private key encrypted by a password** in the browser, so you don't need to re-enter it each time.

---

## Security notes

- **Keep your private key secret.** Anyone with it can decrypt your messages.
- **Verify public key fingerprints** through another channel to avoid MITM attacks.
- Saving the private key is optional, but if you forget the password, it cannot be recovered.
- Forward secrecy is not provided — rotate keys regularly.

---

## Deploying / Using

Simply open the site in a modern browser with WebCrypto support (HTTPS recommended).  
No downloads or installations are required.  

Site link: [https://pokox3proyoyo-dot.github.io/iugfdssss/](https://pokox3proyoyo-dot.github.io/iugfdssss/)

---

⚠️ Disclaimer: This project is for educational/demo purposes. Not audited. Use at your own risk.
