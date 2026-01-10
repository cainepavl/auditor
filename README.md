# Credential Exposure Auditor 🛡️

A privacy-focused Python security tool used to audit passwords against known data breaches. This tool utilizes the **Have I Been Pwned (HIBP) API** and implements the **k-Anonymity** model to ensure that your full credentials never leave your local machine.

## 🔒 Security & Privacy First
This auditor is designed with a "Zero-Trust" approach to user data:

* **k-Anonymity Model:** Only the first 5 characters of the SHA-1 password hash are sent to the API. The full hash and the plain-text password are never transmitted over the network.
* **Zero-Trace Input:** Uses the `getpass` module to ensure that passwords entered into the terminal are not echoed to the screen and are not stored in your shell's command history (e.g., `.bash_history` or `.zsh_history`).
* **Hash-Masking:** Local comparison of hash suffixes ensures 100% anonymity from the API provider.



## 🛠️ Features
* **Real-time Breach Detection:** Cross-references credentials against billions of leaked accounts.
* **Cross-Platform Support:** Fully compatible with Windows, macOS, and Linux via `colorama`.
* **Clean Interface:** Clear, color-coded terminal output for immediate risk assessment.

## 🚀 Getting Started

### Prerequisites
* Python 3.x
* `requests` library
* `colorama` library

### Installation
1. Clone the repository:
   ```bash
   git clone [https://github.com/cainepavl/credential-auditor.git](https://github.com/cainepavl/credential-auditor.git)
   cd credential-auditor
