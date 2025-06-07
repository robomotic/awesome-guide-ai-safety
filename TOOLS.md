# LLM Guardrails Frameworks

## OWASP Top 10 for LLM Applications

The OWASP Top 10 for Large Language Model Applications highlights the most critical security risks for LLM applications, including:
1. Prompt Injection
2. Insecure Output Handling
3. Training Data Poisoning
4. Model Denial of Service
5. Supply Chain Vulnerabilities
6. Sensitive Information Disclosure
7. Insecure Plugin Design
8. Excessive Agency
9. Overreliance
10. Model Theft

## Commercial

-   **Prompt Engineering:** (Not a specific tool, but a technique)
    -   Focuses on crafting input prompts to guide LLM behavior and mitigate risks.
    -   **OWASP Coverage:** Can help reduce Prompt Injection and Insecure Output Handling, but is not a technical control.

-   **LAKERA:**
    -   Website: [https://lakera.ai/](https://lakera.ai/)
    -   Mentioned as a commercial solution provider in the LLM security space.
    -   **OWASP Coverage:**
        - Prompt Injection: ✔️
        - Insecure Output Handling: ✔️
        - Sensitive Information Disclosure: ✔️
        - Excessive Agency: ✔️
        - Compliance Violations: ✔️
        - Real-time threat detection, guardrails, and policy enforcement. Cited in OWASP LLM Security Guide as addressing Top 10 risks.
        - **Detailed Mapping:**
            - Prompt Injection: Detects and blocks prompt injection and jailbreaks.
            - Data Leakage: Prevents sensitive data exposure in outputs.
            - Output Moderation: Controls inappropriate or non-compliant outputs.
            - Compliance: Centralized policy and audit controls.
            - Overreliance/Excessive Agency: Policy-based restrictions on agent actions.

-   **WHYLABS:**
    -   Website: [https://whylabs.ai/](https://whylabs.ai/)
    -   Mentioned as a commercial solution provider in the LLM security space.
    -   **OWASP Coverage:**
        - Sensitive Information Disclosure: ✔️
        - Insecure Output Handling: ✔️ (via monitoring)
        - Prompt Injection: Partial (detects anomalies)
        - **Detailed Mapping:**
            - Observability for LLMs, anomaly detection for data leakage and output issues.
            - Not a guardrail, but provides monitoring and alerting for security events.

-   **CLOUDFLARE:**
    -   Website: [https://www.cloudflare.com/](https://www.cloudflare.com/)
    -   Mentioned as offering security features (like WAF) that can act as guardrails at the network level.
    -   **OWASP Coverage:**
        - Sensitive Information Disclosure: Partial (network-level DLP)
        - Model Denial of Service: ✔️ (DDoS protection)
        - Supply Chain: Partial (API security, bot mitigation)
        - **Detailed Mapping:**
            - Protects against DDoS, bot attacks, and some data exfiltration.
            - Not LLM-specific, but can be part of a defense-in-depth strategy.

-   **Robust Intelligence (Cisco):**
    -   Website: [https://robustintelligence.com/](https://robustintelligence.com/)
    -   Enterprise platform for AI application security, now a Cisco company.
    -   **OWASP Coverage:**
        - Prompt Injection: ✔️
        - Data Poisoning: ✔️
        - Sensitive Information Disclosure: ✔️
        - Toxic Output: ✔️
        - Supply Chain: ✔️ (AI Risk Database, NIST/OWASP mapping)
        - Model Denial of Service: ✔️
        - Others: Automated red teaming, continuous validation, AI firewall for runtime protection.
    -   **Detailed Mapping:**
        - Automated vulnerability detection and mitigation for prompt injection, data leakage, model poisoning, and more.
        - Policy mappings for compliance (NIST, MITRE, OWASP).
        - AI firewall for runtime guardrails and threat intelligence updates.
        - Contributors to the OWASP Top 10 for LLM Applications.

## Open Source

-   **NEMO Guardrails (NVIDIA):**
    -   Website: [https://github.com/NVIDIA/NeMo-Guardrails](https://github.com/NVIDIA/NeMo-Guardrails)
    -   Developer Docs: [https://developer.nvidia.com/nemo-guardrails](https://developer.nvidia.com/nemo-guardrails)
    -   Uses a custom language called Colang for defining rails.
    -   Focuses on controlling dialogue and preventing off-topic conversations.
    -   Can integrate external actions and knowledge bases.
    -   **OWASP Coverage:**
        - Prompt Injection: ✔️
        - Insecure Output Handling: ✔️
        - Sensitive Information Disclosure: ✔️
        - Hallucination: ✔️
        - Jailbreaks: ✔️
        - Excessive Agency: Partial (dialog control)
        - **Detailed Mapping:**
            - Input/Output rails for prompt injection and output moderation.
            - Sensitive data detection (Presidio integration).
            - Fact-checking and hallucination detection.
            - Jailbreak detection and dialog flow control.
            - Retrieval rails for RAG chunk filtering.

-   **Guardrails AI:**
    -   Website: [https://guardrailsai.com/](https://guardrailsai.com/)
    -   GitHub: [https://github.com/guardrails-ai/guardrails](https://github.com/guardrails-ai/guardrails)
    -   Validates and corrects LLM outputs based on predefined structures (e.g., Pydantic models).
    -   Can filter inappropriate content, enforce formatting, and ensure type safety.
    -   Offers re-asking capabilities if validation fails.
    -   **OWASP Coverage:**
        - Prompt Injection: ✔️
        - Insecure Output Handling: ✔️
        - Sensitive Information Disclosure: ✔️
        - Toxicity/Content Moderation: ✔️
        - Excessive Agency: Partial (output structure enforcement)
        - **Detailed Mapping:**
            - Input/output guards and validators for prompt injection, PII, toxicity, and output structure.
            - Custom validators for additional risks.
            - Structured output enforcement to prevent insecure outputs.

-   **PROTECT AI (Now part of Varonis):**
    -   Website: [https://www.varonis.com/](https://www.varonis.com/) (Varonis acquired Protect AI)
    -   (Not explicitly detailed in the video regarding specific guardrail features, mentioned in the broader context of AI security)
    -   **OWASP Coverage:**
        - Sensitive Information Disclosure: ✔️
        - Compliance Violations: ✔️
        - Supply Chain: Partial (data access governance)
        - **Detailed Mapping:**
            - Data discovery, classification, and access governance.
            - DLP and compliance monitoring for AI pipelines.
            - Not LLM-specific, but relevant for data security and compliance.

-   **garak:**
    -   Website: [https://github.com/leondz/garak](https://github.com/leondz/garak)
    -   Primarily an LLM vulnerability scanner, not a runtime guardrail framework itself.
    -   Used for probing and red-teaming LLMs to identify weaknesses.
    -   Helps understand potential failure modes that guardrails need to address.
    -   **OWASP Coverage:**
        - Prompt Injection: ✔️
        - Insecure Output Handling: ✔️ (testing)
        - Sensitive Information Disclosure: ✔️ (leakreplay, xss)
        - Hallucination: ✔️
        - Jailbreaks: ✔️
        - Insecure Code Generation: ✔️
        - **Detailed Mapping:**
            - Probes for prompt injection, data leakage, hallucination, jailbreaks, code generation, and more.
            - Red-teaming and vulnerability scanning, not runtime enforcement.

-   **Llamator:**
    -   Website: [https://llamator-core.github.io/llamator/](https://llamator-core.github.io/llamator/)
    -   A framework for building, testing, and deploying LLM applications, potentially incorporating guardrail mechanisms.
    -   **Feature Comparison (vs PyRIT, Garak, Giskard):**

        | Feature                                                      | PyRIT | Garak | Giskard | LLAMATOR |
        |--------------------------------------------------------------|:-----:|:-----:|:-------:|:--------:|
        | Business orientation, focus on chatbots, Q&A, RAG systems   |   ❌   |   ❌   |   ✔️    |   ✔️     |
        | Dynamic improvement of attacks (based on responses/system)  |   ✔️   |   ✔️   |   ❌    |   ✔️     |
        | Tests for identifying hallucinations and bias               |   ❌   |   ✔️   |   ✔️    |   ✔️     |
        | Attacks on the system prompt                                |   ❌   |   ❌   |   ✔️    |   ✔️     |
        | Attacks on excessive consumption (DoS)                     |   ❌   |   ❌   |   ❌    |   ✔️     |
        | Continuous AI Testing Platform                              |   ❌   |   ❌   |   ✔️    |   ⏳     |

    -   **OWASP Coverage:**
        - Prompt Injection: ✔️ (testing)
        - Insecure Output Handling: ✔️ (testing)
        - Sensitive Information Disclosure: ✔️ (testing)
        - **Detailed Mapping:**
            - Security testing framework with OWASP classification.
            - Supports single-stage and multi-stage attack testing.
            - Not a runtime guardrail, but helps identify vulnerabilities.
            - See table above for feature comparison with other tools.

-   **Mindgard CLI:**
    -   GitHub: [https://github.com/Mindgard/cli](https://github.com/Mindgard/cli)
    -   A command-line interface for security testing of AI models, including LLMs.
    -   Helps identify vulnerabilities and risks, similar in purpose to red-teaming tools like `garak`.
    -   **OWASP Coverage:**
        - Prompt Injection: ✔️
        - Jailbreaks: ✔️
        - Model Inversion/Extraction: ✔️
        - Data Poisoning: ✔️
        - Membership Inference: ✔️
        - **Detailed Mapping:**
            - Automated red-teaming for prompt injection, jailbreaks, model inversion, extraction, poisoning, and more.
            - CLI for continuous security testing and integration into MLOps pipelines.

-   **PyRIT (Microsoft):**
    -   GitHub: [https://github.com/Azure/PyRIT](https://github.com/Azure/PyRIT)
    -   Open-source red teaming tool for LLMs.
    -   **OWASP Coverage:**
        - Prompt Injection: ✔️ (dynamic attack generation)
        - Insecure Output Handling: ✔️ (testing)
        - Data Leakage: ✔️ (testing)
        - Hallucination: Partial (testing)
        - Model Denial of Service: Partial (testing)
    -   **Detailed Mapping:**
        - Focuses on dynamic, automated attack generation to test LLM robustness.
        - Used for red teaming and security evaluation, not runtime protection.
        - Can be integrated into CI/CD for continuous testing.

-   **Giskard:**
    -   Website: [https://giskard.ai/](https://giskard.ai/)
    -   Open-source and enterprise platform for LLM security and quality.
    -   **OWASP Coverage:**
        - Prompt Injection: ✔️
        - Sensitive Information Disclosure: ✔️
        - Toxicity: ✔️
        - Hallucinations & Misinformation: ✔️
        - Stereotypes & Discrimination: ✔️
        - Robustness: ✔️
        - Model Denial of Service: Partial (testing)
    -   **Detailed Mapping:**
        - Automated vulnerability detection (prompt injection, data leaks, hallucinations, etc.).
        - Continuous red teaming and proactive monitoring.
        - Collaborative annotation and test case generation.
        - Can be used before and after deployment for continuous security.

---

## Summary Table

| Tool/Platform         | Prompt Injection | Data Leakage | Output Validation | Hallucination | Jailbreaks | Toxicity/Content | Compliance | DoS/Robustness | Supply Chain | Other Risks | Notes |
|----------------------|:---------------:|:------------:|:-----------------:|:-------------:|:----------:|:---------------:|:----------:|:--------------:|:------------:|:-----------:|:------|
| NeMo Guardrails      |       ✔️        |      ✔️      |        ✔️         |      ✔️       |     ✔️     |       ✔️        |   ✔️*      |     ✔️*        |     ❌       |   Custom    | Programmable rails, dialog control |
| Guardrails AI        |       ✔️        |      ✔️      |        ✔️         |      ✔️*      |     ✔️*    |       ✔️        |   ✔️*      |     ❌         |     ❌       |   Custom    | Input/output guards, validators |
| garak                |       ✔️        |      ✔️      |        ✔️*        |      ✔️       |     ✔️     |       ✔️        |     ❌     |     ✔️*        |     ❌       |   Testing   | Red-teaming, scanner |
| Llamator             |       ✔️        |      ✔️      |        ✔️*        |      ✔️*      |     ✔️*    |       ✔️*       |     ❌     |     ✔️         |     ❌       |   Testing   | Security testing framework |
| Mindgard CLI         |       ✔️        |      ✔️      |        ✔️*        |      ✔️*      |     ✔️     |       ✔️*       |     ❌     |     ✔️         |     ❌       |   Testing   | Automated red-teaming |
| Lakera               |       ✔️        |      ✔️      |        ✔️         |      ✔️*      |     ✔️     |       ✔️        |   ✔️       |     ✔️*        |     ✔️*      | Real-time   | Enterprise, runtime guardrails |
| Whylabs              |       ✔️*       |      ✔️      |        ✔️*        |      ✔️*      |     ❌     |       ✔️*       |   ✔️*      |     ❌         |     ❌       | Monitoring  | Observability, anomaly detection |
| Cloudflare           |       ❌        |      ✔️*     |        ❌         |      ❌       |     ❌     |       ❌        |   ✔️*      |     ✔️         |     ✔️*      | Network     | Network-level protection |
| Protect AI/Varonis   |       ❌        |      ✔️      |        ❌         |      ❌       |     ❌     |       ❌        |   ✔️       |     ❌         |     ✔️*      | Data Sec.   | Data security, compliance |
| Robust Intelligence  |       ✔️        |      ✔️      |        ✔️         |      ✔️       |     ✔️     |       ✔️        |   ✔️       |     ✔️         |     ✔️       | Red-teaming | AI firewall, policy mapping |
| PyRIT                |       ✔️        |      ✔️      |        ✔️*        |      ✔️*      |     ✔️*    |       ✔️*       |     ❌     |     ✔️*        |     ❌       |   Testing   | Dynamic attack generation |
| Giskard              |       ✔️        |      ✔️      |        ✔️*        |      ✔️       |     ✔️*    |       ✔️        |   ✔️*      |     ✔️*        |     ❌       |   Testing   | Continuous red teaming |

*✔️* = Partial or indirect coverage

**Legend:**
- ✔️ = Direct or strong coverage
- Partial/✔️* = Indirect or partial coverage
- (testing) = Tool is for testing, not runtime protection
- ❌ = Not covered

For more details on the OWASP Top 10 for LLM Applications, see: https://owasp.org/www-project-top-10-for-large-language-model-applications/
