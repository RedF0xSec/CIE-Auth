# Project 007 - Secure Online Auction System

## Overview
This project aims to create a **secure online auction platform** that leverages the **Italian Electronic Identity Card (CIE)** for user authentication. The system ensures that only verified users can participate in auctions, enhancing **security, integrity, and transparency** in transactions.

**Note:** This project and its documentation are in **Italian**. It was developed as part of the **Algorithms and Protocols for Security** course in the first year of the Master's Degree in Computer Engineering at the **University of Salerno**.

## Features
- **Authentication via CIE**: Users must authenticate with their **Electronic Identity Card (CIE)** before accessing the auction platform.
- **Credential Verification**: Secure credential issuance and verification through a dedicated credential server.
- **Threat Mitigation**: The system is designed to counteract various threats, including **man-in-the-middle attacks, phishing, and identity theft**.
- **Confidentiality & Integrity**: Uses **Transport Layer Security (TLS 1.3)** and **Merkle Trees** to ensure secure communication and data validation.
- **Zero-Knowledge Proofs**: Implements **Schnorr’s Zero-Knowledge Protocol** for secure identity verification.
- **Efficient Credential Management**: Includes **expiration date verification** and **fraud prevention mechanisms** for compromised identity cards.

## System Components
- **Auction Server**: Handles auction transactions and enforces access policies.
- **Credential Server**: Issues and verifies user credentials based on CIE authentication.
- **User Client**: Requests credentials and interacts with the auction platform.
- **Government Authorities (IPZS & Ministry of the Interior)**: Trusted entities responsible for issuing and managing CIE.

## Workflow
1. **User connects** to the auction server, which redirects to the credential server.
2. **Credential request**: The user requests access credentials from the credential server.
3. **CIE Authentication**: The user digitally signs the credential request with their CIE.
4. **Credential issuance**: The credential server verifies the request and issues the necessary credentials.
5. **Auction access**: The user submits their credentials to the auction server for final verification and access.

## Security Model
The system considers multiple attack vectors and adversaries, including:
- **Passive Eavesdropping (Sniffy McSnifferson)**
- **Credential Theft (Mariuolo)**
- **Denial-of-Service Attacks (Doszilla)**
- **Phishing Attacks (Pescatore)**
- **Insider Threats (Waldo the Intruder)**
- **Identity Fraud (Bonnie & Clyde Collaboration)**

## Implementation
The project includes **bash scripts** simulating interactions between the user, auction server, and credential server. Key technologies and techniques include:
- **ECDSA Digital Signatures** for authentication
- **Merkle Trees** for secure credential management
- **TLS 1.3** for encrypted communication
- **Zero-Knowledge Proofs** for authentication

## Skills Acquired
### Soft Skills
| Skill | Description |
|-------|-------------|
| **Problem-Solving** | Identified security risks and designed appropriate countermeasures. |
| **Critical Thinking** | Evaluated different authentication and encryption strategies. |
| **Collaboration & Teamwork** | Worked effectively within Group 007 to coordinate implementation efforts. |
| **Adaptability** | Learned and applied new security concepts and cryptographic techniques. |
| **Project Management** | Organized tasks, set deadlines, and ensured successful project completion. |
| **Technical Communication** | Documented and presented findings in a clear, structured manner. |

### Hard Skills
| Skill | Description |
|-------|-------------|
| **Cryptography** | Knowledge about ECDSA digital signatures, TLS 1.3, Zero-Knowledge Proofs for authentication and all others cryptographic tools. |
| **Threat Modeling** | Identified potential adversaries and applied security strategies to mitigate threats. |
| **Bash Scripting** | Developed scripts to simulate interactions between system components. |
| **Merkle Trees** | Utilized Merkle Trees for secure and efficient credential verification. |
| **Identity Management** | Integrated authentication via the Italian Electronic Identity Card (CIE). |
| **Secure Software Development** | Designed and implemented a structured security model for the auction system. |

## How to Run the Simulation
1. **Navigate to the project directory**:
   ```sh
   cd WP4
   ```
2. **Run the simulation script**:
   ```sh
   bash ./simulazione.sh
   ```
3. **Follow the on-screen instructions** to simulate credential issuance and auction access.

## Future Enhancements
- **Decentralized server architecture** for improved resilience
- **Blockchain integration** for enhanced transparency
- **Advanced fraud detection mechanisms** using AI

## Contact
For questions or contributions, please contact **Elena Falcone** at [elenafalcone2001@gmail.com].

