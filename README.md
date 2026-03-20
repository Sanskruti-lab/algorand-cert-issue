# algorand-cert-issue
# 🎓 Algorand Digital Certificate Issuer

A blockchain-based system to issue and verify tamper-proof digital certificates on the **Algorand** network using Algorand Standard Assets (ASA).

---

## 📌 Project Overview

This project enables institutions (schools, bootcamps, organizations) to issue digital certificates as unique tokens on the Algorand blockchain. Each certificate is:

- **Tamper-proof** — stored immutably on-chain
- **Instantly verifiable** — anyone can verify authenticity using the transaction ID
- **Decentralized** — no central authority needed to confirm validity

---

## 🚀 Features

- Issue a certificate as an Algorand Standard Asset (ASA)
- Attach certificate metadata (recipient name, course, date)
- Verify a certificate using its Asset ID
- Built on Algorand TestNet (safe for learning, no real funds needed)

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| Python 3.x | Core programming language |
| `py-algorand-sdk` | Interact with Algorand blockchain |
| Algorand TestNet | Test environment (free) |
| Pinata / IPFS *(future)* | Store certificate metadata off-chain |

---

## 📁 Project Structure

```
algorand-cert-issuer/
│
├── README.md               # Project documentation
├── requirements.txt        # Python dependencies
├── config.py               # Network and account configuration
├── issue_certificate.py    # Script to issue a certificate as ASA
├── verify_certificate.py   # Script to verify a certificate by Asset ID
└── sample_output/
    └── sample_cert.json    # Example certificate metadata
```

---

## ⚙️ Setup Instructions

### 1. Clone the Repository
```bash
git clone https://github.com/YOUR_USERNAME/algorand-cert-issuer.git
cd algorand-cert-issuer
```

### 2. Install Dependencies
```bash
pip install -r requirements.txt
```

### 3. Create a TestNet Account
- Visit [Algorand Dispenser](https://testnet.algoexplorer.io/dispenser) to fund a free TestNet wallet
- Or use [AlgoKit](https://developer.algorand.org/algokit/) to set up locally

### 4. Configure Your Account
Edit `config.py` and add your TestNet account mnemonic.

### 5. Issue a Certificate
```bash
python issue_certificate.py
```

### 6. Verify a Certificate
```bash
python verify_certificate.py --asset-id YOUR_ASSET_ID
```

---

## 🔐 Security Note

> ⚠️ Never commit your private key or mnemonic to GitHub. Use environment variables or a `.env` file (add `.env` to `.gitignore`).

---

## 🌐 Resources

- [Algorand Developer Docs](https://developer.algorand.org/)
- [py-algorand-sdk Docs](https://py-algorand-sdk.readthedocs.io/)
- [Algorand TestNet Explorer](https://testnet.algoexplorer.io/)
- [What is an ASA?](https://developer.algorand.org/docs/get-details/asa/)

---

## 📄 License

MIT License — free to use and modify.

---

## 👤 Author

Built as part of an Algorand blockchain development course.
