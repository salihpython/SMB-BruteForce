SMB-BruteForce
SMB-BruteForce is a powerful, multi-threaded security tool developed for professionals to audit and verify the strength of Server Message Block (SMB) authentication. By automating the process of testing credential pairs against networked systems, it helps administrators identify weak passwords and potential entry points for lateral movement within an infrastructure.

## Setup

git clone https://github.com/salihpython/SMB-BruteForce.git                                                                                                       ls                                                                                                                                                                 cd SMB-BruteForcels


## Key Features
Multi-Threaded Performance: Engineered for high-speed execution, allowing for rapid testing of large wordlists without sacrificing system stability.

Protocol Compatibility: Supports various versions of the SMB protocol, targeting TCP Port 445 and legacy Port 139 (NetBIOS).

Dynamic Wordlist Support: Easily load custom dictionaries for both usernames and passwords to perform targeted or broad-spectrum attacks.

Session Management: Automatically handles connection handshakes, timeouts, and error states for a seamless auditing experience.

Detailed Output: Real-time feedback on successful hits, failed attempts, and account lockouts for efficient post-scan analysis.

## Use Cases
Vulnerability Assessments: Proactively identify accounts using default, leaked, or easily guessable credentials.

Penetration Testing: Simulate real-world brute-force and credential-spraying attacks to evaluate network defense resilience.

Compliance Auditing: Verify that organizational password policies and account lockout thresholds are being enforced correctly across the domain.

Network Hardening: Locate exposed SMB shares and ensure that only authorized, strong-credentialed users have access.

## Technical Overview
The tool operates by initiating an SMB negotiation with the target host. It attempts to authenticate using the provided credentials via the NTLM or Kerberos mechanisms (depending on configuration). This process is vital for testing the security of Windows File Sharing, Printer Sharing, and Remote Administration interfaces.

## Disclaimer
[!IMPORTANT]
This tool is strictly intended for educational purposes and authorized security auditing. Unauthorized access to private networks or systems is illegal and unethical. The developer assumes no liability for misuse or damage caused by this program. Always obtain written consent before testing.

## License
Distributed under the MIT License. See LICENSE for more information.
