# Decision matrix

## Introduction

The matrix shows the suitability of the four deployment options for each criterion using a traffic light system:

- 🟢🟢🟢 = Strong/Optimally suitable
- 🟡🟡⚪ = Moderate/Suitable with restrictions
- 🔴⚪⚪ = Weak/Problematic
- ⚪⚪⚪ = To be assessed individually (see instructions below)

Use the matrix to qualitatively assess which option best suits your requirements.

## Decision matrix

| Criterion                                                                                        | Public Cloud | Private Cloud (External) | Private Cloud (On-Prem) | On-Prem (Traditional) |
| ------------------------------------------------------------------------------------------------ | ------------ | ------------------------ | ----------------------- | --------------------- |
| **Internal skills requirements** [(i)](explanations-of-criteria.md#internal-skills-requirements) | 🟢🟢🟢          | 🟡🟡⚪                      | 🔴⚪⚪                     | 🔴⚪⚪                   |
| **Compliance & data protection** [(i)](explanations-of-criteria.md#compliance--data-protection)  | 🟡🟡⚪          | 🟢🟢🟢                      | 🟢🟢🟢                     | 🟢🟢🟢                   |
| **Disaster Recovery** [(i)](explanations-of-criteria.md#disaster-recovery)                       | 🟢🟢🟢          | 🟢🟢🟢                      | 🟡🟡⚪                     | 🔴⚪⚪                   |
| **Flexibility** [(i)](explanations-of-criteria.md#flexibility)                                   | 🟢🟢🟢          | 🟢🟢🟢                      | 🟡🟡⚪                     | 🔴⚪⚪                   |
| **Innovation & Services** [(i)](explanations-of-criteria.md#innovation--services)                | 🟢🟢🟢          | 🟢🟢🟢                      | 🟡🟡⚪                     | 🔴⚪⚪                   |
| **Network Dependency** [(i)](explanations-of-criteria.md#network-dependency)                     | 🔴⚪⚪          | 🟡🟡⚪                      | 🟢🟢🟢                     | 🟢🟢🟢                   |
| **Performance & Latency** [(i)](explanations-of-criteria.md#performance--latency)                | 🟡🟡⚪          | 🟢🟢🟢                      | 🟢🟢🟢                     | 🟢🟢🟢                   |
| **Security & Control** [(i)](explanations-of-criteria.md#security--control)                      | 🟡🟡⚪          | 🟢🟢🟢                      | 🟢🟢🟢                     | 🟢🟢🟢                   |
| **Scalability** [(i)](explanations-of-criteria.md#scalability)                                   | 🟢🟢🟢          | 🟢🟢🟢                      | 🟡🟡⚪                     | 🔴⚪⚪                   |
| **Time-to-Market** [(i)](explanations-of-criteria.md#time-to-market)                             | 🟢🟢🟢          | 🟢🟢🟢                      | 🟢🟢🟢                     | 🔴⚪⚪                   |
| **Vendor lock-in risk** * [(i)](explanations-of-criteria.md#vendor-lock-in-risk)                 | 🔴⚪⚪          | 🟡🟡⚪                      | 🟢🟢🟢                     | 🟢🟢🟢                   |
| **Availability & SLA** [(i)](explanations-of-criteria.md#availability--sla)                      | 🟢🟢🟢          | 🟢🟢🟢                      | 🟡🟡⚪                     | 🟡🟡⚪                   |
|                                                                                                  |              |                          |                         |                       |
| **Architectural suitability** ** [(i)](explanations-of-criteria.md#architectural-suitability)    | ⚪⚪⚪          | ⚪⚪⚪                      | ⚪⚪⚪                     | ⚪⚪⚪                   |
| **Costs (TCO 3-5 years)** *** [(i)](explanations-of-criteria.md#costs-tco-3-5-years)             | ⚪⚪⚪          | ⚪⚪⚪                      | ⚪⚪⚪                     | ⚪⚪⚪                   |

## Variable criteria

These criteria cannot be assessed across the board and depend heavily on your specific situation:

### * Criterion: Vendor lock-in risk

**Adjustment for special approaches:**

The specified rating (public cloud: 🔴⚪⚪, private external: 🟡🟡⚪, private on-premises: 🟢🟢🟢, on-premises traditional: 🟢🟢🟢) applies to the exclusive use of one Public Cloud provider.

**Adjust to:**
- Public cloud: **🟡🟡⚪** or **🟢🟢🟢** if you use a multi-cloud strategy and container-based, portable architectures
- Private On-Prem: **🟢🟢🟢** if OpenStack or Kubernetes instead of proprietary platforms
- Private On-Prem: **🟡🟡⚪** or **🔴⚪⚪** if highly proprietary (e.g., VMware without exit strategy)

### ** Criterion: Architectural suitability

**Assess for yourself based on your application architecture:**

**Cloud-native (microservices, containers, serverless):**
- Public cloud: **🟢🟢🟢** | Private external: **🟢🟢🟢 ** | Private On-Prem: **🟢🟢🟢** | On-Prem Trad: **🔴⚪⚪**

**Modern Enterprise (Containers, REST APIs, Spring Boot, .NET Core):**
- Public Cloud: **🟢🟢🟢** | Private External: ** 🟢🟢🟢** | Private On-Prem: **🟢🟢🟢** | On-Prem Trad: **🟡🟡⚪**

**Traditional Application Servers (JavaEE, WebSphere, JBoss, Monolith):**
- Public Cloud: **🟡🟡 ⚪** | Private External: **🟡🟡⚪** | Private On-Prem: **🟢🟢🟢** | On-Prem Trad: **🟢🟢🟢**

**Legacy & Special Systems (Mainframe, Hardware-Dependent):**
- Public Cloud: **🔴⚪⚪** | Private External: **🔴⚪⚪** | Private On-Prem: **🟡🟡⚪** | On-Prem Trad: **🟢🟢🟢**

### *** Criterion: Costs (TCO 3-5 years)

**Evaluate yourself based on:**

- **Workload characteristics**: Constant (more likely on-premises) vs. Highly variable (more likely public cloud)
- **Scale**: Small (public cloud) vs. very large with constant load (on-premises more cost-effective)
- **Existing infrastructure**: Already in place and depreciated? (on-premises better) vs. new construction? (cloud better)

**Typical ratings:**
- Public cloud: **🔴⚪⚪** expensive with constant load | **🟢🟢🟢** with highly fluctuating load
- Private cloud (external): **🟡🟡⚪** medium price level
- Private cloud (on-premises): **🟡🟡⚪** high initial costs, predictable OpEx
- On-premises (traditional): **🟡🟡⚪** inexpensive with constant load and long-term use