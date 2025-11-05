# Decentralized Healthcare Prescription & Records Management System

This project aims to provide a secure and transparent way to store, share, and manage medical records and prescriptions using **Blockchain, IPFS, and Machine Learning**. The system ensures that patients have full control over their health data, while doctors can securely issue prescriptions and access patient records only with proper authorization.

---

## 🚀 Key Features

- **Patient-Controlled Access:** Patients can grant or revoke access to their medical records.
- **Secure Prescription Storage:** Prescriptions are stored on **IPFS**, and their hash is saved on the **Ethereum Blockchain** to ensure authenticity.
- **Role-Based Access Control (RBAC):** Doctors, Patients, and Medical Staff each have specific permissions.
- **Disease Prediction Support:** A **Random Forest ML model** assists in predicting diseases based on symptoms.
- **Wallet-Based Login:** Users log in using **MetaMask** for secure authentication without usernames/passwords.

---

## 🛠️ Tech Stack Used

| Layer | Technology |
|------|------------|
| Frontend | React.js |
| Backend | Node.js, Express.js |
| Machine Learning | Python, Flask, Random Forest Classifier |
| Blockchain | Ethereum (Solidity, Web3.js, MetaMask) |
| Storage | IPFS (via Pinata) |
| Database | MongoDB |

---

## 🔐 System Workflow (Simplified)

1. **User Login:** Wallet authentication using MetaMask.
2. **Role Assignment:** Users are categorized as Patient / Doctor / Medical Staff.
3. **Prescription Generation:** Doctors generate prescriptions and upload them.
4. **IPFS Storage:** Prescription files are stored in IPFS → returns a unique hash.
5. **Blockchain Entry:** Hash is stored in a Smart Contract for verification.
6. **Access Control:** Patients decide who can view or use their records.

---

## 📊 Machine Learning Module

- Model: **Random Forest Classifier**
- Input: Patient symptoms
- Output: Predicted disease suggestion
- Purpose: Assists doctors in accurate diagnosis

---

## 🧪 How to Run the Project (High-Level)

```bash
# Clone the project
git clone <your-repo-link>

# Backend Setup
cd backend
npm install
npm start

# ML Model Server
cd ml-model
pip install -r requirements.txt
python app.py

# Frontend Setup
cd frontend
npm install
npm start
