
Version: NAFATH-V4 Track: Software


## Overview

A secure software supply chain requires protecting every component and service that an organization depends on. Software configuration and secrets must be managed separately from application code to reduce the risk of exposing sensitive information. AI systems need protection against attacks that manipulate their inputs or training data. Mobile applications should be tested against recognized security requirements to identify weaknesses before release. Networking security is also essential because attackers may manipulate internet routing to redirect traffic. Cybersecurity teams must identify and patch vulnerabilities in widely used software libraries before they can be exploited. Finally, a Software Bill of Materials (SBOM) helps organizations identify the components included in their software and assess their exposure to known vulnerabilities. Together, these practices improve visibility, reduce risk, and support a more trustworthy software supply chain.


## Software

According to the Twelve-Factor App methodology, configuration and secrets should be stored in environment variables rather than directly in the source code. This allows settings, such as database credentials, API keys, and website addresses, to change between development, testing, and production without modifying the code. It also reduces the risk of accidentally exposing sensitive information when sharing or publishing the code on platforms like GitHub.
Resource: The Twelve-Factor App - Config - https://12factor.net/config

## AI

Adversarial machine learning attacks mainly include evasion, poisoning, and privacy attacks. Evasion attacks manipulate inputs during deployment to cause incorrect predictions. Poisoning attacks manipulate training data or model parameters to affect the model’s behavior. Privacy attacks attempt to extract sensitive information about the training data or the model itself. These attacks differ in their targets and methods, threatening the model’s integrity, reliability, and confidentiality.
Resource: https://medium.com/@tahirbalarabe2/%EF%B8%8Fadversarial-machine-learning-a-taxonomy-and-terminology-nist-ai-100-2e2023-fb7ccc11ce98

## Mobile

The OWASP Mobile Application Security Verification Standard (MASVS) is a security standard that defines requirements for protecting mobile applications. It covers areas such as data storage, cryptography, authentication, network communication, and platform interaction. Developers and security testers use MASVS to assess an app against specific security requirements, identify vulnerabilities, and verify that appropriate security controls are implemented before releasing the application.
Resource: OWASP MASVS - https://mas.owasp.org/MASVS/

## Networking

## Cybersecurity

## Data

## Misconception in My Track

## Open Question
