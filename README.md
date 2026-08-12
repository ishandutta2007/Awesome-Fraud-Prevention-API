# Awesome-Fraud-Prevention-API

## Top Fraud Prevention APIs & Platforms

A curated list of leading fraud prevention, risk scoring, and abuse detection platforms for e-commerce, payments, account protection, chargeback management, and real-time transaction monitoring.  
**Primary focus: open-source software.**

Commercial / hosted platforms are listed separately for completeness. Open-source alternatives and community tools are emphasized throughout.

---

## SaaS / Hosted Platforms

| Platform | Description | Key Focus |
|----------|-------------|-----------|
| **[Sift](https://sift.com/)** | Machine-learning fraud platform with real-time risk scores, global data network, account defense, content integrity, and workflow automation. Strong for payments, ATO, and custom risk models. | Real-time risk scoring + global signals |
| **[Signifyd](https://www.signifyd.com/)** | E-commerce fraud protection with chargeback guarantee, network intelligence, anomaly detection, and pre-auth screening. Shifts liability and aims to increase approval rates. | Guaranteed fraud protection + conversion |
| **[Forter](https://www.forter.com/)** | Decisioning platform for fraud, abuse, account protection, and policy enforcement. Real-time approve/decline with identity and behavioral insights across the customer journey. | Identity-centric fraud + abuse prevention |
| **[Riskified](https://www.riskified.com/)** | E-commerce fraud prevention with chargeback guarantee, adaptive checkout, merchant network intelligence, and real-time decisioning optimized for approvals. | Chargeback guarantee + approval optimization |
| **[SEON](https://seon.io/)** | Real-time fraud prevention and AML platform with rich data enrichment (email, phone, IP, digital footprint), customizable scoring engine, and rule + AI hybrid decisioning. | Data enrichment + flexible scoring |
| **[Fraud.net](https://www.fraud.net/)** | Enterprise fraud detection and prevention with AI/ML, behavioral analytics, orchestration, and case management focused on payments and financial crime. | Enterprise payment fraud + analytics |
| **[Kount](https://kount.com/)** (Equifax) | Fraud prevention with device intelligence, customizable rules, omnichannel support, and strong reporting. Widely used for e-commerce and digital goods. | Device + rules-based fraud prevention |
| **[Feedzai](https://feedzai.com/)** | End-to-end financial crime platform covering fraud detection, AML, behavioral analytics, and real-time monitoring for banks, acquirers, and large institutions. | Banking-grade fraud + AML |
| **[DataDome](https://datadome.co/)** | Bot and online fraud protection focused on stopping automated attacks, scrapers, account takeover, and adversarial traffic in real time. | Bot management + adversarial traffic |
| **[Castle](https://castle.io/)** | Account security and fraud prevention platform emphasizing device intelligence, risk scoring for login/registration, and privacy-conscious signals. | Account protection + device intelligence |

---

## Open-Source Softwares

Fully production-grade, network-effect-driven open-source fraud prevention platforms (with the global consortium data and chargeback guarantees of commercial vendors) are rare. Strong open-source building blocks exist for transaction monitoring, ML-based detection, device fingerprinting, rules engines, and self-hosted APIs.

### Core Frameworks & Fraud / Risk Platforms

| Project | Description | License | Notes |
|---------|-------------|---------|-------|
| **[Jube](https://github.com/jube-home/aml-fraud-transaction-monitoring)** | Open-source AML and fraud detection platform for real-time transaction monitoring, adaptive machine learning, rule-based detection, and case management. | AGPLv3 | One of the more complete open AML/fraud stacks |
| **[CreditGuard](https://github.com/omsingh-19/CreditGuard)** | Production-oriented credit risk and fraud detection API built with FastAPI, XGBoost, MLflow, JWT auth, and PostgreSQL. | Open source | Strong MLOps-style fraud/credit scoring API |
| **[FraudProx](https://github.com/makozi/FraudProx)** | Real-time fraud detection API using hybrid LSTM-CNN models, exposed via FastAPI and containerized for deployment. Aimed at mobile financial services. | MIT | Deep-learning fraud detection service |
| **Open-source fraud detection APIs** (various) | Multiple FastAPI + LightGBM/XGBoost/RandomForest projects providing real-time scoring, SHAP explainability, drift monitoring (Evidently), and Prometheus/Grafana observability. | Mostly MIT/Apache | Practical self-hosted scoring endpoints |
| **MLOps fraud pipelines** | Community projects combining Kafka streaming, model serving, feedback loops, continuous training, and monitoring for production fraud systems. | Various | End-to-end detection pipelines |

### Specialized Libraries & Related Tools

| Project | Description | Focus Area |
|---------|-------------|---------|
| **OpenClientID** | Open-source, self-hostable browser and device fingerprinting for anti-fraud and customer tracking (includes server-side signals). | Device / browser fingerprinting |
| **FP-Devicer / related fingerprint cores** | Open-source fingerprinting engines with confidence scoring, storage adapters, and extensible comparison logic. | Device intelligence |
| **RiskEngine (Android)** | Mobile SDK for local device fingerprinting and runtime risk detection (root, hook, emulator, debugging signals). | Mobile device risk |
| **Rules engines** | Open-source business rules engines (Drools, Easy Rules, custom Python/JS engines) commonly used to implement fraud policies. | Policy & decisioning |
| **Anomaly detection libraries** | scikit-learn, PyOD, isolation forests, autoencoders, and streaming anomaly tools for unsupervised fraud signals. | Anomaly & outlier detection |
| **Graph / network analysis** | NetworkX, Neo4j community tools, and graph ML libraries for detecting fraud rings and linked entities. | Entity linking & rings |
| **Explainability tools** | SHAP, LIME, and related libraries for interpreting model decisions in fraud scoring. | Model transparency |

### Additional Notable Open-Source Tools

- **Feature stores & streaming** — Feast, Kafka, Flink, or simple feature pipelines for real-time risk features (velocity, device history, behavioral signals).
- **Case management** — Open-source ticket/workflow tools (or custom Django/React dashboards) for analyst review queues.
- **Bot & automation detection** — Open libraries and heuristics for headless browser, scraper, and automation detection (complementary to DataDome-style protection).
- **IP / email / phone enrichment** — Public datasets, self-hosted reputation lists, and open APIs that can approximate commercial enrichment signals.
- **Chargeback & dispute tooling** — Limited open components; most chargeback guarantee and recovery logic remains commercial.
- **Academic & research models** — Public datasets (e.g., credit-card fraud, synthetic transaction sets) and published models that serve as starting points for custom systems.

**Note:** Commercial platforms derive major advantage from proprietary global networks, chargeback guarantees, large-scale labeled data, and continuously updated threat intelligence. Open-source solutions excel as self-hosted scoring engines, fingerprinting components, rules engines, and ML pipelines that organizations can customize and keep fully under their control. Production deployments frequently combine open components with commercial enrichment or decisioning services.

---

## Quick Start Recommendations

| Goal | Recommended Starting Point |
|------|---------------------------|
| Self-hosted AML + fraud transaction monitoring | **Jube** |
| Production-style ML fraud scoring API | **CreditGuard** or similar FastAPI + XGBoost/LightGBM projects |
| Deep-learning real-time fraud API | **FraudProx** or custom LSTM/CNN services |
| Device / browser fingerprinting | **OpenClientID** or open fingerprint cores |
| Flexible rules + data enrichment | **SEON** (commercial) or open rules engines + self-hosted enrichment |
| Chargeback guarantee + high approvals | **Signifyd** or **Riskified** |
| Identity-centric real-time decisioning | **Forter** or **Sift** |
| Banking / financial crime scale | **Feedzai** |
| Bot & adversarial traffic protection | **DataDome** |
| Account protection focus | **Castle** or **Sift** Account Defense |
| Customizable enterprise rules + device | **Kount** |

---

## Contributing

Contributions, corrections, and new open-source projects are welcome.  
Please open an issue or pull request.

---

**Last updated:** August 2026  
Emphasizing open-source tools while documenting the major commercial platforms for context. Fully featured, network-powered open-source fraud prevention platforms remain limited; the strongest options are self-hosted ML scoring APIs, device fingerprinting projects, rules engines, and emerging AML/fraud monitoring systems such as Jube that organizations can extend and operate themselves.