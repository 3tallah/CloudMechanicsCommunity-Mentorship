# Development Resources & Lab Building Guide

## Purpose

This comprehensive guide provides curated Microsoft Learn resources, documentation links, and step-by-step guidance to build hands-on test labs and excel as an Azure Cloud Engineer. It is aligned with Azure certifications (AZ-900 -> AZ-104 -> AZ-305) and Azure Well-Architected Framework principles.

## Azure Cloud Engineer Learning Path Overview

Follow this structured progression to become an Azure Cloud Engineer:

1. **Foundation (Week 1-2):** [Azure Fundamentals](https://learn.microsoft.com/en-us/training/paths/azure-fundamentals/)
2. **Administrator (Month 1-3):** [AZ-104: Azure Administrator Associate](https://learn.microsoft.com/en-us/training/paths/az-104-administrator-prerequisites/)
3. **Architect (Month 4-6):** [AZ-305: Azure Solutions Architect](https://learn.microsoft.com/en-us/training/paths/microsoft-azure-architect-design-prerequisites/)

## How to Use These Resources

- **Lab Environment:** Set up your personal Azure lab subscription (free tier or paid) to practice all hands-on tasks.
- **Progressive Learning:** Follow the resources in sequence, starting with foundational topics before moving to advanced areas.
- **Hands-On Practice:** For each resource marked "Required," complete the suggested lab exercises. Use [Microsoft Learn Sandbox](https://learn.microsoft.com/) for free hands-on labs.
- **Arc Integration:** Enable [Azure Arc](https://learn.microsoft.com/en-us/azure/azure-arc/overview) to manage both cloud and on-premises resources.
- **Documentation:** Document lab configurations, learnings, and architecture decisions for portfolio development.

---

## Azure Cloud Engineer Certification Path

*Estimated Study Duration: 6 months (Month 1-6)*

| Certification | Exam | Microsoft Learn Path | Study Time | Prerequisites |
| --- | --- | --- | --- | --- |
| **Azure Fundamentals** | [AZ-900](https://learn.microsoft.com/credentials/certifications/exams/az-900/) | [Azure Fundamentals](https://learn.microsoft.com/en-us/training/paths/azure-fundamentals/) | 2-3 weeks | None |
| **Azure Administrator**  | [AZ-104](https://learn.microsoft.com/credentials/certifications/exams/az-104/) | [AZ-104 Learning Paths](https://learn.microsoft.com/en-us/training/paths/az-104-administrator-prerequisites/) | 6-8 weeks | AZ-900 (recommended) |
| **Azure Solutions Architect** | [AZ-305](https://learn.microsoft.com/credentials/certifications/exams/az-305/) | [AZ-305 Learning Paths](https://learn.microsoft.com/en-us/training/paths/microsoft-azure-architect-design-prerequisites/) | 8-10 weeks | AZ-104 (recommended) |

### Key Resources

- [Azure Certification Poster](https://aka.ms/AzureCerts_Poster) - Visual guide to all Azure certifications
- [Exam Practice Assessments](https://learn.microsoft.com/en-us/credentials/certifications/exams/az-104/practice/assessment) - Free practice tests
- [Azure Study Guides](https://learn.microsoft.com/credentials/certifications/resources/study-guides/az-104) - Official Microsoft study guides
- [Exam Readiness Zone](https://learn.microsoft.com/shows/exam-readiness-zone/) - Video prep courses

---

## 1. Azure Networking Resources

*Estimated Study Duration: 2 weeks (Month 1-2)*

**AZ-104 Learning Paths:**
- [Configure virtual networks](https://learn.microsoft.com/training/modules/configure-virtual-networks/) - VNet setup, subnets, IP addressing
- [Configure network security groups](https://learn.microsoft.com/training/modules/configure-network-security-groups/) - NSG rules and best practices
- [Configure Azure Virtual Network peering](https://learn.microsoft.com/training/modules/configure-vnet-peering/) - VNet connectivity
- [Manage and control traffic flow with routes](https://learn.microsoft.com/training/modules/control-network-traffic-flow-with-routes/) - User-defined routes
- [Introduction to Azure Load Balancer](https://learn.microsoft.com/training/modules/intro-to-azure-load-balancer/) - Traffic distribution
- [Introduction to Azure Application Gateway](https://learn.microsoft.com/training/modules/intro-to-azure-application-gateway/) - Layer 7 routing
- [Introduction to Azure Network Watcher](https://learn.microsoft.com/training/modules/intro-to-azure-network-watcher/) - Network diagnostics

**Additional Networking Topics:**

| Topic Area | Resource Links | Lab Practice |
| --- | --- | --- |
| **Virtual Networks** | [Configure virtual networks](https://learn.microsoft.com/training/modules/configure-virtual-networks/) - Address space planning, subnet design, DNS | * Required |
| **VNet Peering** | [Configure VNet peering](https://learn.microsoft.com/training/modules/configure-vnet-peering/) - Transit routing, connectivity | * Required |
| **Network Security Groups** | [Configure NSGs](https://learn.microsoft.com/training/modules/configure-network-security-groups/) - Inbound/outbound rules | * Required |
| **Application Security Groups** | [ASG Implementation](https://learn.microsoft.com/training/modules/configure-network-security-groups/) | * Required |
| **Azure Firewall** | [Deploy Azure Firewall](https://learn.microsoft.com/training/modules/configure-azure-firewall-as-network-security-solution/) - WAF and DDoS protection | * Required |
| **Load Balancer** | [Azure Load Balancer](https://learn.microsoft.com/training/modules/intro-to-azure-load-balancer/) - Internal and public LB, health probes | * Required |
| **Application Gateway** | [Application Gateway](https://learn.microsoft.com/training/modules/intro-to-azure-application-gateway/) - WAF, SSL termination | * Required |
| **DNS** | [Host domain on Azure DNS](https://learn.microsoft.com/training/modules/host-domain-azure-dns/) - DNS zones, records | * Required |
| **User-Defined Routes** | [Manage routes](https://learn.microsoft.com/training/modules/control-network-traffic-flow-with-routes/) - Custom routing tables | * Required |
| **Network Watcher** | [Azure Network Watcher Tools](https://learn.microsoft.com/training/modules/intro-to-azure-network-watcher/) - Connection Monitor, Traffic Analytics | * Required |
| **Azure Bastion** | [Connect to VMs with Bastion](https://learn.microsoft.com/training/modules/connect-vm-with-azure-bastion/) - Secure RDP/SSH | * Required |
| **Azure VPN Gateway** | [Configure VPN Gateway](https://learn.microsoft.com/training/modules/configure-vpn-gateway/) - Site-to-site, Point-to-site VPN | * Config Only |
| **Azure ExpressRoute** | [ExpressRoute Fundamentals](https://learn.microsoft.com/training/modules/intro-to-expressroute/) - Dedicated connectivity | Concept Only |
| **Azure Traffic Manager** | [Traffic Manager routing](https://learn.microsoft.com/training/modules/configure-traffic-manager-routing-methods/) - Geographic routing, failover | * Required |

**Suggested Comprehensive Lab (Month 2):**

- Deploy a multi-tier application across multiple availability zones
- Configure load balancing with Application Gateway and WAF rules
- Implement NSG rules and ASG-based traffic control
- Set up VNet peering between multiple virtual networks
- Configure user-defined routes for custom traffic flow
- Monitor network performance with Network Watcher and Connection Monitor
- Test failover scenarios with Traffic Manager or Load Balancer
- Deploy Azure Bastion for secure VM access

## 2. Compute & Storage Resources

*Estimated Study Duration: 2 weeks (Month 2-3)*

**AZ-104 Learning Paths:**
- [Deploy and manage Azure compute resources](https://learn.microsoft.com/training/paths/az-104-manage-compute-resources/) - VMs, scale sets, App Service, containers
- [Implement and manage storage in Azure](https://learn.microsoft.com/training/paths/az-104-manage-storage/) - Storage accounts, blobs, files, security
- [Configure virtual machine availability](https://learn.microsoft.com/training/modules/configure-virtual-machine-availability/) - Availability sets and zones
- [Configure App Service plans](https://learn.microsoft.com/training/modules/configure-app-service-plans/) - App hosting and scaling
- [Configure Azure Container Instances](https://learn.microsoft.com/training/modules/configure-azure-container-instances/) - Container orchestration

**Storage Resources:**

| Topic Area | Resource Links | Lab Practice |
| --- | --- | --- |
| **VM Families & Sizing** | [Choose Azure VM Sizes](https://learn.microsoft.com/training/modules/intro-to-azure-virtual-machines/) - Right-sizing for workloads | Concept Only |
| **VM Availability** | [Configure VM Availability](https://learn.microsoft.com/training/modules/configure-virtual-machine-availability/) - Availability sets, zones | * Required |
| **VM Extensions** | [Azure VM Extensions](https://learn.microsoft.com/training/modules/intro-to-azure-virtual-machines/) - Custom Script, monitoring | * Required |
| **VM Diagnostics** | [Boot Diagnostics](https://learn.microsoft.com/training/modules/intro-to-azure-virtual-machines/) - Troubleshooting VMs | * Required |
| **Storage Accounts** | [Configure storage accounts](https://learn.microsoft.com/training/modules/configure-storage-accounts/) - Redundancy, endpoints | * Required |
| **Blob Storage** | [Configure Blob Storage](https://learn.microsoft.com/training/modules/configure-blob-storage/) - Tiers, lifecycle policies | * Required |
| **Azure Files** | [Configure Azure Files](https://learn.microsoft.com/training/modules/configure-azure-files-file-sync/) - SMB shares, sync | * Required |
| **Storage Security** | [Configure storage security](https://learn.microsoft.com/training/modules/configure-storage-security/) - SAS, firewalls, encryption | * Required |
| **VMSS** | [VM Scale Sets](https://learn.microsoft.com/en-us/azure/virtual-machine-scale-sets/overview) - Auto-scaling | Concept Only |
| **App Service** | [Configure App Service](https://learn.microsoft.com/training/modules/configure-azure-app-services/) - Deployment slots, scaling | * Required |
| **Container Instances** | [Configure Container Instances](https://learn.microsoft.com/training/modules/configure-azure-container-instances/) - Serverless containers | * Required |
| **Containers & Kubernetes** | [Azure Kubernetes Service](https://learn.microsoft.com/azure/aks/concepts-clusters-workloads) - Container orchestration | Concept Only |
| **Managed Disks** | [Managed Disks Benefits](https://learn.microsoft.com/training/modules/intro-to-azure-virtual-machines/) - Performance, reliability | Concept Only |
| **Azure SQL Database** | [Azure SQL Database](https://learn.microsoft.com/azure/azure-sql/database/sql-database-paas-overview) - PaaS databases | Concept Only |
| **Cosmos DB** | [Cosmos DB](https://learn.microsoft.com/azure/cosmos-db/introduction) - Global distributed database | Concept Only |

**Suggested Comprehensive Lab (Month 3):**

- Deploy VMs across multiple availability zones with managed disks
- Configure Azure Storage accounts with redundancy options
- Upload and manage blobs with lifecycle policies
- Set up Azure Files with sync capabilities
- Deploy a web app using App Service with deployment slots
- Test Autoscale on App Service with custom metrics
- Deploy container instances for microservices
- Configure storage security with access keys and SAS tokens

## 3. Azure Migration Resources

*Estimated Study Duration: 5 days (Month 3)*

**AZ-104 Migration Coverage:**
- [Migration Overview](https://learn.microsoft.com/azure/migrate/migrate-services-overview) - Azure Migrate service capabilities
- [Rehost and Replatform migrations](https://learn.microsoft.com/azure/cloud-adoption-framework/migrate/index) - Cloud Adoption Framework migration patterns

**Migration & Disaster Recovery Resources:**

| Topic Area | Resource Links | Lab Practice |
| --- | --- | --- |
| **Azure Migrate Assessment** | [Assessment overview (migrate to Azure VMs)](https://learn.microsoft.com/en-us/azure/migrate/concepts-assessment-calculation?view=migrate)  [Azure Migrate Tutorial](https://learn.microsoft.com/azure/migrate/tutorial-assess-vmware-azure-vm) | * Required |
| **Azure Site Recovery** | [ASR Migration Guide](https://learn.microsoft.com/azure/site-recovery/migrate-tutorial-on-premises-azure) [Test Failover Process](https://learn.microsoft.com/azure/site-recovery/site-recovery-test-failover-to-azure) | * Required |
| **Database Migration** | [Azure Database Migration Service](https://learn.microsoft.com/azure/dms/dms-overview) | Concept Only |
| **Data Migration** | [Azure Data Box](https://learn.microsoft.com/azure/databox/data-box-overview) - Large data transfers | Concept Only |

## 4. Security & Monitoring Resources

*Estimated Study Duration: 5 days (Month 3-4)*

**AZ-104 Security Paths:**
- [Configure Azure RBAC](https://learn.microsoft.com/training/modules/configure-role-based-access-control/) - Identity and access management
- [Configure authentication and authorization](https://learn.microsoft.com/training/modules/configure-security-for-containers/) - Container security
- [Implement and manage Azure Monitor](https://learn.microsoft.com/training/paths/az-104-monitor-and-maintain-azure-resources/) - Monitoring and diagnostics

**Security & Monitoring Resources:**

| Topic Area | Resource Links | Lab Practice |
| --- | --- | --- |
| **Azure RBAC** | [Role-Based Access Control](https://learn.microsoft.com/azure/role-based-access-control/overview) | * Required |
| **Managed Identity** | [Managed Identities for Azure resources](https://learn.microsoft.com/azure/active-directory/managed-identities-azure-resources/overview) | * Required |
| **Disk Encryption** | [Azure Disk Encryption](https://learn.microsoft.com/azure/security/fundamentals/azure-disk-encryption-vms-vmss) | * Required |
| **Microsoft Defender for Cloud** | [Microsoft Defender for Cloud Overview](https://learn.microsoft.com/azure/defender-for-cloud/defender-for-cloud-introduction) | * Required |
| **Audit Logs** | [Azure Activity Log and Resource Logs](https://learn.microsoft.com/azure/azure-monitor/essentials/activity-log) | * Required |
| **Azure Monitor** | [Azure Monitor Overview](https://learn.microsoft.com/azure/azure-monitor/overview) | * Required |
| **Key Vault** | [Azure Key Vault Overview](https://learn.microsoft.com/azure/key-vault/general/overview) - Secrets management | * Required |
| **Network Security** | [Network Security Best Practices](https://learn.microsoft.com/azure/security/fundamentals/network-best-practices) | * Required |

**Suggested Comprehensive Lab (Month 4):**

- Create Resource Groups with RBAC assignments
- Configure managed identities on VMs and App Service
- Enable disk encryption on VMs
- Set up Microsoft Defender for Cloud for threat detection
- Create Key Vault and retrieve secrets programmatically
- Configure Azure Monitor metrics and alerts
- View activity logs and diagnose issues
- Build custom dashboards in Azure Monitor
- Create action groups for incident response

## 5. Backup & Recovery Resources

*Estimated Study Duration: 2 days (Month 4)*

**AZ-104 Backup & Disaster Recovery Coverage:**
- [Configure backup and recovery](https://learn.microsoft.com/training/modules/configure-backups-disaster-recovery/) - Azure Backup and disaster recovery patterns
- [Azure Site Recovery for disaster recovery](https://learn.microsoft.com/azure/site-recovery/site-recovery-overview) - Replication and failover

**Backup & Recovery Resources:**

| Topic Area | Resource Links | Lab Practice |
| --- | --- | --- |
| **Azure Backup Service** | [Azure Backup Overview](https://learn.microsoft.com/azure/backup/backup-overview)  [Configure and manage backups](https://learn.microsoft.com/training/modules/configure-backups-disaster-recovery/) | * Required |
| **Backup Best Practices** | [Backup security best practices](https://learn.microsoft.com/azure/backup/security-overview) | Concept Only |
| **Recovery Scenarios** | [Restore files from Azure Backup](https://learn.microsoft.com/azure/backup/restore-files-from-azure-backup) | * Required |

## 6. Azure Automation & Infrastructure as Code Resources

*Estimated Study Duration: 5 days (Month 4-5)*

**AZ-104 Automation Paths:**
- [Deploy and configure infrastructure](https://learn.microsoft.com/training/modules/configure-azure-resources-tools/) - Azure CLI, PowerShell, Azure Resource Manager
- [Infrastructure as Code with Bicep and Terraform](https://learn.microsoft.com/training/paths/fundamentals-bicep/) - Declarative infrastructure

**Automation & IaC Resources:**

| Topic Area | Resource Links | Lab Practice |
| --- | --- | --- |
| **Azure PowerShell** | [Install Azure PowerShell module](https://learn.microsoft.com/powershell/azure/install-azps-windows) | * Required |
| **Azure CLI** | [Install and use Azure CLI](https://learn.microsoft.com/cli/azure/install-azure-cli) | * Required |
| **Runbooks** | [Create Azure Automation runbooks](https://learn.microsoft.com/azure/automation/automation-runbook-types) | * Required |
| **ARM Templates** | [Deploy resources with ARM templates](https://learn.microsoft.com/training/paths/deploy-manage-resource-manager-templates/) | * Required |
| **Bicep** | [Build Azure infrastructure with Bicep](https://learn.microsoft.com/training/paths/fundamentals-bicep/) - Infrastructure as Code | * Required |
| **Azure Automation** | [Azure Automation overview](https://learn.microsoft.com/azure/automation/automation-intro) | * Required |

**Suggested Comprehensive Lab (Month 5):**

- Create and run PowerShell scripts with Azure CLI integration
- Deploy infrastructure using ARM templates with parameter files
- Build Bicep modules for reusable infrastructure definitions
- Create and schedule runbooks for automated tasks
- Set up managed identities for runbooks to execute
- Deploy multi-tier applications using Infrastructure as Code
- Test roll-back scenarios with Azure Deployment History
- Enable source control integration for IaC templates

## 7. Billing & Cost Management Resources

*Estimated Study Duration: 3 days (Month 5)*

**AZ-104 Cost Management Coverage:**
- [Subscription management and cost optimization](https://learn.microsoft.com/training/modules/describe-cost-management-azure/) - Azure cost tools and optimization strategies
- [Azure Pricing Calculator](https://azure.microsoft.com/pricing/calculator/) - Estimate costs for resources

**Billing & Cost Management Resources:**

| Topic Area | Resource Links | Lab Practice |
| --- | --- | --- |
| **Subscription Management** | [Manage subscriptions and directories](https://learn.microsoft.com/azure/cost-management-billing/manage/direct-ea-administration) | * Required |
| **Azure Hybrid Benefit** | [Hybrid Benefit benefits](https://azure.microsoft.com/hybrid-benefit/) | Concept Only |
| **Reserved Instances** | [Azure Reservations and savings plans](https://learn.microsoft.com/azure/cost-management-billing/reservations/save-compute-costs-reservations) | * Required |
| **Azure Pricing Calculator** | [Estimate prices using calculator](https://azure.microsoft.com/pricing/calculator/) | * Required |
| **Cost Analysis** | [Analyze costs with Cost Management](https://learn.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis) | * Required |
| **Cost Alerts** | [Set up cost alerts and budgets](https://learn.microsoft.com/azure/cost-management-billing/costs/cost-mgt-alerts) | * Required |

## 8. Additional Learning Platforms

- **Microsoft Learn:** [Microsoft Learn Azure](https://learn.microsoft.com/en-us/azure/) - Free, hands-on Azure learning paths

- **Azure Architecture Center:** [Best practices and reference architectures](https://learn.microsoft.com/en-us/azure/architecture/)

- **Azure CAF:** [Cloud Adoption Framework](https://learn.microsoft.com/en-us/azure/cloud-adoption-framework/)

- **Azure WAF:** [Well-Architected Framework](https://learn.microsoft.com/en-us/azure/architecture/framework/)

- **Pluralsight Azure Courses:** Available via your approved learning subscription

- **Azure Friday Videos:** [Weekly Azure updates and demos](https://azure.microsoft.com/en-us/resources/videos/azure-friday/)

## Real-World Problem Scenarios for Practice

*Use these scenarios to test your understanding and problem-solving skills:*

**Networking Challenges:**

- How to implement VLAN-like traffic control in Azure (NSG & ASG approach)?

- Fixing session-based application issues with WAF (cookie-based session affinity)

- Implementing MFA for P2S VPN access

- Geo-restricting web application access using Azure Firewall/Application Gateway

- When to configure BGP for VPN Gateway scenarios

**Compute & Storage Challenges:**

- Windows Server file share vs Azure Files for enterprise applications (e.g., FileNet)

- Hosting Exchange on Azure - email flow challenges during failover

- SCCM on Azure - limitations and cloud alternatives

- Handling D: drive conflicts with Azure temporary storage

- App Service assessment tools and LDAP-integrated app hosting

- Why load balancer is required for Always On clusters in Azure

**Migration Challenges:**

- Multi-VM migration planning based on application dependencies

- Testing Azure VMs before go-live while maintaining service dependencies

- Managing network consumption during ASR synchronization

**Security & Governance Challenges:**

- Granting access to external parties - B2B vs service principal options

- Least-privilege access for network teams using Azure RBAC

- Adaptive application control implementation without downtime

- Using Security Center for on-premises machines (Arc integration)

- Investigating Azure resource changes using Activity Logs

- Integrating third-party SIEM (Splunk) with Azure logs

