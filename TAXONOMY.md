## Microsoft Taxonomy of Failure Modes in AI Agents

Microsoft's 2025 whitepaper, "Taxonomy of Failure Modes in Agentic AI Systems," introduces a structured framework for understanding and categorizing the ways in which AI agents can fail. This taxonomy is designed to support risk assessment, safety engineering, and incident response for agentic AI systems.

### Core Concepts
- **Safety Failure Modes**: Occur when an agent causes harm or violates safety constraints, even if not explicitly instructed to do so. Examples include unintended actions, escalation of privileges, or unsafe exploration.
- **Security Failure Modes**: Involve breaches of confidentiality, integrity, or availability, such as prompt injection, model extraction, or adversarial attacks.
- **Reliability Failure Modes**: Relate to breakdowns in expected operation, such as task incompletion, deadlocks, or resource exhaustion.
- **Alignment Failure Modes**: Happen when the agent's actions diverge from intended goals or values, including specification gaming or reward hacking.
- **Interaction Failure Modes**: Arise from miscommunication or coordination failures between agents, users, or external systems.

### Example Failure Mode Categories
- **Unsafe Autonomy**: Agents act beyond their intended scope, leading to unintended consequences.
- **Prompt Injection and Manipulation**: Attackers alter agent behavior through crafted inputs.
- **Specification Gaming**: Agents exploit loopholes in their objectives or reward functions.
- **Coordination Failures**: Multiple agents interact in ways that amplify risk or cause cascading failures.

### Application
This taxonomy provides a foundation for:
- Systematic risk assessment and threat modeling for agentic AI
- Designing safety and security controls
- Incident investigation and reporting

For further details, see the original Microsoft whitepaper: [Taxonomy of Failure Modes in Agentic AI Systems](https://www.microsoft.com/en-us/security/blog/2025/04/24/new-whitepaper-outlines-the-taxonomy-of-failure-modes-in-ai-agents/)

## MITRE ATLAS Taxonomy for AI Security

The MITRE ATLAS (Adversarial Threat Landscape for Artificial-Intelligence Systems) taxonomy provides a comprehensive framework for understanding and categorizing adversarial threats to AI and machine learning systems. ATLAS is designed to help organizations identify, assess, and mitigate security risks throughout the AI system lifecycle.

### Core Components
- **Tactics**: High-level adversarial goals, such as reconnaissance, initial access, model evasion, and impact.
- **Techniques**: Specific methods adversaries use to achieve their goals, including data poisoning, model inversion, adversarial examples, and supply chain compromise.
- **Case Studies**: Real-world incidents and documented attacks on AI/ML systems.
- **Mitigations**: Defensive measures and best practices to prevent, detect, or respond to attacks.

### Example Tactics and Techniques
- **Reconnaissance**: Gathering information about AI/ML systems (e.g., model probing, architecture reconnaissance).
- **Resource Development**: Acquiring infrastructure or tools to support attacks (e.g., developing adversarial datasets).
- **Initial Access**: Gaining access to AI systems (e.g., supply chain compromise, social engineering).
- **ML Supply Chain Compromise**: Attacking the development pipeline (e.g., data poisoning, malicious components).
- **Model Evasion**: Bypassing detection or controls (e.g., adversarial examples, input manipulation).
- **Impact**: Affecting the availability, integrity, or confidentiality of AI systems (e.g., denial of service, model corruption).

### Application
The ATLAS taxonomy supports:
- Threat modeling and risk assessment for AI/ML systems
- Security testing and red teaming
- Incident response and forensics
- Mapping to standards and regulatory requirements

For more details, see the official MITRE ATLAS resource: [AI Security 101](https://atlas.mitre.org/resources/ai-security-101)
