# Windows Server 2019 Hardening & Auditing Project

## Objective
This project focuses on hardening and auditing a Windows Server 2019 environment using the [CIS Microsoft Windows Server 2019 Benchmark](https://www.cisecurity.org/benchmark/microsoft_windows_server). The goal is to implement security configurations to enhance system security and compliance.

## Steps

### Step 1: Initial Setup & Benchmark Selection
- Configured a virtual machine running Windows Server 2019 and selected the CIS benchmark as the security guideline.

### Step 2-6: Password Policy Hardening
- **Step 2:** Enforced password history to 24 or more passwords. ![Screenshot](./screenshot2.png)
- **Step 3:** Reviewed the default value of this policy. ![Screenshot](./screenshot3.png)
- **Step 4:** Set the maximum password age to 365 or fewer days, but not 0. ![Screenshot](./screenshot4.png)
- **Step 5-6:** Applied a 90-day password reset policy. ![Screenshot](./screenshot5.png) ![Screenshot](./screenshot6.png)

### Step 7-10: Strengthening Password Requirements
- **Step 7:** Ensured minimum password age was 1 or more days. ![Screenshot](./screenshot7.png)
- **Step 8:** Minimum password length defaulted to 7 characters. ![Screenshot](./screenshot8.png)
- **Step 9:** Increased minimum password length to 14 characters. ![Screenshot](./screenshot9.png)
- **Step 10:** Verified password complexity requirements were enabled. ![Screenshot](./screenshot10.png)

### Step 11: Secure Password Storage
- **Step 11:** Ensured 'Store passwords using reversible encryption' was disabled. ![Screenshot](./screenshot11.png)

### Step 12-15: Account Lockout Policy
- **Step 12:** Account lockout duration was not defined by default. ![Screenshot](./screenshot12.png)
- **Step 13:** Set account lockout duration to 15 minutes. ![Screenshot](./screenshot13.png)
- **Step 14:** Ensured lockout threshold was set to 5 or fewer invalid logon attempts. ![Screenshot](./screenshot14.png)
- **Step 15:** Configured reset lockout counter after 15 minutes. ![Screenshot](./screenshot15.png)

### Step 16-21: User & Network Access Controls
- **Step 16:** Restricted Access Credential Manager as a trusted caller to No One. ![Screenshot](./screenshot16.png) ![Screenshot](./screenshot17.png)
- **Step 18-19:** Configured network access settings for authenticated users. ![Screenshot](./screenshot18.png) ![Screenshot](./screenshot19.png)
- **Step 20:** Restricted "Act as part of the operating system" to No One. ![Screenshot](./screenshot20.png)
- **Step 21:** Limited "Add workstations to domain" to Administrators. ![Screenshot](./screenshot21.png)

### Step 22-24: Print Spooler Security
- **Step 22:** Audited Print Spooler settings via registry. ![Screenshot](./screenshot22.png)
- **Step 23:** Disabled Print Spooler for Domain Controllers. ![Screenshot](./screenshot23.png) ![Screenshot](./screenshot24.png)

### Step 25-26: Windows Firewall Configuration
- **Step 25:** Enabled Windows Firewall: Domain: Firewall state. ![Screenshot](./screenshot25.png)
- **Step 26:** Configured inbound connections to be blocked by default. ![Screenshot](./screenshot26.png)

## Conclusion
This project successfully implemented Windows Server 2019 hardening measures, covering:

✔️ Enforcing strong password policies  
✔️ Implementing account lockout policies  
✔️ Restricting user and network access controls  
✔️ Disabling unnecessary services like Print Spooler  
✔️ Configuring Windows Firewall for security enforcement  

This security hardening ensures compliance with the CIS Benchmark and enhances the overall security posture of the system. 🚀
