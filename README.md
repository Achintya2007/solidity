![Screenshot 2025-05-26 134929](https://github.com/user-attachments/assets/5f54efa2-4a84-46f4-89de-925d2552e4e8)
# 📦 Supply Chain Transparency Platform

A Solidity-based smart contract enabling end-to-end **tracking**, **verification**, and **transparency** in supply chain systems. This platform ensures product integrity by recording location updates, status changes, and authorized user interactions on the Ethereum blockchain.

---

## 🚀 Features

- **Register Products**: Manufacturers can register products with metadata and an initial location.
- **Track Journey**: Update product location, status, and timestamp as it moves through the supply chain.
- **Access Control**: Fine-grained access control ensures only authorized participants can modify or view product details.
- **Product Verification**: Anyone can verify if a product is authentic by checking its existence.
- **Audit Trail**: Every movement and handler is logged to enable historical traceability.

---

## 🛠️ Smart Contract Details

### ✅ Contract Name
`Project`

### 📄 SPDX License
MIT

### 🧱 Solidity Version
`^0.8.19`

---

## 📚 Core Data Structures

### `Product` Struct

```solidity
struct Product {
    uint256 id;
    string name;
    string description;
    address manufacturer;
    uint256 timestamp;
    string currentLocation;
    ProductStatus status;
    string[] locationHistory;
    uint256[] timeHistory;
    address[] handlers;
    bool exists;
}
contract address:0x2dC1770d9C9F006F1F0c68DD654E61cB7282c183
