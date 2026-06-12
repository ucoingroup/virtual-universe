# Virtual Universe

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Discord](https://img.shields.io/discord/HWsweV6fFy?label=Discord&logo=discord)](https://discord.gg/HWsweV6fFy)
[![GitHub Stars](https://img.shields.io/github/stars/ucoingroup/virtual-universe)](https://github.com/ucoingroup/virtual-universe/stargazers)
[![GitHub Forks](https://img.shields.io/github/forks/ucoingroup/virtual-universe/network)
[![GitHub Issues](https://img.shields.io/github/issues/ucoingroup/virtual-universe)](https://github.com/ucoingroup/virtual-universe/issues)
[![GitHub Pull Requests](https://img.shields.io/github/issues-pr/ucoingroup/virtual-universe)](https://github.com/ucoingroup/virtual-universe/pulls)

> A project exploring how EACO ($eaco) integrates with the virtual universe and facilitates circulation and usage within it.

## 🌟 About EACO

EACO ($eaco) is an innovative community currency — the only $eaco in the universe and on Earth.

| Item | Value |
|------|-------|
| **Token Ticker** | $eaco |
| **Contract Address (CA)** | `DqfoyZH96RnvZusSp3Cdncjpyp3C74ZmJzGhjmHnDHRH` |
| **Mission** | Promote environmental protection and sustainable development |
| **Tagline** | EACO — Earth's Best Coin |
| **Blockchain** | Solana |
| **Community** | [Discord](https://discord.gg/HWsweV6fFy) |

## ✨ Features

- 🪙 **Community Currency** — Innovative decentralized currency system
- 🌍 **Sustainable Development** — Environmental protection focus
- 🔗 **Blockchain Native** — Built on Solana ecosystem
- 🤝 **Community Driven** — Open participation and governance
- 🚀 **Virtual Universe Integration** — Exploring new circulation paradigms
- 🔒 **Secure & Transparent** — Open-source and verifiable

## 📁 Project Structure

```
virtual-universe/
├── .gitignore      # Standard ignore rules
├── LICENSE         # MIT License
└── README.md        # Project documentation
```

## 🚀 Quick Start

### Prerequisites

- Git
- Node.js (v16 or higher)
- Solana CLI (optional, for advanced usage)

### Installation

```bash
# Clone the repository
git clone https://github.com/ucoingroup/virtual-universe.git
cd virtual-universe

# Install dependencies
npm install @solana/web3.js
```

### Verify Installation

```bash
# Check Node.js
node --version
npm --version

# Check Solana CLI (optional)
solana --version
```

## 📖 Usage

This repository focuses on documentation and community alignment. Contributions for virtual-universe integrations are welcome.

### Query EACO Token Info

```javascript
const solanaWeb3 = require('@solana/web3.js');

const EACO_MINT_ADDRESS = 'DqfoyZH96RnvZusSp3Cdncjpyp3C74ZmJzGhjmHnDHRH';
const connection = new solanaWeb3.Connection(
  solanaWeb3.clusterApiUrl('mainnet-beta'),
  'confirmed'
);

console.log('EACO CA:', EACO_MINT_ADDRESS);
console.log('Network: Solana Mainnet Beta');
```

### Check EACO Balance

```javascript
async function getEacoBalance(walletAddress) {
  const publicKey = new solanaWeb3.PublicKey(walletAddress);
  const accounts = await connection.getParsedTokenAccountsByOwner(publicKey);
  const eaco = accounts.value.find(a =>
    a.account.data.parsed.info.mint === EACO_MINT_ADDRESS
  );
  return eaco ? eaco.account.data.parsed.info.tokenAmount.uiAmount : 0;
}
```

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-idea`)
3. Commit your changes (`git commit -m 'Add amazing idea'`)
4. Push to the branch (`git push origin feature/amazing-idea`)
5. Open a Pull Request

## 🔗 Useful Links

- [EACO on Solana Explorer](https://explorer.solana.com/address/DqfoyZH96RnvZusSp3Cdncjpyp3C74ZmJzGhjmHnDHRH)
- [Solana Documentation](https://docs.solana.com/)
- [Discord Community](https://discord.gg/HWsweV6fFy)

## 📄 License

MIT License — see [LICENSE](LICENSE) file.

---

Made with ❤️ by [ucoingroup](https://github.com/ucoingroup)