---

# Juniper vSRX

---

## Product Description

Data centers increasingly rely on server virtualization to deliver services faster and more efficiently than ever before. The virtualized data center, however, introduces new challenges that require additional security considerations beyond those needed to secure physical assets.

Virtual machines (VM) can be highly dynamic and elastic in a virtualized data center, with frequent additions, moves, and changes. These frequent changes complicate the ability to attach security policies to a VM instantiation and track security policies with VM movement to ensure continued regulatory compliance. 

In short, the dynamic and flexible nature of virtualization can easily lead to a loss of visibility and control.
Network and security professionals must perform a delicate balancing act, delivering the benefits of virtualization and cloud technologies without undermining the organization's security.

This challenge can only be met by a security solution that can keep pace with evolving threats while matching the agility and scalability of virtualized and cloud environments—without sacrificing reliability, visibility, and control.

Juniper addresses these challenges head-on by extending the capabilities of the awardwinning Juniper Networks® SRX Series Services Gateways to the virtual world with the vSRX Virtual Firewall. 

Juniper makes security easy by securing the cloud at every level: between applications, between instances, and across environments.

Powered by Juniper Networks Junos® operating system, the vSRX delivers a complete and integrated virtual security solution, including L4-L7 advanced security services, robust networking, and automated life cycle management capabilities for service providers and enterprises alike.

The vSRX’s automated provisioning capabilities allow network and security administrators to quickly and efficiently provision and scale firewall protection to meet the dynamic needs of virtualized and cloud environments. By combining the vSRX with the power of Junos Space® Security Director, administrators can significantly improve policy configuration, management, and visibility into both physical and virtual assets from a standard, centralized platform.

For service providers and organizations deploying service-oriented applications in software, the vSRX’s portfolio of virtualized network and security services supports a variety of Network Functions Virtualization (NFV) use cases. The vSRX also supports Juniper Networks Contrail, OpenContrail, and other third-party solutions, and can be integrated with other next-generation cloud orchestration tools such as OpenStack, either directly or through rich APIs.

## Before you begin

* Terraform >= 0.12.0
* Terraform Provider IBM >= 1.12.0 Needs to install the IBM Provider pluging following the link IBM Setup
* Terraform Provider Template >= 2.1.2


## Required resources

To run the software, the following resources are required:
* 3 subnets in your VPC : one for Out Of BAnd Management, one for private side, one for public side
* SSH key that is used to reach the vSRX mgmt IP through SSH
* one or more security-groups to apply to the 3 subnets 

## Production configuration

# Advanced Security Services
Implementing nonintegrated, legacy systems built around traditional firewalls and individual standalone appliances and software is no longer adequate to protect against today’s sophisticated attacks. Juniper’s advanced security suite enables users to deploy multiple technologies to meet the unique and evolving needs of modern organizations and the continually changing threat landscape. Real-time updates ensure that the technologies, policies, and other security measures are always current.

The vSRX delivers a versatile and powerful set of advanced security services, including content security, intrusion detection and prevention (IDP/IPS), and application control and visibility services through Juniper Networks AppSecure.

# Content Security
The vSRX includes comprehensive content security against malware, viruses, phishing attacks, intrusions, spam, and other threats with best-in-class antivirus, antispam, Web filtering, and content filtering features (see Table 1).

# Intrusion Prevention System (IPS)
IPS for vSRX controls access to IT networks to protect systems from attack by inspecting data and taking actions such as blocking attacks as they are developing—and before they succeed—or creating a series of rules in the firewall. IPS tightly integrates Juniper’s applications security features with the network infrastructure to further mitigate threats and protect against a wide range of attacks and vulnerabilities (see Table 2).

# Application Visibility and Control with AppSecure
AppSecure is a next-generation application security suite for vSRX and SRX Series Services Gateways that delivers threat visibility, protection, enforcement, and control. Whether needing to understand how many users are accessing cloud-based applications like Facebook every day, or needing to know what applications are using the most bandwidth, AppSecure delivers powerful visibility and ongoing application tracking. With open signatures, unique application sets can be monitored, measured, and controlled to tie closely to the organization’s business priorities.

# Juniper Advanced Threat Prevention
Juniper Advanced Threat Prevention integrates with the vSRX to provide dynamic, automated protection against known malware and advanced zero-day threats, resulting in instantaneous responses.
Security policies determine if a session can originate in one zone and be forwarded to another zone. The vSRX receives packets and keeps track of every session, every application, and every user. As a VM moves within a virtualized or cloud environment, it will still send packets to the vSRX for processing, continuously communicating in a secure mode.


# High Availability (HA)
The vSRX provides mission-critical reliability, supporting chassis clustering for active/active and active/passive modes. The HA functionality provides full stateful failover for any connections processed and for cluster members to span hypervisors. When configured in a cluster, vSRX VMs synchronize the connection/session state and flow information with IPsec security associations, Network Address Translation (NAT) traffic, address book information, configuration changes, and more. As a result, not only is the session preserved during failover, but security is also kept intact. In an unstable network, vSRX also mitigates link flapping.


# Juniper Secure Connect
Juniper Secure Connect is a highly flexible SSL VPN application that provides secure access to corporate and cloud resources for employees working away from protected resources.
Juniper Secure Connect is available for desktop and mobile devices including Windows, Mac OS, Android, and iOS. When combined with the SRX Series Services Gateways, Secure Connect helps organizations achieve dynamic, flexible, and adaptable connectivity to any device anywhere, reducing risk by extending visibility and enforcement from users to cloud.


## Upgrading to a new version

When a new version of a Helm Chart is available, you're alerted in your Schematics workspace. To upgrade to a new version, complete the following steps:

1. Go to the **Menu** > **Schematics**.
2. Select your workspace name. 
3. Click **Settings**. In the Summary section, your version number is displayed. 
4. Click **Update**.
5. Select a version, and click **Update**.

## Uninstalling the software

Complete the following steps to uninstall a Helm Chart from your account. 

1. Go to the **Menu** > **Schematics**.
2. Select your workspace name. 
3. Click **Actions** > **Destroy resources**. All resources in your workspace are deleted.
4. Click **Update**.
5. To delete your workspace, click **Actions** > **Delete workspace**.

## Getting support

### Support site URL

https://apps.juniper.net/home/vsrx/support

### Support response process
Keeping your network up and running depends on the ability to resolve issues fast or even proactively identifying conditions before they impact service. Juniper offers a wide range of support services, that can be highly customized, to help you manage your network for optimal performance and reliability while improving operational efficiency. Juniper’s flexible maintenance services offer mission-critical support for Juniper hardware and software products around the clock, 365 days a year.

### Support locations
United States, Netherlands, Israel, India, Hong Kong, China, Japan, Korea, Republic of, Australia


### Support escalations
Our systematic escalation process is intended to notify and brief various levels of management throughout the lifecycle of a Service Request. Escalation timeframes are measured on a 24x7x365 basis. If the issue is not resolved to your satisfaction or in the expected timeframe, call the Customer Care number +1-888-314-5822, or +1 408-745-9500 and ask for your Service Request to be assigned to an Escalation team member. For P1 escalations occurring on weekends or after office hours, please request to have the on-call escalations Customer Care person contacted. Customer Care managers are available 7x24x365 formanagement escalations. Upon reaching Customer Care, please provide your Service Request number and ask for the escalation manager. More information at: https://support.juniper.net/support/pdf/guides/7100156-001-EN.pdf
