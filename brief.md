
Version: NAFATH-V4 Track: Software



## Overview

A secure software supply chain requires protecting every component and service that an organization depends on. Software configuration and secrets must be managed separately from application code to reduce the risk of exposing sensitive information. AI systems need protection against attacks that manipulate their inputs or training data. Mobile applications should be tested against recognized security requirements to identify weaknesses before release. Networking security is essential because attackers may manipulate internet routing to redirect traffic. Cybersecurity teams must identify and patch vulnerabilities in software libraries before they can be exploited. Finally, a Software Bill of Materials (SBOM) helps organizations identify software components and assess their exposure to known vulnerabilities. Together, these practices improve visibility, reduce risk, and support a more trustworthy software supply chain. My chosen Software track focuses on secure configuration and secrets management.



## Software

According to the Twelve-Factor App methodology, configuration and secrets should be stored in environment variables rather than directly in the source code. This allows settings, such as database credentials, API keys, and website addresses, to change between development, testing, and production without modifying the code. It also reduces the risk of accidentally exposing sensitive information when sharing or publishing the code on platforms like GitHub.

Resource: The Twelve-Factor App - Config - https://12factor.net/config

## AI

Adversarial machine learning attacks mainly include evasion, poisoning, and privacy attacks. Evasion attacks manipulate inputs during deployment to cause incorrect predictions. Poisoning attacks manipulate training data or model parameters to affect the model’s behavior. Privacy attacks attempt to extract sensitive information about the training data or the model itself. These attacks differ in their targets and methods, threatening the model’s integrity, reliability, and confidentiality.

Resource:Medium-Adversarial Machine Learning: Understanding Risks and Defenses- https://medium.com/@tahirbalarabe2/%EF%B8%8Fadversarial-machine-learning-a-taxonomy-and-terminology-nist-ai-100-2e2023-fb7ccc11ce98

## Mobile

The OWASP Mobile Application Security Verification Standard (MASVS) is a security standard that defines requirements for protecting mobile applications. It covers areas such as data storage, cryptography, authentication, network communication, and platform interaction. Developers and security testers use MASVS to assess an app against specific security requirements, identify vulnerabilities, and verify that appropriate security controls are implemented before releasing the application.

Resource: OWASP MASVS - https://mas.owasp.org/MASVS/


## Networking

BGP hijacking occurs when a network announces incorrect or unauthorized internet routes, potentially redirecting traffic to the wrong destination. Resource Public Key Infrastructure (RPKI) helps reduce this risk through Route Origin Authorisations (ROAs), which identify the Autonomous System allowed to originate an IP prefix. Networks can validate route origins and reject invalid announcements. However, origin validation alone cannot verify the complete AS path or prevent every routing attack.

Resource: RIPE NCC - BGP Origin Validation - https://www.ripe.net/manage-ips-and-asns/resource-management/rpki/bgp-origin-validation/

## Cybersecurity

Log4Shell (CVE-2021-44228) is a critical remote code execution vulnerability in Apache Log4j, a Java logging library. It received a CVSS severity score of 10.0 out of 10. An attacker could exploit vulnerable configurations through crafted input processed by Log4j. Organizations should identify affected applications, update Log4j to an appropriate current patched version, and verify that remediation has succeeded.

Resource: Apache Logging Services - Security - https://logging.apache.org/security.html

## Data

A Software Bill of Materials (SBOM) is a formal record describing software components and their relationships. It helps organizations identify what is included in an application and investigate whether components are affected by known vulnerabilities. Minimum elements include supplier name, component name, component version, other unique identifiers, dependency relationships, SBOM author, and timestamp. Maintaining accurate SBOMs improves software supply-chain visibility but does not eliminate every security risk.

Resource: NTIA - The Minimum Elements For a Software Bill of Materials (SBOM) - https://www.ntia.gov/report/2021/minimum-elements-software-bill-materials-sbom


## Misconception in My Track

A common misconception is that passwords and API keys are safe to hardcode in source code if the GitHub repository is private. This is incorrect because code may be shared, copied, logged, or exposed accidentally, making secrets harder to control and rotate. The Twelve-Factor App recommends separating configuration from code and storing configuration in the environment. However, environment variables also require protection and are not a complete secrets-management solution. The relevant evidence is in “III. Config,” particularly “Store config in the environment”.


## Open Question

How can a development team securely manage secrets across development, testing, and production environments while preventing accidental exposure through logs, deployment settings, or compromised systems?

