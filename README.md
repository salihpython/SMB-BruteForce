SMB-BruteForce is a professional-grade, high-performance security auditing tool designed to evaluate the robustness of Server Message Block (SMB) authentication mechanisms. In modern network environments, SMB is a primary target for lateral movement and unauthorized data access. This tool provides security researchers, penetration testers, and system administrators with a reliable way to identify weak credentials and misconfigured authentication policies before malicious actors can exploit them.

By automating the systematic testing of username and password combinations, SMB-BruteForce streamlines the process of discovering "low-hanging fruit"—accounts with default, common, or easily guessable passwords that often serve as the first link in a breach chain.

Key Features
🚀 High-Concurrency Engine
Built with performance in mind, the tool utilizes advanced multi-threading to handle hundreds of authentication attempts per second. This ensures that even large-scale network segments can be audited in a fraction of the time required by traditional scripts.

🛠️ Protocol Versatility
The tool is engineered to interact with multiple versions of the SMB protocol. It can target:

Direct TCP (Port 445): For modern Windows and Samba environments.

NetBIOS over TCP/IP (Port 139): To ensure coverage for legacy systems and older infrastructure.

📂 Flexible Dictionary Management
Users can supply custom wordlists for both usernames and passwords. Whether you are performing a Credential Spraying attack (testing one password against many users) or a Traditional Brute-Force (testing many passwords against one user), the tool adapts to your specific audit requirements.

🔍 Intelligent Session Handling
The engine manages the complexities of the SMB handshake, including dialect negotiation and session setup. It is designed to gracefully handle connection timeouts, network jitter, and remote server resets without crashing.

📊 Real-Time Analytics & Logging
Every attempt is logged with precision. Successful authentications are highlighted for immediate attention, while failure codes are analyzed to distinguish between "Wrong Password," "Account Locked," or "Connection Refused."

Technical Use Cases
1. Internal Penetration Testing
Simulate the tactics of real-world adversaries who have gained a foothold in a network and are attempting to escalate privileges or move laterally to file servers and domain controllers.

2. Password Policy Enforcement
Quantify the effectiveness of your organization's password policy. Use this tool to prove that even if a policy exists, users may still be using weak credentials that bypass standard filters.

3. Red Team Operations
Incorporate SMB-BruteForce into automated red team pipelines to identify exposed shares and administrative interfaces that rely on weak NTLM authentication.

Installation & Setup
Bash
# Clone the repository
git clone https://github.com/salihpython/SMB-BruteForce.git

# Navigate to the directory
cd SMB-BruteForce

# Install dependencies
pip install -r requirements.txt
