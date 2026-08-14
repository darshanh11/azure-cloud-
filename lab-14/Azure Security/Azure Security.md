## Azure Security

### Microsoft Defender for Cloud

#### Explanation

Microsoft Defender for Cloud is an Azure security service that helps protect cloud resources by providing security recommendations, threat detection, security posture management, and workload protection.

It helps identify security weaknesses in Azure resources and provides recommendations to improve the security of the cloud environment.

### Steps

1. Open the **Azure Portal**.
2. Search for **Microsoft Defender for Cloud**.
3. Open the Defender for Cloud dashboard.
4. Review the **Security posture**.
5. Check the available security recommendations.
6. Review security alerts and detected threats.
7. Enable the required Defender plans.
8. Follow the recommended security improvements.

---

### Key Vault

#### Explanation

Azure Key Vault is a cloud service used to securely store and manage secrets, keys, and certificates.

It helps applications and administrators protect sensitive information such as passwords, API keys, connection strings, encryption keys, and certificates without storing them directly in application code.

### Steps

1. Open the **Azure Portal**.
2. Search for **Key Vaults**.
3. Select **Create**.
4. Select the required subscription and Resource Group.
5. Enter the Key Vault name.
6. Select the required Azure region.
7. Configure the security and access settings.
8. Select **Review + create**.
9. Select **Create**.
10. Add the required secrets, keys, or certificates.

---

### Network Security

#### Explanation

Network security protects Azure resources and controls network traffic between resources and external networks.

Azure provides services such as Network Security Groups (NSGs), Azure Firewall, private endpoints, and network security rules to control and protect network communication.

### Steps

1. Open the **Azure Portal**.
2. Open the required Virtual Network.
3. Select the required subnet or network interface.
4. Configure a **Network Security Group**.
5. Add inbound and outbound security rules.
6. Specify the source, destination, port, and protocol.
7. Set the required access action.
8. Save the configuration.
9. Verify the network security rules.

---

### Identity Security

#### Explanation

Identity security protects user accounts, applications, and access to Azure resources.

Microsoft Entra ID provides identity and access management features such as authentication, authorization, role-based access control, and multifactor authentication.

### Steps

1. Open the **Microsoft Entra ID** service in the Azure Portal.
2. Review the users and groups.
3. Configure appropriate access permissions.
4. Assign Azure roles using **Role-Based Access Control (RBAC)**.
5. Enable multifactor authentication where required.
6. Apply the principle of least privilege.
7. Review sign-in and audit information.
8. Remove unnecessary access.

---

### Security Best Practices

#### Explanation

Azure security best practices help protect cloud resources from unauthorized access, data loss, misconfiguration, and security threats.

A secure Azure environment should use strong identity controls, least-privilege access, network security, encryption, monitoring, regular updates, and secure management of secrets.

### Best Practices

- Use **Microsoft Entra ID** for identity management.
- Apply the **principle of least privilege**.
- Enable **multifactor authentication**.
- Use **Network Security Groups** to control network traffic.
- Store secrets and keys in **Azure Key Vault**.
- Enable appropriate **Defender for Cloud** protections.
- Encrypt sensitive data.
- Monitor security logs and alerts.
- Keep operating systems and applications updated.
- Remove unused users, permissions, and resources.
- Regularly review security recommendations.
