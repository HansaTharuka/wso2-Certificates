# WSO2 Certification Paths

```mermaid
flowchart TD
    START([🎓 WSO2 Certifications]) --> APIM
    START --> MI
    START --> IS
    START --> BAL
    START --> CHOREO
    START --> SA

    %% ─── API Manager Track ───
    subgraph APIM["🔷 API Manager Track"]
        direction TB
        APIM_P["Practitioner V4\n30 MCQ | 90 min"]
        APIM_DEV["Developer V4\n50 MCQ"]
        APIM_EXP["Expert V4\n2 Practical Exams"]
        APIM_SALES["Sales Professional 2024\n50 MCQ"]
        APIM_P --> APIM_DEV --> APIM_EXP
    end

    %% ─── Micro Integrator Track ───
    subgraph MI["🔶 Micro Integrator Track"]
        direction TB
        MI_P["Practitioner V4\n30 MCQ | 90 min"]
        MI_DEV["Developer V4\n50 MCQ"]
        MI_EXP["Expert V4\n2 Practical Exams"]
        MI_SALES["Integration Sales Pro 2024\n50 MCQ"]
        MI_P --> MI_DEV --> MI_EXP
    end

    %% ─── Identity Server Track ───
    subgraph IS["🟣 Identity Server Track"]
        direction TB
        IS_P["Practitioner V7\n30 MCQ | 90 min"]
        IS_DEV["Developer V7\n50 MCQ"]
        IS_EXP["Expert V7\n2 Practical Exams"]
        IS_EXP_V6["Expert V6 ⚠️ Legacy"]
        IS_EXP_V5["Expert V5 ⚠️ Legacy"]
        IS_SALES["IAM Sales Pro 2023\n50 MCQ"]
        IS_P --> IS_DEV --> IS_EXP
    end

    %% ─── Ballerina Track ───
    subgraph BAL["🟢 Ballerina Track"]
        BAL_DEV["Certified Developer\nSwan Lake"]
    end

    %% ─── Choreo Track ───
    subgraph CHOREO["🔵 Choreo Track"]
        CHOREO_SALES["Sales Professional 2025\n50 MCQ"]
    end

    %% ─── Solutions Architect ───
    subgraph SA["🏆 Solutions Architect"]
        SA_ASSOC["Solutions Architect Associate 2025\nMCQ + Scenario-based\nRequires: 2 Developer Certs"]
    end

    %% Solutions Architect prerequisites
    APIM_DEV -->|"prerequisite"| SA_ASSOC
    MI_DEV -->|"prerequisite"| SA_ASSOC
    IS_DEV -->|"prerequisite"| SA_ASSOC

    %% ─── Styling ───
    style START fill:#1a73e8,color:#fff,stroke:#1558b0
    style APIM fill:#e8f4fd,stroke:#1a73e8
    style MI fill:#fff3e0,stroke:#f57c00
    style IS fill:#f3e5f5,stroke:#7b1fa2
    style BAL fill:#e8f5e9,stroke:#388e3c
    style CHOREO fill:#e3f2fd,stroke:#1565c0
    style SA fill:#fff9c4,stroke:#f9a825

    style APIM_P fill:#bbdefb,stroke:#1a73e8
    style APIM_DEV fill:#90caf9,stroke:#1565c0
    style APIM_EXP fill:#1e88e5,color:#fff,stroke:#0d47a1
    style APIM_SALES fill:#e1f5fe,stroke:#0288d1

    style MI_P fill:#ffe0b2,stroke:#f57c00
    style MI_DEV fill:#ffcc80,stroke:#e65100
    style MI_EXP fill:#fb8c00,color:#fff,stroke:#e65100
    style MI_SALES fill:#fff8e1,stroke:#f9a825

    style IS_P fill:#e1bee7,stroke:#7b1fa2
    style IS_DEV fill:#ce93d8,stroke:#6a1b9a
    style IS_EXP fill:#8e24aa,color:#fff,stroke:#4a148c
    style IS_EXP_V6 fill:#f8bbd0,stroke:#c2185b
    style IS_EXP_V5 fill:#f8bbd0,stroke:#c2185b
    style IS_SALES fill:#fce4ec,stroke:#c2185b

    style BAL_DEV fill:#a5d6a7,stroke:#388e3c
    style CHOREO_SALES fill:#90caf9,stroke:#1565c0
    style SA_ASSOC fill:#fff176,stroke:#f9a825
```

---

## Legend

| Level | Description | Format |
|-------|-------------|--------|
| **Practitioner** | Entry level | 30 MCQ, 90 min, no prerequisites |
| **Developer** | Intermediate | 50 MCQ, ~3 months hands-on experience |
| **Expert** | Advanced | 2 Practical exams, requires Developer cert |
| **Sales Professional** | Sales/pre-sales | 50 MCQ |
| **Solutions Architect Associate** | Architect level | MCQ + Scenario-based, requires 2 Developer certs |

---

## Certification Tracks Summary

| Track | Levels Available |
|-------|-----------------|
| 🔷 API Manager | Practitioner → Developer → Expert + Sales Pro |
| 🔶 Micro Integrator | Practitioner → Developer → Expert + Sales Pro |
| 🟣 Identity Server | Practitioner → Developer → Expert (V5/V6 Legacy) + Sales Pro |
| 🟢 Ballerina | Developer (Swan Lake) |
| 🔵 Choreo | Sales Professional |
| 🏆 Solutions Architect | Associate (requires 2 Developer certs) |

> **Note:** Legacy certifications (IS Expert V5 & V6) are still valid but no longer offered for new candidates. It is recommended to pursue the latest V7 track.
>
> 🔗 Register at: [wso2.com/training/certification](https://wso2.com/training/certification)

---

## 📚 Exam Study Guide — Topics & References

> **Exam policy:** Exams are **partially open-book**. You may use official WSO2 documentation and the LMS during the exam. AI tools, Google, and external resources are **strictly prohibited**. Passing score is **70%**.

---

### 🔷 API Manager Track (V4 — based on APIM 4.5)

#### Practitioner V4

| Topic Area | Key Concepts | Reference |
|---|---|---|
| **Standards & Protocols** | REST, HTTP/HTTPS, JSON, XML, Swagger/OpenAPI 3.0, SOAP | [APIM Docs](https://apim.docs.wso2.com/en/latest/) |
| **Core Features** | API creation, Publisher Portal, Developer Portal, API lifecycle | [Create & Publish API](https://apim.docs.wso2.com/en/latest/design/create-api/create-rest-api/create-a-rest-api/) |
| **Security Basics** | OAuth2, API keys, subscriptions, application creation | [API Security](https://apim.docs.wso2.com/en/latest/design/api-security/api-authentication/secure-apis-using-oauth2-tokens/) |
| **Throttling** | Subscription tiers, rate limiting, burst control | [Throttling Policies](https://apim.docs.wso2.com/en/latest/design/rate-limiting/introducing-throttling-use-cases/) |
| **Deployment** | Gateway, Control Plane, Traffic Manager components | [Architecture Overview](https://apim.docs.wso2.com/en/latest/get-started/apim-architecture/) |

📖 **Recommended LMS Course:** [APIM Developer Fundamentals V4.6](https://lms.wso2.com/courses/wso2-api-manager-developer-fundamentals-v4-1-api-management-profile)

---

#### Developer V4

| Topic Area | Key Concepts | Reference |
|---|---|---|
| **Standards & Technologies** | OAuth2 grant types, JWT, OpenID Connect, WS-Security, Mutual TLS | [OAuth2 Docs](https://apim.docs.wso2.com/en/latest/design/api-security/oauth2/oauth2-overview/) |
| **API Policies** | Request/response/fault flows, mediation policies, policy attachment | [API Policies](https://apim.docs.wso2.com/en/latest/design/api-policies/overview/) |
| **Advanced Throttling** | Custom policies, per-user quotas, multi-TM sync, IP/header conditions | [Advanced Throttling](https://apim.docs.wso2.com/en/latest/design/rate-limiting/setting-throttling-limits/) |
| **Extensions & Customization** | Custom handlers, interceptors, API monetization | [Extending APIM](https://apim.docs.wso2.com/en/latest/install-and-setup/setup/distributed-deployment/overview/) |
| **Deployment & Config** | Distributed deployment, HA setup, database configuration, Kubernetes | [Deployment Guide](https://apim.docs.wso2.com/en/latest/install-and-setup/install/installation-prerequisites/) |
| **Analytics** | Choreo Connect analytics, API usage reporting | [Analytics](https://apim.docs.wso2.com/en/latest/observe/api-manager-analytics/overview-of-api-analytics/) |

📖 **Recommended LMS Courses:**
- [APIM Developer Fundamentals V4.6](https://lms.wso2.com/courses/wso2-api-manager-developer-fundamentals-v4-1-api-management-profile)
- [APIM Developer Advanced V4.6](https://lms.wso2.com/courses/wso2-api-manager-developer-advanced-v4-1-api-management-profile)

🧪 **Sample Questions:** [APIM Developer V4 Sample Questions](https://wso2.com/training/certification/api-manager-developer-v4-sample-questions/)

---

#### Expert V4 *(requires Developer V4 + 6 months experience)*

| Topic Area | Key Concepts | Reference |
|---|---|---|
| **Architecture & Design** | Solution architecture, deployment patterns, HA/DR strategies | [Deployment Patterns](https://apim.docs.wso2.com/en/latest/install-and-setup/setup/distributed-deployment/overview/) |
| **Custom Development** | Custom mediators, sequence templates, custom throttling executors | [Custom Extensions](https://apim.docs.wso2.com/en/latest/reference/customize-product/extending-api-manager/) |
| **Configuration Review** | Artifact review, TOML config, performance tuning | [Config Reference](https://apim.docs.wso2.com/en/latest/reference/config-catalog/) |
| **Security Advanced** | Token introspection, scope validation, FAPI, certificate pinning | [Security Hardening](https://apim.docs.wso2.com/en/latest/install-and-setup/setup/security/overview/) |
| **Troubleshooting** | Wire logs, debug logs, performance monitoring, Gateway errors | [Troubleshooting](https://apim.docs.wso2.com/en/latest/troubleshooting/troubleshooting-gateway/) |

---

### 🔶 Micro Integrator Track (V4 — based on MI 4.4)

#### Practitioner V4

| Topic Area | Key Concepts | Reference |
|---|---|---|
| **Core Concepts** | Proxy services, REST APIs, inbound endpoints, sequences, tasks | [MI Docs](https://mi.docs.wso2.com/en/latest/) |
| **Basic Mediators** | Log, Property, Filter, Switch, Call, Send, Respond mediators | [Mediators Reference](https://mi.docs.wso2.com/en/latest/reference/mediators/about-mediators/) |
| **EIP Patterns** | Message Router, Splitter/Aggregator, Content Enricher, Store & Forward | [EIP Guide](https://mi.docs.wso2.com/en/latest/learn/enterprise-integration-patterns/eip-overview/) |
| **Message Formats** | JSON, XML, SOAP, CSV transformations with PayloadFactory & XSLT | [Data Transformation](https://mi.docs.wso2.com/en/latest/learn/examples/data-integration-examples/json-xml-examples/) |
| **Connectors** | SaaS connectors, protocol connectors (JMS, File, HTTP) | [Connector Store](https://mi.docs.wso2.com/en/latest/reference/connectors/connector-overview/) |

📖 **Recommended LMS Course:** [MI Developer Fundamentals V4](https://lms.wso2.com/collections)

---

#### Developer V4

| Topic Area | Key Concepts | Reference |
|---|---|---|
| **Advanced Mediators** | Enrich, Iterate, Aggregate, Throttle, Cache, DBLookup, DBReport | [Mediator Catalog](https://mi.docs.wso2.com/en/latest/reference/mediators/about-mediators/) |
| **EIP Advanced** | Pipes & Filters, Message Broker, Scatter-Gather, Dead Letter Channel | [EIP Patterns](https://mi.docs.wso2.com/en/latest/learn/enterprise-integration-patterns/eip-overview/) |
| **Transports & Security** | JMS, HTTPS, WS-Security, OAuth2, message builders & formatters | [Transport Configurations](https://mi.docs.wso2.com/en/latest/install-and-setup/setup/transport-configurations/) |
| **Data Integration** | Data Services Server (DSS), SQL/NoSQL connectors, data transformations | [Data Integration](https://mi.docs.wso2.com/en/latest/learn/examples/data-integration-examples/) |
| **Deployment & Config** | TOML configuration, C-Apps, artifact deployment, environment variables | [MI Deployment](https://mi.docs.wso2.com/en/latest/install-and-setup/install/) |
| **Debugging** | Wire logs, mediation debugger, message tracing | [Debugging Integrations](https://mi.docs.wso2.com/en/latest/develop/debugging-mediation/) |

📖 **Recommended LMS Courses:**
- MI Developer Fundamentals V4
- MI Developer Advanced V4

---

#### Expert V4 *(requires Developer V4 + 6 months experience)*

| Topic Area | Key Concepts | Reference |
|---|---|---|
| **Custom Mediators** | Class mediators (OSGI vs non-OSGI), AbstractMediator/AbstractConnector | [Custom Mediators](https://mi.docs.wso2.com/en/latest/develop/customizations/creating-custom-mediators/) |
| **Custom Connectors** | Building connectors, connector SDK, packaging | [Custom Connectors](https://mi.docs.wso2.com/en/latest/develop/customizations/creating-new-connector/) |
| **HA & Clustering** | Cluster setup, coordinated node deployment, DB sharing | [Cluster Deployment](https://mi.docs.wso2.com/en/latest/install-and-setup/setup/deployment/deploying-wso2-mi/) |
| **Performance Tuning** | Thread pools, JVM tuning, transport-level optimization | [Performance Tuning](https://mi.docs.wso2.com/en/latest/install-and-setup/setup/performance-tuning/) |

---

### 🟣 Identity Server Track (V7 — based on IS 7.1)

#### Practitioner V7

| Topic Area | Key Concepts | Reference |
|---|---|---|
| **IAM Fundamentals** | Authentication vs Authorization, Identity Providers, Service Providers | [IS Docs](https://is.docs.wso2.com/en/latest/) |
| **Standards** | OAuth2, OpenID Connect, SAML 2.0, SCIM 2.0, WS-Trust | [IAM Standards](https://is.docs.wso2.com/en/latest/references/concepts/) |
| **Core Features** | SSO, MFA, Adaptive Authentication, Self-Service portal | [Getting Started](https://is.docs.wso2.com/en/latest/get-started/overview/) |
| **User Management** | User stores (LDAP/AD/JDBC), claim management, roles & permissions | [User Management](https://is.docs.wso2.com/en/latest/guides/users/) |
| **Application Registration** | Register web/mobile/API apps, OIDC & SAML app config | [App Registration](https://is.docs.wso2.com/en/latest/guides/applications/) |

📖 **Recommended LMS Course:** [IS Fundamentals V7.1](https://lms.wso2.com/courses/wso2-identity-server-fundamentals-v5-11)

🧪 **Sample Questions:** [IS Practitioner V7 Sample Questions](https://wso2.com/training/certified-Identity-server-practitioner-v7-sample-questions/)

---

#### Developer V7

| Topic Area | Key Concepts | Reference |
|---|---|---|
| **Authentication Protocols** | OIDC flows (auth code, implicit, PKCE), SAML2 SSO, WS-Federation | [OIDC Guide](https://is.docs.wso2.com/en/latest/guides/authentication/oidc/) |
| **MFA & Adaptive Auth** | TOTP, FIDO2, Email OTP, risk-based authentication, Adaptive Auth scripts | [MFA Docs](https://is.docs.wso2.com/en/latest/guides/authentication/mfa/) |
| **Federation** | Social login (Google, GitHub), corporate IdP federation, JIT provisioning | [Identity Federation](https://is.docs.wso2.com/en/latest/guides/authentication/federated-login/) |
| **Provisioning** | SCIM2 inbound/outbound, JIT provisioning, user provisioning connectors | [SCIM2 Docs](https://is.docs.wso2.com/en/latest/guides/users/user-stores/) |
| **API Security** | OAuth2 scopes, token validation, token introspection, API authorization | [API Authorization](https://is.docs.wso2.com/en/latest/guides/authorization/) |
| **Deployment** | Deployment topologies, RDBMS setup, keystore management | [IS Deployment](https://is.docs.wso2.com/en/latest/deploy/) |

📖 **Recommended LMS Courses:**
- [IS Fundamentals V7.1](https://lms.wso2.com/courses/wso2-identity-server-fundamentals-v5-11)
- IS Advanced V7.1

🧪 **Sample Questions:** [IS Developer V7 Sample Questions](https://wso2.com/training/certification/certified-identity-server-developer-v7-sample-questions/)

---

#### Expert V7 *(requires Developer V7 + 6 months experience)*

| Topic Area | Key Concepts | Reference |
|---|---|---|
| **User Store Management** | Custom user store managers, LDAP/AD advanced configs, hybrid stores | [User Store Config](https://is.docs.wso2.com/en/latest/deploy/configure-user-stores/) |
| **Custom Extensions** | Custom authenticators, custom provisioning connectors, event handlers | [Writing Custom Authenticator](https://is.docs.wso2.com/en/latest/references/extend/authentication/) |
| **Token & Session** | Token persistence, session management, token revocation, PKCE | [Token Management](https://is.docs.wso2.com/en/latest/guides/authentication/oidc/token-binding/) |
| **Security Hardening** | FAPI compliance, TLS config, keystore, certificate pinning, CORS | [Security Configs](https://is.docs.wso2.com/en/latest/deploy/security/) |
| **Tenancy** | Multi-tenancy setup, tenant isolation, tenant-specific configurations | [Multi-tenancy](https://is.docs.wso2.com/en/latest/deploy/set-up-separate-databases-for-clustering/) |
| **Monitoring & Troubleshooting** | Log analysis, diagnostic logs, performance analysis | [IS Monitoring](https://is.docs.wso2.com/en/latest/deploy/monitor/) |

---

### 🟢 Ballerina Developer (Swan Lake)

| Topic Area | Key Concepts | Reference |
|---|---|---|
| **Language Basics** | Types, functions, modules, error handling, concurrency (strands) | [Ballerina by Example](https://ballerina.io/learn/by-example/) |
| **Network Abstractions** | Services, clients, HTTP/REST, GraphQL, gRPC, WebSockets | [Ballerina HTTP Module](https://lib.ballerina.io/ballerina/http/latest) |
| **Data Handling** | JSON/XML/CSV, data binding, query expressions, table type | [Data Docs](https://ballerina.io/learn/by-example/xml-to-json-conversion/) |
| **Integration Patterns** | Service chaining, data transformation, async messaging | [Integration Patterns](https://ballerina.io/learn/integration/) |
| **Observability & Security** | Logging, tracing, metrics, OAuth2/JWT in services | [Observability](https://ballerina.io/learn/observe-ballerina-programs/) |
| **Deployment** | Docker, Kubernetes deployment from Ballerina code | [Deployment Guide](https://ballerina.io/learn/deploy-ballerina-on-kubernetes/) |

📖 **Official Resources:**
- [Ballerina Learn](https://ballerina.io/learn/)
- [Ballerina Central (packages)](https://central.ballerina.io/)
- [Swan Lake Documentation](https://ballerina.io/downloads/swan-lake-release-notes/)

---

### 🏆 Solutions Architect Associate (2025)

*Requires: 2 Developer-level certifications in different products (latest versions)*

| Topic Area | Key Concepts | Reference |
|---|---|---|
| **Architecture Patterns** | Microservices, event-driven, API-led connectivity, SOA | [WSO2 Architecture Guide](https://wso2.com/whitepapers/) |
| **Integration Design** | Choosing APIM vs MI vs IS for given business problems | [Product Overview](https://wso2.com/products/) |
| **Security Architecture** | Zero trust, API gateway security, IAM integration patterns | [WSO2 Security Docs](https://apim.docs.wso2.com/en/latest/install-and-setup/setup/security/overview/) |
| **Deployment Topologies** | On-prem, hybrid cloud, multi-region, SaaS (Choreo) | [Choreo Docs](https://wso2.com/choreo/docs/) |
| **Solution Design** | Pre-sales solution proposals, POC design, deployment sizing | [WSO2 Reference Architectures](https://wso2.com/library/reference-architecture/) |

---

## 🛠️ General Preparation Tips

1. **Complete LMS courses first** — All courses on [lms.wso2.com](https://lms.wso2.com) are **free**. Enrolled courses stay active for 90 days.
2. **Practice with the Quick Start Guide** — Set up a local instance before the exam: [APIM Quick Start](https://apim.docs.wso2.com/en/latest/get-started/quick-start-guide/) | [IS Quick Start](https://is.docs.wso2.com/en/latest/get-started/try-your-own-app/)
3. **Review sample questions** — WSO2 provides official sample questions for each certification on the certification page.
4. **Bookmark docs** — The exam is open-book (WSO2 docs only). Bookmark key pages in advance so you can look things up quickly.
5. **Attend Live Training** — Free certifications are sometimes awarded to live training attendees: [lms.wso2.com/pages/live-training](https://lms.wso2.com/pages/live-training)
6. **2 attempts per registration** — If you fail, you have a second attempt within 30 days.

---

## 🔗 Key Reference Links

| Resource | URL |
|---|---|
| WSO2 Certification Portal | https://wso2.com/training/certification |
| WSO2 LMS (Free Courses) | https://lms.wso2.com |
| API Manager Documentation | https://apim.docs.wso2.com/en/latest/ |
| Micro Integrator Documentation | https://mi.docs.wso2.com/en/latest/ |
| Identity Server Documentation | https://is.docs.wso2.com/en/latest/ |
| Ballerina Documentation | https://ballerina.io/learn/ |
| Choreo Documentation | https://wso2.com/choreo/docs/ |
| Exam Guidelines | https://wso2.com/training/certification/exam-guidelines/ |
| Certification FAQs | https://wso2.com/training/faqs |
| Live Training | https://lms.wso2.com/pages/live-training |
| WSO2 Discord Community | https://discord.gg/wso2 |
| WSO2 LinkedIn Community | https://www.linkedin.com/groups/WSO2-Certified-Developers |
