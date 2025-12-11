🔍 Task 3 – Basic Vulnerability Scan on Local Machine

📌 Objective

Perform a basic vulnerability scan on your PC using a free vulnerability scanning tool to identify security risks and document the findings.

⸻

🛠️ Tools Used

You may use any free vulnerability scanner, such as:
	•	OpenVAS Community Edition
	•	Nessus Essentials ✔️ (Used in this task)

⸻

🖥️ Setup and Scan Process

1. Install the Vulnerability Scanner

Nessus Essentials was installed successfully and the user account was created.

2. Set the Scan Target

Local machine IP was selected as the target for scanning:
192.168.136.129

3. Start the Scan

A Full Vulnerability Scan was initiated for the local machine.

4. Wait for Scan Completion

Scan completed successfully (typical duration 30–60 minutes).

5. Review the Results

The scan produced a detailed list of vulnerabilities with severity levels.

⸻

🚨 Identified Critical Vulnerabilities

1. Node.js Multiple Vulnerabilities

Severity: Critical
Description:
Node.js HTTP servers are vulnerable to specially crafted chunked-encoding requests which may lead to resource exhaustion and Denial of Service (DoS).

Affected Versions:
	•	Node.js 18.x < 18.19.1
	•	Node.js 20.x < 20.11.1
	•	Node.js 21.x < 21.6.2

CVE IDs:
CVE-2023-46809, CVE-2024-21890, CVE-2024-21891, CVE-2024-21892, CVE-2024-21896, CVE-2024-22017, CVE-2024-22019

Fix:
Upgrade Node.js to 18.19.1 / 20.11.1 / 21.6.2 or later.

⸻

2. Python Tornado Library DoS Vulnerability

Severity: High
CVE: CVE-2025-47287

Description:
A DoS condition may occur due to improper handling of specific requests.

Fix:
Update Tornado to version 6.5.0 or later.

⸻

3. SSL Certificate Cannot Be Trusted

Severity: Medium

Description:
The SSL certificate used by the service is either self-signed, expired, or misconfigured.

Fix:
Use a valid SSL certificate from a trusted Certificate Authority (CA) or configure it correctly.

⸻

🧪 Conclusion

This task helped identify several vulnerabilities on the local machine using Nessus Essentials. The results highlight the importance of keeping software updated and ensuring proper SSL configurations. Applying the recommended fixes will significantly reduce the attack surface and improve the overall system security posture.
