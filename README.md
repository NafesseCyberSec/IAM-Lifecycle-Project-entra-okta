# IAM-Lifecycle-Project-entra-okta
A hands-on project simulating identity lifecycle and SCIM-based provisioning using Azure Entra ID and Okta.
IAM Lifecycle Automation Project
This project replicates a real-world Identity and Access Management (IAM) environment using free tools like Azure Entra ID and Okta. It simulates user provisioning through SCIM-like workflows, multi-factor authentication (MFA), SAML-based single sign-on (SSO), and lifecycle automation using an HR data source.

🧰 Tools Used
Azure Entra ID
Okta
Excel (simulating HR system)
SCIM-style provisioning
⚙️ What This Project Covers
🔄 Lifecycle Automation
HR adds user to Excel (simulating an HR system like Workday)
User is created in IDP (Entra ID or Okta)
Group assignment & app access automated
🔐 Access Governance
MFA policies & Conditional Access
SSO with SAML
Least Privilege & Access Reviews
🔁 SCIM Provisioning (Simulated)
Provisioning based on department:

Finance users → Assigned to Finance group → Auto-provisioned access to Finance apps
🧾 IAM Lab Summary
🔹 Azure / Entra ID
Created users
Assigned security groups
Enforced MFA
Built conditional access policies
🔹 Okta
Created users/groups
Enabled MFA with Okta Verify
Configured SSO (SAML)
Created custom attribute: departmentCode

🧑‍💼 Example Provisioned User
This user was provisioned from the simulated HR system (Excel) into both Azure Entra ID and Okta using SCIM-style automation.

Attribute	Value
FirstName - Nafesse
LastName - Dulaney
Department - Finance
Job Title - Financial Analyst I
Email - nafessedulaney@outlook.com

Provisioned into:

✅ Azure Entra ID (MFA enforced, Group: Finance, App access assigned)
✅ Okta (MFA via Okta Verify, Group: Finance, SSO enabled, Custom Attribute: departmentCode: FIN)

 Project Screenshot Overview
The following screenshot provides a high-leve User Created in Entra IDl view of the Identity and Access Management (IAM) lifecycle flow implemented in this simulation project. It highlights key steps across both Entra ID and Okta:

User Created in Entra ID
<img width="1173" height="612" alt="image" src="https://github.com/user-attachments/assets/edffb357-c09a-495e-8fc5-f799d900cb97" />

Group Assignment + Access
<img width="1144" height="536" alt="image" src="https://github.com/user-attachments/assets/e739a1c2-a9c9-4ff5-bdfe-7ba910c4a834" />

MFA Setup
<img width="1328" height="558" alt="image" src="https://github.com/user-attachments/assets/1db52f5e-78bc-4543-9adc-eedba9562df9" />

 SSO Config in Okta
 <img width="1292" height="597" alt="image" src="https://github.com/user-attachments/assets/6d31e8cd-80d5-4396-be1e-53d59f76f51c" />

 Project Structure
The repository is organized as follows:

📁 iam-lifecycle-simulation-scim-entra-okta/
├── README.md                          # Project overview and documentation
├── user_data.csv                      # Sample input data for identity provisioning
├── provisioning_steps.md              # Step-by-step notes for SCIM provisioning flow
├── screenshots/
│   └── iam-summary.png                # Combined IAM screenshots (Entra ID & Okta)


