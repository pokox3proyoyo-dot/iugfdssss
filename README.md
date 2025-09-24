# Secure Chat (GitHub Pages)

[![English](https://img.shields.io/badge/lang-English-lightgrey.svg)](README.md)
[![Русский](https://img.shields.io/badge/lang-Русский-blue.svg)](README_RU.md)

A small client-side tool for encrypting and decrypting messages in the browser.  
The site runs entirely in the browser (no server-side crypto) and helps two people exchange encrypted messages using public/private key pairs.

---

## Features
- Generate a key pair directly in the browser.
- Import and save peer public key in localStorage.
- Encrypt/decrypt messages with AES-GCM derived from ECDH.
- Save your private key encrypted with a password.
- Mobile-friendly UI with notifications and design.

---

## Usage
1. Generate a key pair → copy your public key.
2. Share your public key with your peer.
3. Import peer's public key → verify fingerprint.
4. Encrypt a message and send the ciphertext.
5. Paste ciphertext to decrypt.

---

## Security notes
- Private keys must stay secret.
- Public keys should be verified by fingerprint.
- If you forget your password for the encrypted private key, recovery is impossible.
- Forward secrecy is not provided — rotate keys regularly.

---

## Deploying on GitHub Pages
1. Put `index.html` in the repo root (or `docs/`).
2. Enable Pages in repo settings.
3. Your site: `https://<username>.github.io/<repo>/`

---

⚠️ Disclaimer: This project is for educational/demo purposes. Not audited. Use at your own risk.
