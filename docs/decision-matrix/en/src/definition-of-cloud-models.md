# Definitions of (cloud) models

## Public Cloud

Public cloud refers to IT infrastructure and services provided over the internet by commercial providers such as AWS, Microsoft Azure, or Google Cloud. The resources are shared by many customers (multi-tenancy), with each customer being logically isolated and only seeing their own data and applications. Billing is usage-based according to the pay-as-you-go principle, where you only pay for the resources you actually use. The public cloud offers virtually unlimited scalability and an extensive catalog of services, from simple virtual machines to complex AI and analytics platforms. The provider is responsible for the operation, maintenance, and security of the underlying infrastructure, while the customer manages their applications and data.

## Private Cloud (Hosted externally)

Private cloud (externally hosted) is a cloud infrastructure that is operated exclusively for a single organization but is hosted by a hosting provider or as a dedicated environment by a cloud provider (e.g., AWS Outposts, Azure Dedicated Host, IBM Cloud Dedicated). It offers cloud characteristics such as self-service, automation, and elastic resources, combined with greater control over security, compliance, and data sovereignty than a public cloud. The organization uses dedicated hardware but does not have to worry about physical operation, cooling, or power supply. This option is chosen when compliance requirements necessitate a dedicated infrastructure, but the expense of a dedicated data center is to be avoided. The connection is typically established via dedicated connections or VPN.


## Private Cloud (On-Premises)

Private cloud (on-premises) is a cloud-based infrastructure that is operated in the organization's own data center and offers cloud characteristics. It is based on platforms such as VMware vCloud, OpenStack, or Red Hat OpenShift and enables self-service portals, automation, infrastructure-as-code, and elastic resources. Unlike traditional on-premises solutions, it offers modern cloud management functions but remains completely under the organization's control in its own data center. This option combines maximum control and data sovereignty with cloud convenience and is chosen when the highest security or compliance requirements need to be combined with modern cloud operating models. The organization bears full responsibility for hardware, operation, and maintenance.

## On-Premises (traditional)

On-premises (traditional) refers to classic IT infrastructure without cloud characteristics that is operated entirely in the company's own data center. The infrastructure is based on traditional approaches such as physical servers, classic virtualization (without self-service), manual provisioning processes, and individual configuration. The organization owns the hardware, is responsible for all operations, and bears all costs for procurement, maintenance, electricity, and personnel. This approach is often found in legacy systems, mainframes, specialized production systems, or when cloud abstractions are deliberately avoided. In contrast to private cloud (on-premises), modern automation and self-service functions are lacking, which leads to longer provisioning times, but also to very stable, well-understood environments.

## Important distinctions

**Hybrid cloud** is a combination of two or more of the above models (e.g., private cloud on-premises + public cloud) that work together in an integrated manner and allow workloads to be moved flexibly.

**Multi-cloud** refers to the parallel use of multiple public cloud providers to avoid vendor lock-in or to leverage best-of-breed services.

**Edge computing** refers to computing capacity at the edge of the network, close to the data sources, and can be combined with all four models.


## Summary of the main differences

| Aspect                         | Public Cloud         | Private Cloud (External)         | Private Cloud (On-Prem) | On-Prem (Traditional) |
| ------------------------------ | -------------------- | -------------------------------- | ----------------------- | --------------------- |
| **Location**                   | Provider data center | Provider data center (dedicated) | Own data center         | Own data center       |
| **Multi-tenancy**              | Multi-tenant         | Single-tenant                    | Single-tenant           | Single-tenant         |
| **Cloud features**             | Full                 | Full                             | Full                    | Minimal/None          |
| **Internet dependency**        | High                 | High                             | Low                     | Low                   |
| **Operational responsibility** | Provider             | Shared                           | Entirely customer       | Entirely customer     |
| **Scalability**                | Virtually unlimited  | Limited, fast                    | Limited, medium         | Limited, slow         |
| **Cost model**                 | OpEx (pay-per-use)   | Mixed OpEx/CapEx                 | CapEx + OpEx            | CapEx + OpEx          |
| **Control**                    | Shared               | High                             | Maximum                 | Maximum               |
| **Automation**                 | High                 | High                             | High                    | Low                   |


## Impact of application architecture

The choice between the four options is largely influenced by the architecture of your application:

**Cloud-native applications** (microservices, containers, serverless, API-first) are specifically designed for cloud environments and make optimal use of their elasticity, managed services such as Kubernetes, databases, and message queues. They benefit from automatic scaling and you only pay for actual usage. Public cloud is ideal here, while private cloud (both variants) is also well suited. Traditional on-premises would eliminate most of the advantages.

**Modern enterprise applications** with container technology, REST/GraphQL APIs, modern frameworks (Spring Boot, .NET Core, Node.js), and stateless design work well in all cloudified environments. They benefit from self-service and automation, but do not necessarily require the unlimited scaling of the public cloud. All four options are fundamentally suitable, with the choice depending on other factors such as compliance and cost.

**Traditional application server applications** with monolithic architecture, JavaEE/J2EE on application servers (WebSphere, JBoss, WebLogic), and stateful sessions are optimized for stable, predictable infrastructure. They scale primarily vertically and benefit little from cloud elasticity. Private cloud (on-premises) or traditional on-premises are often more economical here, as you do not pay for unused cloud flexibility. Public cloud is technically possible, but often more expensive.

**Legacy systems** with hardware dependencies, proprietary protocols, mainframe integration, or specialized hardware usually require traditional on-premises solutions. Migrating such systems to cloud environments is often technically very complex and only makes economic sense if refactoring is carried out at the same time.