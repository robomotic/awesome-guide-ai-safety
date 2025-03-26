# Awesome Guide to AI Safety

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![GitHub stars](https://img.shields.io/github/stars/robomotic/awesome-guide-ai-safety?style=social)](https://github.com/robomotic/awesome-guide-ai-safety/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/robomotic/awesome-guide-ai-safety?style=social)](https://github.com/robomotic/awesome-guide-ai-safety/network/members)
[![GitHub issues](https://img.shields.io/github/issues/robomotic/awesome-guide-ai-safety)](https://github.com/robomotic/awesome-guide-ai-safety/issues)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/robomotic/awesome-guide-ai-safety/pulls)
[![Contributors](https://img.shields.io/github/contributors/robomotic/awesome-guide-ai-safety)](https://github.com/robomotic/awesome-guide-ai-safety/graphs/contributors)

A comprehensive collection of resources, frameworks, standards, regulations, and tools related to AI safety and governance. This repository also includes a [list of AI safety conferences](CONFERENCES.md) for networking and a [global map of AI regulations](AILAW.md) to track the evolving legal landscape.

## Table of Contents
- [Understanding AI Safety, Security, Assurance and Governance](#understanding-ai-safety-security-assurance-and-governance)
- [ISO Standards for AI Safety](#iso-standards-for-ai-safety)
- [AI Safety Tools](#ai-safety-tools)
  - [Open Source Tools](#open-source-tools)
  - [AI Security Tools](#ai-security-tools)
  - [Commercial Tools](#commercial-tools)
- [AI Risk Frameworks](#ai-risk-frameworks)
- [AI Regulations](#ai-regulations)
- [OWASP Top 10 for LLM Applications](#owasp-top-10-for-llm-applications)
- [MITRE ATLAS Framework](#mitre-atlas-framework)
- [AI Incident Sources](#ai-incident-sources)
- [National CERTs and Organizations Addressing AI Security](#national-certs-and-organizations-addressing-ai-security)
- [Framework Relationships](#framework-relationships)
- [Relationship to Other Regulations](#relationship-to-other-regulations)
- [Timeline of Standards and Regulations](#timeline-of-standards-and-regulations)
- [AI Safety Conferences](CONFERENCES.md)
- [Global AI Regulations and Legal Framework](AILAW.md)

## Understanding AI Safety, Security, Assurance and Governance

### AI Safety vs AI Security

While interconnected, AI Safety and AI Security focus on different aspects of AI system trustworthiness:

#### AI Safety
- **Primary Focus**: Preventing unintended harm from AI system behavior and outputs
- **Key Objectives**: 
  - Alignment with human values and ethical principles
  - System reliability and robustness
  - Prevention of unintended consequences
- **Risk Areas**: 
  - Algorithmic bias
  - Lack of transparency
  - Societal impact
  - Value misalignment

#### AI Security
- **Primary Focus**: Protecting AI systems from malicious threats
- **Key Objectives**: 
  - Confidentiality of AI systems and data
  - Integrity of models and outputs
  - Availability of AI services
- **Risk Areas**:
  - Data breaches
  - Model theft
  - Adversarial attacks
  - Infrastructure vulnerabilities

### AI Assurance

AI Assurance is the process of providing confidence in AI system trustworthiness through:

#### Key Components
1. **Measurement**: Evaluating AI system properties and behavior
2. **Evaluation**: Assessing against standards and requirements
3. **Communication**: Transparent reporting to stakeholders

#### Assurance Mechanisms
- Technical testing and validation
- Bias audits
- Conformity assessments
- Impact assessments
- Risk assessments
- Formal verification

### AI Governance

AI Governance provides the framework for ensuring responsible AI development and deployment:

#### Core Elements
1. **Policies and Standards**: Guidelines for AI development and use
2. **Risk Management**: Identifying and mitigating AI-related risks
3. **Accountability**: Clear roles and responsibilities
4. **Monitoring**: Continuous oversight of AI systems

#### Implementation Approach
- Risk-based assessment
- Cross-functional collaboration
- Regular auditing and review
- Stakeholder engagement
- Continuous improvement

The relationship between these four aspects is crucial:
- **Safety** ensures AI systems behave as intended
- **Security** protects against malicious threats
- **Assurance** provides evidence of trustworthiness
- **Governance** establishes the framework for responsible AI

Effective AI risk management requires addressing all these aspects throughout the AI system lifecycle, from design and development to deployment and monitoring.

## ISO Standards for AI Safety

| Standard | Title | Description | Status |
|----------|-------|-------------|--------|
| ISO/IEC 42001 | Information technology — Artificial intelligence — Management system | Provides requirements for an AI management system, focusing on responsible development and use of AI | Published 2023 |
| ISO/IEC TS 4213 | Assessment of machine learning classification performance | Provides a methodology for assessment of ML classification performance | Published 2023 |
| ISO/IEC 23894 | AI Risk Management | Guidance on managing risks to organizations related to AI systems | Published 2023 |
| ISO/IEC 24027 | Bias in AI systems and AI aided decision making | Guidelines addressing bias in AI systems | Under development |
| ISO/IEC 24029 | Assessment of the robustness of neural networks | Guidelines for neural network robustness assessment | Part 1 published 2021 |
| ISO/IEC 24368 | AI governance implications of using AI systems | Guidance on AI governance | Under development |
| ISO/IEC 5259 | Data quality for analytics and ML | Guidelines for data quality | Multiple parts under development |
| ISO/IEC 25059 | Quality evaluation of learning capabilities in AI systems | Guidance on evaluating AI system quality | Under development |
| ISO/IEC 38507 | Governance implications of the use of AI by organizations | Provides guidance for governing bodies on AI use | Published 2022 |
| ISO/IEC 5338 | AI system life cycle processes | Framework for AI system life cycle processes | Published 2022 |
| ISO/IEC TS 6254 | Objectives and methods for explainability of ML models | Technical specification for ML explainability | Under development |

## AI Safety Tools

### Open Source Tools

| Tool | Category | Description | Link |
|------|----------|-------------|------|
| AI Fairness 360 | Fairness | Toolkit to help detect and mitigate bias in ML models | [GitHub](https://github.com/Trusted-AI/AIF360) |
| EthicalML | Ethics | Open-source tools for ethical machine learning | [GitHub](https://github.com/EthicalML) |
| InterpretML | Explainability | Toolkit for model interpretability | [GitHub](https://github.com/interpretml/interpret) |
| LIME | Explainability | Tool for explaining predictions of ML models | [GitHub](https://github.com/marcotcr/lime) |
| SHAP | Explainability | Tool to explain outputs of any ML model | [GitHub](https://github.com/slundberg/shap) |
| ML Privacy Meter | Privacy | Tool to quantify privacy risks in ML models | [GitHub](https://github.com/privacytrustlab/ml_privacy_meter) |
| MLflow | ML Lifecycle | Platform for managing ML lifecycle | [GitHub](https://github.com/mlflow/mlflow) |
| Model Cards Toolkit | Documentation | Tool for creating model cards | [GitHub](https://github.com/tensorflow/model-card-toolkit) |

### AI Security Tools

#### Open Source

| Tool | Category | Description | Link |
|------|----------|-------------|------|
| Adversarial Robustness Toolbox | Security | Comprehensive library for building AI systems that are secure against adversarial threats, developed by IBM Research | [GitHub](https://github.com/Trusted-AI/adversarial-robustness-toolbox) |
| Foolbox | Neural Network Security | Framework for creating and evaluating adversarial examples that fool neural networks, supporting multiple ML frameworks | [GitHub](https://github.com/bethgelab/foolbox) |
| Garak | LLM Security | Comprehensive LLM vulnerability scanner by NVIDIA that detects prompt injection, jailbreaking, data extraction, and other LLM-specific attacks | [GitHub](https://github.com/NVIDIA/garak) |
| Mindgard | AI Application Security | End-to-end framework for testing and securing AI applications against prompt injection, data poisoning, and model extraction | [GitHub](https://github.com/mindgard) |
| NOVA Framework | Prompt Analysis | Open-source prompt pattern matching system combining keyword detection, semantic similarity, and LLM-based evaluation to analyze and detect prompt content | [GitHub](https://github.com/fr0gger/nova-framework) |
| CSA AI Matrix | Security Controls | Cloud Security Alliance's comprehensive framework mapping security controls to AI risks across development and deployment stages | [GitHub](https://cloudsecurityalliance.org/artifacts/ai-security-framework) |
| AI Verify | Testing Framework | World's first AI Governance Testing Framework aligned with international standards (EU, OECD, Singapore) for validating AI systems across transparency, explainability, fairness, and safety | [Website](https://aiverifyfoundation.sg/what-is-ai-verify/) |
| Project Moonshot | LLM Testing | Open-source LLM Evaluation Toolkit for benchmarking, red teaming, and testing baselines to help manage LLM deployment risks | [GitHub](https://github.com/aiverify-foundation/moonshot) |

### Commercial Tools

| Tool | Category | Description | Link |
|------|----------|-------------|------|
| IBM Watson OpenScale | Fairness/Monitoring | AI bias detection and fairness monitoring | [IBM](https://www.ibm.com/products/watson-openscale) |
| Microsoft Azure Responsible AI | Comprehensive | Suite of tools for responsible AI | [Microsoft](https://azure.microsoft.com/en-us/solutions/responsible-ai/) |
| Google Cloud AI | Comprehensive | AI platform with responsible AI features | [Google](https://cloud.google.com/ai) |
| Dataiku | ML Operations | Platform for data science and ML operations | [Dataiku](https://www.dataiku.com/) |
| Arthur AI | Monitoring | ML model monitoring platform | [Arthur](https://www.arthur.ai/) |
| Fiddler AI | Explainability/Monitoring | ML monitoring and explainability platform | [Fiddler](https://www.fiddler.ai/) |
| Credo AI | Governance | AI governance platform | [Credo AI](https://www.credo.ai/) |
| DotData | AutoML | Automated ML platform with governance features | [DotData](https://dotdata.com/) |
| Weights & Biases | Experiment Tracking | ML experiment tracking tool | [W&B](https://wandb.ai/) |
| Determined AI | Training Platform | ML training platform | [Determined AI](https://www.determined.ai/) |

#### Commercial

| Tool | Category | Description | Link |
|------|----------|-------------|------|
| Lakera | LLM Security | AI security platform that protects against prompt injections, jailbreaks, and other LLM-specific vulnerabilities with continuous monitoring | [Lakera](https://www.lakera.ai/) |
| Vijil AI | AI Security Monitoring | Comprehensive AI security platform that monitors AI systems for vulnerabilities, unauthorized access, and data leakage in real-time | [Vijil](https://www.vijil.ai/) |
| Robust Intelligence | AI Security Platform | End-to-end platform for testing, monitoring, and securing AI systems against adversarial attacks, data drift, and model failures | [Robust Intelligence](https://www.robustintelligence.com/) |

## AI Risk Frameworks

| Framework | Organization | Description | Release Date |
|-----------|--------------|-------------|--------------|
| AI Risk Management Framework (AI RMF) | NIST | Comprehensive framework for identifying, assessing, and managing AI risks | January 2023 |
| AI Risk Repository | MIT | Repository of over 1,000 AI risks with structured taxonomies | Ongoing |
| OECD Framework for the Classification of AI Systems | OECD | Classification system for AI systems based on risk levels | February 2022 |
| Responsible AI Framework | Microsoft | Framework for responsible AI development and deployment | 2022 |
| Artificial Intelligence Risk & Controls Matrix | ISACA | Matrix for evaluating AI risks and controls | 2022 |
| AI Ethics Guidelines | IEEE | Guidelines for ethical AI development | 2019 |
| Responsible AI Maturity Model | Accenture | Framework to assess and improve responsible AI practices | 2022 |
| AI Principles | Google | Principles and practices for responsible AI | 2018 |
| AI Ethics Framework | Singapore PDPC | Guidelines for ethical use of AI | 2020 |
| AI Fairness 360 | IBM | Toolkit and framework for fairness in AI | 2018 |

## AI Regulations

| Regulation | Jurisdiction | Description | Status | Effective Date |
|------------|--------------|-------------|--------|---------------|
| EU AI Act | European Union | Comprehensive regulation of AI systems based on risk levels | Approved | Phased implementation 2024-2027 |
| GDPR (AI provisions) | European Union | Data protection regulation with AI implications | Enforced | May 2018 |
| AI Executive Order (14110) | United States | Orders for development of AI with safety, security, and trust | Issued | October 2023 |
| AI Risk Management Framework (AI RMF) | United States | Voluntary framework for managing AI risks | Released | January 2023 |
| Blueprint for an AI Bill of Rights | United States | Guidelines for protecting rights in AI systems | Released | October 2022 |
| Algorithmic Accountability Act | United States | Proposed legislation for impact assessments | Proposed | - |
| China's Generative AI Regulations | China | Regulations for generative AI models | Effective | August 2023 |
| Artificial Intelligence and Data Act (AIDA) | Canada | Proposed legislation for regulating AI | Proposed | - |
| Algorithm Act | South Korea | Regulates algorithmic recommendation systems | Proposed | - |
| AI Governance Framework | Singapore | Guidelines for responsible AI deployment | Released | 2019 |

## OWASP Top 10 for LLM Applications

The OWASP Top 10 for LLM Applications provides a standardized awareness document for developers and security professionals about the most critical security risks to Large Language Model (LLM) applications. This list is updated regularly to reflect the evolving threat landscape of generative AI systems.

### OWASP GenAI Top 10 (2023-2024)

| Risk ID | Risk Name | Description | Key Mitigations |
|---------|-----------|-------------|----------------|
| LLM01 | Prompt Injection | Attackers manipulate LLMs through crafted inputs that override intended instructions or controls | Input validation, prompt hardening, context window sanitization |
| LLM02 | Insecure Output Handling | Insufficient validation of LLM outputs leading to vulnerabilities like XSS, SSRF, etc. | Output filtering, content security policies, sandboxed rendering |
| LLM03 | Training Data Poisoning | Manipulation of training data to introduce vulnerabilities or biases | Data provenance tracking, anomaly detection, dataset security |
| LLM04 | Model Denial of Service | Crafting inputs that cause excessive resource consumption | Rate limiting, resource quotas, monitoring for anomalous behavior |
| LLM05 | Supply Chain Vulnerabilities | Weaknesses in the LLM development/deployment pipeline | Vendor security assessment, model verification, integrity controls |
| LLM06 | Sensitive Information Disclosure | LLMs revealing confidential data from training or user interactions | Data minimization, PII detection, output filtering |
| LLM07 | Insecure Plugin Design | Security flaws in plugins or extensions that enhance LLM functionality | Least privilege principles, API security, input/output validation |
| LLM08 | Excessive Agency | Granting LLMs too much autonomy to perform actions | Explicit user confirmation, guardrails, limited action scope |
| LLM09 | Overreliance | Excessive trust in LLM outputs without verification | Human oversight, confidence scoring, cross-validation |
| LLM10 | Model Theft | Unauthorized access or extraction of proprietary models | Access controls, API rate limiting, watermarking |

### Mapping OWASP GenAI Top 10 to Other Frameworks and Standards

| OWASP Risk | ISO/IEC Standards | NIST AI RMF | EU AI Act Implications |
|------------|------------------|-------------|----------------------|
| LLM01: Prompt Injection | ISO/IEC 42001 (Governance), ISO/IEC 27001 (Security) | Govern 1.2, Govern 1.4, Map 1.3 | High-risk system requirements, Art. 9 |
| LLM02: Insecure Output Handling | ISO/IEC 5259 (Data quality), ISO/IEC 27001 | Map 1.3, Measure 2.2 | Transparency obligations, Art. 13 |
| LLM03: Training Data Poisoning | ISO/IEC 42001, ISO/IEC 5259, ISO/IEC 25059 | Map 2.2, Map 2.3, Map 2.4 | Data governance provisions, Art. 10 |
| LLM04: Model Denial of Service | ISO/IEC 27001, ISO/IEC TR 5469 | Measure 1.4, Manage 2.3 | Technical robustness, Art. 15 |
| LLM05: Supply Chain Vulnerabilities | ISO/IEC 42001, ISO/IEC 27001, ISO/IEC 5338 | Govern 2.3, Map 1.4 | Risk management systems, Art. 9 |
| LLM06: Sensitive Information Disclosure | ISO/IEC 27001, ISO/IEC 29134 (PIA) | Map 2.1, Measure 3.2, Manage 1.2 | Data minimization, Art. 10, GDPR alignment |
| LLM07: Insecure Plugin Design | ISO/IEC 27001, ISO/IEC 5338 | Govern 3.3, Measure 1.4 | Integration security, Art. 15 |
| LLM08: Excessive Agency | ISO/IEC 23894 (Risk Management) | Govern 1.5, Manage 3.1 | Human oversight provisions, Art. 14 |
| LLM09: Overreliance | ISO/IEC 23894, ISO/IEC 42001 | Measure 2.1, Manage 3.2 | Accuracy requirements, Art. 15 |
| LLM10: Model Theft | ISO/IEC 27001, ISO/IEC 24028 | Govern 3.2, Manage 1.4 | Technical robustness, Art. 15 |

### Benefits of OWASP Integration with ISO Standards and Regulatory Frameworks

1. **Comprehensive Security Coverage**: Using OWASP GenAI Top 10 alongside ISO standards provides both security-specific guidance and broader governance frameworks.

2. **Regulatory Alignment**: Mapping OWASP risks to regulatory requirements (e.g., EU AI Act) helps organizations proactively address compliance needs.

3. **Risk-Based Prioritization**: The OWASP risk ranking helps organizations prioritize their security efforts within the broader context of standards implementation.

4. **Implementation Guidance**: OWASP provides specific technical mitigations that complement the more process-oriented approaches in ISO standards.

5. **Security by Design**: Integrating OWASP considerations during the early stages of AI system development aligns with ISO/IEC 42001's emphasis on proper governance throughout the AI lifecycle.

## MITRE ATLAS Framework

The MITRE Adversarial Threat Landscape for Artificial-Intelligence Systems (ATLAS) framework provides a comprehensive knowledge base for understanding and mitigating adversarial threats to AI systems. Modeled after the widely-used MITRE ATT&CK framework, ATLAS maps out tactics, techniques, and procedures (TTPs) specific to attacks against machine learning systems.

### Core Components of MITRE ATLAS

| Component | Description | Examples |
|-----------|-------------|----------|
| Tactics | High-level adversarial goals | Reconnaissance, ML Supply Chain Compromise, Model Evasion |
| Techniques | Specific methods to achieve these goals | Data Poisoning, Model Inversion, Adversarial Examples |
| Case Studies | Real-world examples of AI attacks | Documented incidents of ML system compromises |
| Mitigations | Countermeasures to prevent or detect attacks | Adversarial Training, Input Validation, Model Monitoring |

### ATLAS Tactics and Techniques

| Tactic | Description | Key Techniques |
|--------|-------------|---------------|
| Reconnaissance | Gathering information about ML systems | ML Model Probing, ML Architecture Reconnaissance |
| Resource Development | Establishing resources to support operations | Acquire ML Infrastructure, Develop ML Capabilities |
| Initial Access | Gaining initial access to ML systems | Supply Chain Compromise, Social Engineering |
| ML Supply Chain Compromise | Attacking the ML development pipeline | Data Poisoning, Algorithm Poisoning, Malicious ML Components |
| ML Model Access | Accessing an ML model or its artifacts | Model Theft, Credential Access, API Abuse |
| Execution | Running adversarial code or manipulating ML execution | Code Injection, Prompt Injection, Input Manipulation |
| Collection | Gathering sensitive data from ML systems | Output Filtering, Model Inversion, Data Extraction |
| Exfiltration | Stealing model artifacts or sensitive data | Unauthorized Data Transfer, Model Extraction |
| Impact | Directly affecting ML availability, integrity, or confidentiality | DoS Attack, Model Corruption, Output Manipulation |
| Model Evasion | Bypassing ML detection systems | Adversarial Examples, Input Filtering Evasion, Feature Manipulation |
| Inference | Extracting information about the model or training data | Membership Inference, Property Inference, Training Data Extraction |

### Mapping MITRE ATLAS to ISO Standards and Risk Frameworks

| ATLAS Component | ISO/IEC Standards | AI Risk Frameworks | Implementation Considerations |
|-----------------|-------------------|-------------------|------------------------------|
| Reconnaissance Defense | ISO/IEC 27001 (Information Security), ISO/IEC 42001 (AI Management) | NIST AI RMF (Govern 2.3, Map 1.1) | Implement monitoring for ML system probing and reconnaissance |
| ML Supply Chain Security | ISO/IEC 5338 (AI Lifecycle), ISO/IEC 42001, ISO/IEC 27001 | NIST AI RMF (Map 2.3, Map A/B/C), ISACA AI Controls Matrix | Secure the entire ML development pipeline and verify data integrity |
| Model Access Controls | ISO/IEC 27001, ISO/IEC 24028 (AI Trustworthiness) | NIST AI RMF (Govern 3.2, Manage 1.4), Microsoft Responsible AI | Implement strict authentication, authorization, and auditing for model access |
| Adversarial Example Defense | ISO/IEC TR 24029 (AI Robustness), ISO/IEC 5469 (AI Functional Safety) | NIST AI RMF (Measure 1.1, Measure 1.4), Google AI Principles | Deploy adversarial training and input validation techniques |
| Model Evasion Prevention | ISO/IEC TR 24029, ISO/IEC 42001 | NIST AI RMF (Measure 2.2, Manage 1.2), Accenture Responsible AI Maturity | Implement detection mechanisms for adversarial inputs and model robustness testing |
| Inference Attack Mitigation | ISO/IEC 27001, ISO/IEC 29134 (Privacy) | NIST AI RMF (Measure 3.2, Manage 2.4), IBM AI Fairness 360 | Apply differential privacy and minimize unnecessary information disclosure |

### Benefits of Integrating MITRE ATLAS with Other Standards

1. **Comprehensive Threat Coverage**: ATLAS provides specific technical details about AI threats that complement the broader governance focus of ISO standards and risk frameworks.

2. **Security Testing Guidance**: ATLAS offers concrete examples and case studies that can be used to develop effective security testing methodologies aligned with ISO/IEC TR 24029 (Robustness assessment of neural networks).

3. **Defense-in-Depth Strategy**: Combining ATLAS with OWASP GenAI Top 10 creates a multi-layered defense approach, with ATLAS focusing on adversarial ML attacks and OWASP covering broader LLM application security.

4. **Supply Chain Security**: ATLAS's ML Supply Chain Compromise tactic aligns with ISO/IEC 5338 (AI system life cycle processes) to secure the entire AI development lifecycle.

5. **Risk Assessment Enhancement**: ATLAS case studies provide real-world examples to inform risk assessments required by ISO/IEC 23894 (AI Risk Management) and NIST AI RMF.

6. **Regulatory Compliance Support**: The detailed controls derived from ATLAS tactics help organizations meet the technical requirements of regulations like the EU AI Act, particularly for high-risk AI systems.

### Implementation Approach

Organizations can implement a unified security approach by mapping ATLAS tactics to their existing ISO-based management systems and risk frameworks:

1. Incorporate ATLAS threats into ISO/IEC 42001 risk assessments
2. Develop security controls based on ATLAS mitigations that satisfy ISO/IEC 27001 requirements
3. Use ATLAS case studies to inform threat modeling exercises required by NIST AI RMF
4. Align ATLAS defensive measures with EU AI Act technical documentation requirements
5. Implement continuous monitoring for ATLAS tactics using metrics defined in ISO/IEC 5338

### MITRE ATLAS and OWASP Relationships Diagram

```mermaid
graph TB
    classDef governance fill:#d4f1f9,stroke:#05a,stroke-width:1px
    classDef security fill:#ffe6cc,stroke:#d79b00,stroke-width:1px
    classDef regulation fill:#d5e8d4,stroke:#82b366,stroke-width:1px
    classDef relationship fill:none,stroke:#999,stroke-width:1px,stroke-dasharray: 5 5
    
    %% Main Nodes
    ATLAS[MITRE ATLAS]:::security
    OWASP[OWASP GenAI Top 10]:::security
    NIST[NIST AI RMF]:::governance
    ISO42001[ISO/IEC 42001]:::governance
    EUAI[EU AI Act]:::regulation
    
    %% ATLAS components
    ATLAS_RECON[Reconnaissance]:::security
    ATLAS_SUPPLY[ML Supply Chain]:::security
    ATLAS_EVASION[Model Evasion]:::security
    ATLAS_IMPACT[Impact]:::security
    
    %% OWASP components
    OWASP_PROMPT[LLM01: Prompt Injection]:::security
    OWASP_OUTPUT[LLM02: Insecure Output]:::security
    OWASP_POISON[LLM03: Training Data Poisoning]:::security
    OWASP_DOS[LLM04: Model DoS]:::security
    
    %% Framework components
    NIST_GOV[Govern]:::governance
    NIST_MAP[Map]:::governance
    NIST_MEASURE[Measure]:::governance
    NIST_MANAGE[Manage]:::governance
    
    ISO_RISK[Risk Management]:::governance
    ISO_LIFECYCLE[AI Lifecycle]:::governance
    
    EU_HIGHRISK[High-Risk Requirements]:::regulation
    EU_GENPURPOSE[General Purpose AI]:::regulation
    
    %% Main relationships
    ATLAS --> NIST
    OWASP --> NIST
    ATLAS --> ISO42001
    OWASP --> ISO42001
    ATLAS --> EUAI
    OWASP --> EUAI
    
    %% ATLAS breakdown
    ATLAS --> ATLAS_RECON
    ATLAS --> ATLAS_SUPPLY
    ATLAS --> ATLAS_EVASION
    ATLAS --> ATLAS_IMPACT
    
    %% OWASP breakdown
    OWASP --> OWASP_PROMPT
    OWASP --> OWASP_OUTPUT
    OWASP --> OWASP_POISON
    OWASP --> OWASP_DOS
    
    %% NIST breakdown
    NIST --> NIST_GOV
    NIST --> NIST_MAP
    NIST --> NIST_MEASURE
    NIST --> NIST_MANAGE
    
    %% ISO breakdown
    ISO42001 --> ISO_RISK
    ISO42001 --> ISO_LIFECYCLE
    
    %% EU AI Act breakdown
    EUAI --> EU_HIGHRISK
    EUAI --> EU_GENPURPOSE
    
    %% Cross-framework relationships
    ATLAS_SUPPLY -.->|Aligns with| OWASP_POISON
    ATLAS_IMPACT -.->|Relates to| OWASP_DOS
    ATLAS_EVASION -.->|Complements| OWASP_PROMPT
    
    ATLAS_RECON -.->|Informs| NIST_MAP
    ATLAS_SUPPLY -.->|Supports| NIST_GOVERN
    OWASP_PROMPT -.->|Addresses| NIST_MANAGE
    OWASP_OUTPUT -.->|Measured by| NIST_MEASURE
    
    ATLAS_SUPPLY -.->|Required by| ISO_LIFECYCLE
    OWASP_POISON -.->|Managed in| ISO_RISK
    
    ATLAS_EVASION -.->|Compliance for| EU_HIGHRISK
    OWASP_OUTPUT -.->|Required for| EU_GENPURPOSE
    
    %% Labels
    subgraph SecurityFrameworks ["Security Frameworks"]
        ATLAS
        OWASP
    end
    
    subgraph GovernanceStandards ["Governance Standards"]
        NIST
        ISO42001
    end
    
    subgraph Regulations ["Regulations"]
        EUAI
    end
```

The diagram above illustrates how MITRE ATLAS and OWASP GenAI Top 10 security frameworks integrate with key governance standards (NIST AI RMF and ISO/IEC 42001) and regulations (EU AI Act). It highlights specific relationships between components:

1. **Security Framework Components**:
   - ATLAS tactics (Reconnaissance, ML Supply Chain, Model Evasion, Impact)
   - OWASP Top 10 risks (Prompt Injection, Insecure Output, Training Data Poisoning, Model DoS)

2. **Key Relationships**:
   - ATLAS ML Supply Chain components align with OWASP Training Data Poisoning, both addressing data integrity
   - ATLAS Model Evasion techniques complement OWASP Prompt Injection defenses
   - Both frameworks support NIST AI RMF's Govern, Map, Measure, and Manage functions
   - Security controls derived from both frameworks help satisfy ISO/IEC 42001 Risk Management requirements
   - Compliance with EU AI Act high-risk and general-purpose AI provisions is enabled by implementing mitigations from both frameworks

3. **Integration Benefits**:
   - Comprehensive coverage: ATLAS focuses on adversarial ML while OWASP addresses LLM-specific vulnerabilities
   - Complementary approaches: Technical security controls (ATLAS/OWASP) support governance requirements (ISO/NIST)
   - Regulatory alignment: Security framework implementation facilitates compliance with EU AI Act requirements

## AI Incident Sources

| Source | Organization | Description | Link |
|--------|--------------|-------------|------|
| AI Incident Database | AIID | Repository of AI incidents and issues | [AIID](https://incidentdatabase.ai/) |
| AI Incidents Database | MIT | Database tracking AI incidents with risk taxonomy | [MIT](https://www.aiincidentdatabase.com/) |
| XRSI AI Incident Register | XRSI | Reports of privacy violations and harms from AI | [XRSI](https://xrsi.org/the-xrsi-ai-incident-register) |
| AI Vulnerabilities Database | AVID | Database of ML vulnerabilities | [AVID](https://avidml.org/) |
| Responsible AI Tracker | Montreal AI Ethics Institute | Tracking AI ethics incidents and developments | [MAIEI](https://montrealethics.ai/) |
| AI Ethics Incidents | ParthLabs | Collection of AI ethics incidents | [ParthLabs](https://parthlabs.github.io/ai_ethics_incidents/) |
| Algorithm Watch | Algorithm Watch | Monitoring AI systems and their impacts | [Algorithm Watch](https://algorithmwatch.org/) |
| AI Alignment Map | AI Alignment | Mapping AI alignment research and incidents | [Alignment Map](https://www.alignmentmap.org/) |
| AI Safety Gridworlds | DeepMind | Testing environments for AI safety | [GitHub](https://github.com/deepmind/ai-safety-gridworlds) |
| AI Testing Toolkit | Anthropic | Tools for testing AI safety | [Anthropic](https://www.anthropic.com/research) |

## National CERTs and Organizations Addressing AI Security

| Organization | Country/Region | AI Security Focus | Link |
|--------------|----------------|------------------|------|
| Cybersecurity and Infrastructure Security Agency (CISA) | United States | AI security guidance, vulnerability reporting, and incident response | [CISA AI](https://www.cisa.gov/ai) |
| CERT Coordination Center (CERT/CC) | United States | Vulnerability coordination and AI security research | [CERT/CC](https://www.sei.cmu.edu/about/divisions/cert/index.cfm) |
| National Cyber Security Centre (NCSC) | United Kingdom | AI security guidelines and incident reporting | [NCSC AI](https://www.ncsc.gov.uk/collection/ai) |
| Australian Cyber Security Centre (ACSC) | Australia | AI security guidance and incident response | [ACSC](https://www.cyber.gov.au/) |
| Japan Computer Emergency Response Team (JPCERT/CC) | Japan | AI vulnerability coordination and security alerts | [JPCERT/CC](https://www.jpcert.or.jp/english/) |
| BSI National Cyber Security Centre | Germany | AI security standards and incident reporting | [BSI](https://www.bsi.bund.de/EN/Themen/Unternehmen-und-Organisationen/Informationen-und-Empfehlungen/Kuenstliche_Intelligenz_KI/kuenstliche_intelligenz_node.html) |
| Canadian Centre for Cyber Security (CCCS) | Canada | AI security guidance and vulnerability management | [CCCS](https://cyber.gc.ca/en/) |
| Singapore Computer Emergency Response Team (SingCERT) | Singapore | AI system vulnerability coordination | [SingCERT](https://www.csa.gov.sg/singcert) |
| Thailand Computer Emergency Response Team (ThaiCERT) | Thailand | AI security trends and incident monitoring | [ThaiCERT](https://www.thaicert.or.th/en/) |
| Korea Internet & Security Agency (KISA) | South Korea | AI security research and incident response | [KISA](https://www.kisa.or.kr/eng/) |
| CERT-EU | European Union | AI security coordination for EU institutions | [CERT-EU](https://cert.europa.eu/) |

## Framework Relationships

Below is a Mermaid diagram showing how various frameworks, standards, and regulations are related:

```mermaid
graph TB
    AIGOVERNANCE[AI Governance Ecosystem]
    
    AIGOVERNANCE --> STANDARDS[Standards]
    AIGOVERNANCE --> FRAMEWORKS[Frameworks]
    AIGOVERNANCE --> REGULATIONS[Regulations]
    AIGOVERNANCE --> GUIDELINES[Guidelines]
    
    STANDARDS --> ISO42001[ISO/IEC 42001]
    STANDARDS --> ISO27001[ISO/IEC 27001]
    STANDARDS --> ISO27701[ISO/IEC 27701]
    STANDARDS --> ISO23894[ISO/IEC 23894]
    STANDARDS --> ISO5338[ISO/IEC 5338]
    
    FRAMEWORKS --> NISTRMF[NIST AI RMF]
    FRAMEWORKS --> MITRISK[MIT Risk Repository]
    FRAMEWORKS --> ISACA[ISACA AI Controls]
    FRAMEWORKS --> OECD[OECD AI Framework]
    
    REGULATIONS --> EUAI[EU AI Act]
    REGULATIONS --> GDPR[GDPR]
    REGULATIONS --> USEO[US AI Executive Order]
    REGULATIONS --> CHINA[China AI Regulations]
    
    GUIDELINES --> ETHICS[Ethics Guidelines]
    GUIDELINES --> BILLRIGHTS[AI Bill of Rights]
    GUIDELINES --> SINGAPORE[Singapore Guidelines]
    
    %% Relationships
    ISO42001 -->|Aligns with| NISTRMF
    ISO27001 -->|Security foundation for| ISO42001
    ISO27701 -->|Privacy extension to| ISO27001
    NISTRMF -->|Influenced| USEO
    EUAI -->|Compatible with| ISO42001
    GDPR -->|Privacy requirements for| EUAI
    MITRISK -->|Informs| NISTRMF
    OECD -->|Principles adopted in| EUAI
    BILLRIGHTS -->|Informed by| NISTRMF
```

## Relationship to Other Regulations

```mermaid
graph TD
    AIREGULATIONS[AI Regulations]
    
    AIREGULATIONS --- EUAI[EU AI Act]
    AIREGULATIONS --- USEO[US AI Executive Order]
    AIREGULATIONS --- CHINA[China AI Regulations]
    
    DATAREGULATIONS[Data Protection Regulations]
    DATAREGULATIONS --- GDPR[GDPR]
    DATAREGULATIONS --- CCPA[CCPA/CPRA]
    DATAREGULATIONS --- PIPEDA[PIPEDA]
    
    SECURITYSTANDARDS[Security Standards]
    SECURITYSTANDARDS --- ISO27001[ISO 27001]
    SECURITYSTANDARDS --- NIST800[NIST 800-53]
    SECURITYSTANDARDS --- SOC2[SOC 2]
    
    EUAI -->|Builds on| GDPR
    EUAI -->|References| ISO27001
    USEO -->|Complements| CCPA
    USEO -->|Builds on| NIST800
    
    GDPR -->|Data protection for| AI
    CCPA -->|US consumer data rights affecting| AI
    
    ISO27001 -->|Security foundation for| ISO42001
    NIST800 -->|Security controls referenced by| NISTRMF
    
    subgraph "Overlap Areas"
        DATAMINIMIZATION[Data Minimization]
        PRIVACY[Privacy by Design]
        IMPACT[Impact Assessments]
        TRANSPARENCY[Transparency]
        SECURITY[Security Measures]
    end
    
    GDPR -->|Requires| DATAMINIMIZATION
    EUAI -->|Mandates| DATAMINIMIZATION
    
    GDPR -->|Enforces| PRIVACY
    CCPA -->|Promotes| PRIVACY
    ISO42001 -->|Recommends| PRIVACY
    
    GDPR -->|Requires| IMPACT
    EUAI -->|Requires| IMPACT
    NISTRMF -->|Recommends| IMPACT
    
    GDPR -->|Focuses on| TRANSPARENCY
    EUAI -->|Mandates| TRANSPARENCY
    USEO -->|Promotes| TRANSPARENCY
    
    ISO27001 -->|Establishes| SECURITY
    NIST800 -->|Details| SECURITY
    EUAI -->|Requires| SECURITY
```

## Timeline of Standards and Regulations

```mermaid
timeline
    title Major AI Safety Standards and Regulations Timeline
    section Standards
        2019 : IEEE Ethics Guidelines
        2021 : ISO/IEC 24029-1 (Neural Networks Robustness)
        2022 : ISO/IEC 5338 (AI System Life Cycle), ISO/IEC 38507 (Governance)
        2023 : ISO/IEC 42001 (AI Management System), ISO/IEC 23894 (Risk Management), ISO/IEC TS 4213 (ML Classification)
        2024-2025 : ISO/IEC 24027, ISO/IEC 24368, ISO/IEC 5259, ISO/IEC TS 6254 (Expected)
    section Frameworks
        2018 : Google AI Principles, IBM AI Fairness 360
        2019 : Singapore AI Governance Framework
        2020 : Singapore PDPC AI Ethics Framework
        2022 : OECD AI Systems Classification, Microsoft Responsible AI, ISACA AI Controls Matrix, Accenture Responsible AI Maturity Model
        2023 : NIST AI Risk Management Framework (AI RMF)
    section Regulations
        2018 : GDPR Enforcement (EU)
        2022 : US Blueprint for an AI Bill of Rights
        2023 : China's Generative AI Regulations, US AI Executive Order 14110
        2024 : EU AI Act Adoption
        2025 : EU AI Act Initial Implementation Phase
        2027 : EU AI Act Full Implementation
```

## Related Resources

- [AI Safety Conferences](CONFERENCES.md) - A curated list of dedicated AI safety conferences and cybersecurity events with AI safety tracks
- [Global AI Regulations and Legal Framework](AILAW.md) - A comprehensive map of AI regulations and legislation worldwide with focus on safety implications
- [Contributing Guidelines](CONTRIBUTING.md) - Information on how to contribute to this repository

## Contributing

Contributions to this repository are welcome! Please see the [CONTRIBUTING.md](CONTRIBUTING.md) file for guidelines on how to contribute.

## License

This repository is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
