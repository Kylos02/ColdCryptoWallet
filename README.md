<div align="center">

# 🪙 Cryptography Final Project 

### Faculty of Engineering UNAM | Semester 2026-1

</div>

---

## 📋 Description

This is the **final project** for the **Cryptography** course of the 2026-1 semester.

**Crypto-Wallet** is a complete implementation of a **cold crypto wallet** for account-based cryptocurrencies, developed from scratch using fundamental cryptographic primitives.

### What is a Cold Wallet?

A cold wallet is a cryptocurrency storage system that keeps private keys completely **offline and network-isolated**, maximizing security against remote attacks. Unlike "hot wallets" that are permanently connected to the internet, cold wallets only sign transactions locally, exporting only the signed result.

### Main Features

This project implements the **fundamental cryptographic primitives** of a professional wallet:

- 🔐 **Secure Key Management**: Ed25519 key pair generation, encrypted storage with AES-256-GCM, and key derivation using Argon2id
- ✍️ **Deterministic Digital Signature**: JSON transaction canonicalization and verifiable cryptographic signing
- ✅ **Complete Verification**: Digital signature validation, replay attack detection, and integrity checking
- 🪙 **Address System**: Ethereum-style address derivation using SHA-256
- 🧪 **Local Simulation**: Inbox/outbox folders that emulate sending/receiving without requiring a real blockchain

### Project Approach

The objective is to master **cryptographic fundamentals** through a practical implementation that meets professional security standards:
- No predefined wallet frameworks — implemented from scratch
- Exclusive use of audited cryptographic primitives (Ed25519, AES-256-GCM, Argon2id)
- Secure handling of secrets in memory and protection against common vulnerabilities
- Complete unit testing suite with golden test vectors

---

## 👥 Development Team

<table align="center">
  <tr>
    <td align="center">
      <b>👨‍💻 Garcia Cerda Gerardo Daniel</b>
    </td>
  </tr>
  <tr>
    <td align="center">
      <b>👨‍💻 Hernandez Ruiz Leny Javier</b>
    </td>
  </tr>
  <tr>
    <td align="center">
      <b>👨‍💻 Silverio Martinez Andres</b>
    </td>
  </tr>
  <tr>
    <td align="center">
      <b>👨‍💻 Rios Valdes Oscar</b>
    </td>
  </tr>
</table>


---

## 🎯 Project Objective

Implement from scratch the **core cryptographic functions** of a cold wallet for an account-based cryptocurrency. The project includes:

### Main Components

- 🔑 **Secure Key Storage**  
  Design and implement an encrypted storage system to protect private keys, using key derivation functions (KDF) and authenticated encryption.

- ✍️ **Transaction Signing**  
  Develop the mechanism to sign transactions using elliptic curve cryptography (Ed25519), ensuring authenticity and integrity.

- ✅ **Signature Verification**  
  Implement the cryptographic validation of received transactions, including protection against replay attacks using nonce systems.

- 🪙 **Address Management**  
  Derive cryptographic addresses from public keys using secure hash functions (SHA-256).

### Scope

> [!NOTE]
> This project simulates sending and receiving transactions **locally**, without requiring a network connection or blockchain state updates. It focuses on the fundamental cryptographic aspects of a cold wallet.

### Applied Cryptographic Concepts

- 🔑 Asymmetric key pair generation (Ed25519)
- 🔒 Authenticated encryption (AES-256-GCM)
- 🧂 Key derivation with Argon2id
- 📝 Digital signature and verification
- 🛡️ Protection against replay attacks
- 🔗 Data canonicalization for integrity

---

## 🚀 Installation

```bash
# Clone this repository
git clone "https://github.com/Kylos02/ColdCryptoWallet"

# Navigate to the project directory
cd ColdCryptoWallet

# Install dependencies
pip install cryptography customtkinter
py -m pip install customtkinter packaging
