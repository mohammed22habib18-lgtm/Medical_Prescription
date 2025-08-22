Here’s a clean and professional `README.md` file for your **Medical Prescription Ledger** project based on blockchain:

---

```markdown
# 🩺 Medical Prescription Ledger (Blockchain-Based)

A simple blockchain-based ledger system for securely issuing, revoking, and verifying medical prescriptions. This project demonstrates how blockchain can help prevent fraud, ensure data integrity, and provide transparency in medical records management.

---

## 📦 Features

- ✅ **Issue Prescriptions**: Doctors can issue prescriptions for patients.
- ❌ **Revoke Prescriptions**: Revocation is allowed if an error or misuse is discovered.
- 🔍 **Verify Prescriptions**: Patients and pharmacies can verify if a prescription is still valid.
- ⛓️ **Blockchain-Powered**: Ensures data integrity with proof-of-work and linked blocks.
- 🗃️ **Persistent Storage**: Ledger is saved to a local JSON file (`prescriptions_chain.json`).

---

## 📁 Project Structure

```

prescription\_blockchain/
├── prescription\_blockchain.py   # Main blockchain logic & CLI
├── prescriptions\_chain.json     # Ledger file (auto-generated)
└── README.md

````

---

## 🚀 Getting Started

### 🔧 Prerequisites

- Python 3.7+
- No external libraries required

### ▶️ Run the Program

```bash
python prescription_blockchain.py
````

---

## 🖥️ Menu Options

```text
--- Medical Prescription Ledger ---
1) Issue prescription
2) Revoke prescription
3) Verify prescription
4) Show chain length & validity
5) List last N blocks
0) Exit
```

---

## 💡 Example Usage

### Issue a Prescription

```
Prescription ID: RX001
Patient name: Alice Smith
Medication: Amoxicillin
Dosage: 500mg
Issued on: 2025-08-22
Doctor: Dr. John Miller
```

➡️ Output:

```
[✓] Issued RX001 in block #1.
```

---

## 📂 Data Format (Block)

Each block contains:

```json
{
  "index": 2,
  "timestamp": 1692712390.123,
  "data": {
    "type": "REVOKE",
    "prescription": {
      "prescription_id": "RX001",
      "patient_name": "Alice Smith",
      "medication": "Amoxicillin",
      "dosage": "500mg",
      "issued_on": "2025-08-22",
      "doctor": "Dr. John Miller",
      "status": "REVOKED",
      "remarks": "Allergic reaction"
    }
  },
  "prev_hash": "e3a25b...",
  "nonce": 9123
}
```

---

## ✅ Blockchain Rules

* All blocks require a valid **proof-of-work** (hash must start with `"00"`).
* All blocks are linked via **SHA-256 hashes**.
* Tampering with any block will invalidate the chain.

---

## 🛡️ Security & Integrity

* Immutable ledger (blocks cannot be modified without breaking hash links)
* Tamper detection via built-in validity checker
* Proof-of-work protects against unauthorized block insertion

---

## 📘 Future Ideas

* Integration with hospital databases or electronic health records (EHR)
* Web or mobile frontend for patients & doctors
* QR code for prescription verification
* Smart contract backend (e.g., Ethereum or Hyperledger)

---

## 👨‍⚕️ Author

Built with ❤️ for learning and demonstrating blockchain's use in healthcare systems.

---

## 📄 License

This project is licensed under the MIT License.

```

---

Let me know if you'd like a version tailored for a **GitHub repository**, with badges, project boards, or contribution guidelines!
```
