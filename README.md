# Ethical Hacking Technical Report
## Client: Royal Financial Services
## Date: May 8, 2024
## Prepared by: Benedict Alam and Alliah Jane Arevalo

### Executive Summary:
This comprehensive report outlines the findings of the ethical hacking assessment conducted for Royal Financial Services. The primary objective of this assessment was to evaluate the security posture of the organization's network infrastructure, applications, and systems. Through a combination of penetration testing, vulnerability scanning, and social engineering techniques, several critical and high-risk vulnerabilities were identified across various components of Royal Financial Services' IT environment. This report presents a detailed analysis of these vulnerabilities and provides actionable recommendations for remediation to enhance the overall security resilience of the organization.

### Vulnerability Summary:
1. **Network Infrastructure:**
   - **Critical:** A Remote Code Execution vulnerability (CVE-2024-1234) was discovered in the Apache Struts framework (version 2.5.22) running on FinanceServer1. This vulnerability allows attackers to execute arbitrary code remotely, posing a significant risk to the confidentiality, integrity, and availability of sensitive financial data.
   - **High:** Misconfigured firewall rules were observed on FinanceServer2, permitting unrestricted access from external IP ranges to sensitive internal services such as SSH and RDP. This misconfiguration exposes the organization to potential unauthorized access and data exfiltration.

2. **Web Applications:**
   - **Critical:** The login form of the OnlineBankingApp was found to be vulnerable to SQL Injection attacks, enabling attackers to extract sensitive customer data from the database. This critical vulnerability poses a severe threat to the confidentiality of financial information and undermines customer trust.
   - **High:** Cross-Site Scripting (XSS) vulnerabilities were identified in the CustomerPortalApp, allowing attackers to inject and execute malicious scripts in users' browsers. Exploitation of these vulnerabilities could lead to session hijacking, unauthorized data disclosure, and financial fraud.

3. **Operating Systems:**
   - **Critical:** Outdated and unpatched operating systems (Windows Server 2008 R2) were observed on critical servers such as FinanceServer3 and FinanceServer4. These systems are susceptible to known exploits and malware, posing a significant risk to the stability and security of the organization's IT infrastructure.
   - **High:** Weak password policies were observed on domain user accounts, facilitating brute-force attacks and unauthorized access to sensitive financial systems and resources.

4. **Wireless Networks:**
   - **Critical:** Weak encryption protocols (WEP) were identified in use on the organization's wireless networks, allowing attackers to intercept and decrypt wireless traffic with relative ease. This vulnerability exposes sensitive financial data to potential eavesdropping and unauthorized access.

5. **Social Engineering:**
   - **High:** Several employees were found to have fallen victim to phishing emails, disclosing their credentials and sensitive information in response. This highlights a significant weakness in the organization's security awareness and training programs, increasing the risk of unauthorized access and data breaches.

6. **Database Security:**
   - **Critical:** The database server storing financial transactions was found to have default credentials for administrative access. This exposes the database to unauthorized access and potential data manipulation by malicious actors.
   
7. **Software Patching:**
   - **High:** Numerous critical security patches were found to be missing on servers and workstations across the organization's network. Failure to apply these patches exposes the systems to known vulnerabilities and exploits.

8. **Physical Security:**
   - **High:** Unauthorized personnel were observed accessing server rooms without proper authentication or supervision. This physical security lapse increases the risk of unauthorized access to critical infrastructure and data theft.

9. **Third-Party Software:**
   - **Critical:** A widely used third-party software component in the organization's infrastructure was found to have multiple known vulnerabilities with available exploits. Failure to update or patch this software increases the risk of exploitation by attackers.

10. **Insecure File Sharing:**
   - **High:** Employees were observed sharing sensitive financial documents via unsecured file-sharing platforms outside the organization's secure network, potentially exposing confidential information to unauthorized parties.

### Recommendations:
1. **Network Infrastructure:**
   - Immediately apply patches to mitigate the Remote Code Execution vulnerability in Apache Struts.
   - Conduct a thorough review of firewall configurations and implement access controls based on the principle of least privilege.

2. **Web Applications:**
   - Perform comprehensive code reviews and implement input validation mechanisms to prevent SQL Injection and XSS attacks.
   - Deploy web application firewalls (WAFs) and implement strict security headers to mitigate the risk of exploitation.

3. **Operating Systems:**
   - Establish a robust patch management process to ensure timely updates and security patches are applied to all systems.
   - Enforce the use of complex passwords and consider implementing multi-factor authentication (MFA) to enhance access controls.

4. **Wireless Networks:**
   - Upgrade wireless network encryption protocols to WPA2 or WPA3 to improve the confidentiality and integrity of wireless communications.
   - Implement network segmentation and access controls to limit exposure to wireless network vulnerabilities.

5. **Social Engineering:**
   - Conduct regular security awareness training sessions for all employees to educate them about the risks of phishing attacks and how to identify and report suspicious emails.
   - Implement email filtering and monitoring solutions to detect and block phishing attempts targeting employees.



### Conclusion:
The findings of the ethical hacking assessment underscore the critical importance of proactively addressing cybersecurity vulnerabilities within Royal Financial Services. By implementing the recommended remediation measures outlined in this report, Royal Financial Services can strengthen its security posture, safeguard sensitive financial data, and mitigate the risk of cyber threats and data breaches. It is imperative that these recommendations are prioritized and implemented promptly to ensure the continued trust and confidence of customers and stakeholders.

### Signature:
Benedict Alam
Ethical Hacker

Alliah Jane Arevalo
Ethical Hacker
