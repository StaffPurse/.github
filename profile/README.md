<div align="center">
  <img src="https://placehold.co/800x200/1e1e2e/a6accd.svg?text=StaffPurse" alt="StaffPurse Banner" width="100%" />

  <h1>StaffPurse</h1>
  <p><strong>Secure spend control and virtual card issuance for Nigeria's micro-businesses.</strong></p>

  <p>
    <a href="https://staffpurse.gitbook.io"><strong>Documentation</strong></a> ·
    <a href="https://t.me/+Gflo5jZStw1jMjE0"><strong>Community Telegram</strong></a>
  </p>
</div>

## 📖 About StaffPurse

StaffPurse is a spend control platform tailored for Nigeria's informal micro-businesses. It enables instant virtual card issuance with a focus on self-custody and high transparency.

By leveraging the Stellar blockchain and Soroban smart contracts, StaffPurse anchors daily Merkle roots of off-chain spend records. This approach provides a mathematically verifiable audit trail for business owners and third-party auditors while preserving sensitive employee and business data off-chain.

## 🏗️ Our Open Source Ecosystem

We build our tools in the open. Our core architecture consists of three main repositories:

### 📱 [StaffPurse App](https://github.com/StaffPurse/staffpurse-app)
The main Flutter mobile application (powered by BMONI) and our Deno-based Supabase Edge Functions. It enforces self-custody via secure hardware-enclaves for EIP-191 signing and handles the daily cron jobs to build Merkle trees for the daily spend proofs.

### 🔗 [StaffPurse Contracts](https://github.com/StaffPurse/staffpurse-contracts)
The on-chain transparency layer written in Rust for the Soroban smart contract platform. It acts as an immutable key-value store, securely anchoring daily Merkle roots to the Stellar blockchain.

### 🌐 [StaffPurse Web](https://github.com/StaffPurse/staffpurse-web)
A lightweight Next.js (React/TypeScript) public verification dashboard. It queries both the off-chain database and the on-chain Soroban contract to perform native client-side cryptographic hash validation, ensuring all records perfectly match the anchored root.

## 🤝 Contributing

We welcome contributions from the community! Check out the `CONTRIBUTING.md` and `SECURITY.md` files in our respective repositories to get started. All PRs must pass CI gates and follow our code quality standards.
