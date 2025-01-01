# Software and Database Security Projects  

This repository showcases two key software security audit projects conducted in collaboration with EPITA as part of the **Software and Database Security** course. These projects focused on analyzing vulnerabilities in two locally run desktop applications—a **Banking App** and a **Stock Management App**—and proposing remediations to enhance their security.  

**Achievement**: Our team received the **highest marks in the entire course** (20/20 for the project), with individual grades ranging from **17/20 to 20/20**, highlighting the thoroughness and impact of our work.  

## Projects Overview  

### 1. [**Banking App Security Audit**  ](https://github.com/Mf4z/BankingApp)
   - **Objective**: Audit and identify vulnerabilities in a desktop banking application and recommend remediations.  
   - **Key Findings**:  
     - Password hashing without sufficient computational effort (CWE-916).  
     - Use of hashed passwords instead of raw passwords for authentication (CWE-836).  
   - **Remediations**:  
     - Implemented salted hashing using **Bcrypt** for secure password storage.  
     - Suggested adoption of multi-factor authentication (MFA) to enhance security.  
   - **Impact**: Increased resilience against brute-force attacks and replay exploits by enforcing secure password management practices.
   - **Detailed Report**: [Banking App Security Audit Report (PDF)](https://github.com/Mf4z/SDS-Audit-Project/blob/main/EPITA/Bank_app/report/SDS_Report_Exams_Bonus_Bank_App.pdf)  

### 2. **Stock Management App Security Audit**  
   - **Objective**: Assess vulnerabilities in a desktop stock application and implement security improvements.  
   - **Key Findings**:  
     - Hardcoded credentials and plaintext storage of passwords (CWE-259, CWE-256).  
     - SQL injection vulnerabilities (CWE-89).  
     - Improper access control and permission assignment (CWE-284, CWE-732).  
   - **Remediations**:  
     - Replaced plaintext passwords with hashed passwords and unique salts.  
     - Transitioned to a three-tier architecture (Client → API → Database) to isolate the database from direct access.  
     - Utilized parameterized queries and strict input validation to mitigate SQL injection risks.  
   - **Impact**: Strengthened access control, reduced the risk of credential leaks, and secured communication channels.
   - **Detailed Report**: [Stock Management App Security Audit Report (PDF)](https://github.com/Mf4z/SDS-Audit-Project/blob/main/EPITA/Stock_app/report/SDS_Report_Exams.pdf)

## Skills and Technologies Used  
- **Programming and Tools**:  
  - **Languages**: SQL, Bash scripting.  
  - **Security Tools**:  
    - **Wireshark**: Packet analysis for identifying vulnerabilities.  
    - **Echo Mirage**: Proxy for data interception and vulnerability testing.  
    - **HxD**: Hex editor for analyzing compiled binaries.  
    - **CyberChef**: Hashing and encryption validation.  
    - **HeidiSQL**: Database management and testing.  
  - **Database Systems**: MySQL.  
- **Security Concepts**:  
  - Vulnerability identification and scoring using **CVSS**.  
  - Cryptographic hashing techniques (e.g., Bcrypt).  
  - Access control mechanisms and principle of least privilege.  
  - Secure architecture design with three-tier systems.  
- **Collaboration**:  
  - Conducted as part of a 3-person team using Agile principles.  
  - Delivered comprehensive audit reports with detailed remediations.  

## Achievements  
- Identified and mitigated over 10 critical and high-severity vulnerabilities across two applications.  
- Improved app security posture through encryption, hashing, and secure architecture redesign.  
- Gained hands-on experience in using industry-standard security tools and techniques.  
- Achieved the highest course grade with exemplary feedback on report quality and thoroughness.  

## Contribution  
This project was conducted by:  
- **Marwan Mustapha Mai**  
- **Omar Issa**  
- **Bishal Udash**  

Our team collaboratively performed vulnerability assessments, developed remediation strategies, and implemented security enhancements in the audited applications. 