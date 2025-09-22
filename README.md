# 🚀 Soundness CLI Guide

My personal guide for setting up and using the **Soundness Testnet**.  
Includes installation steps, account import, key management, and basic commands.

---

1️⃣ System Preparation  

Update your system and install required dependencies:  

```bash
sudo apt update && sudo apt upgrade -y
sudo apt install pkg-config libssl-dev openssl
2️⃣ Install SoundnessUP

Download and run the installer:
```bash
curl -sSL https://raw.githubusercontent.com/soundnesslabs/soundness-layer/main/soundnessup/install | bash
source ~/.bashrc

Install Rust (if not installed):
```bash
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs/ | sh
source $HOME/.cargo/env

Update & verify installation:
```bash
soundnessup install
soundnessup upgrade

3️⃣ Import Existing Account

Recover your old account with mnemonic:
```bash
soundness-cli key import --name my-key --mnemonic "your secret phrase"

4️⃣ Create a New Key / Pubkey

Generate a fresh key:
```bash
soundness-cli key generate --name my-key

---

## ✨ Personal Notes
- This testnet is my personal learning and experimentation playground.  
- Every error is not a failure, but a chance to improve.  
- Soundness Testnet = where I sharpen my Web3 developer skills.  

