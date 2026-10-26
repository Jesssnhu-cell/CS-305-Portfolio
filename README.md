# CS-305-Portfolio
A portfolio showcasing secure software development, vulnerability assessment, and cryptographic practices completed in CS 305 at Southern New Hampshire University.
# CS 305 Portfolio — Software Security

**Southern New Hampshire University | CS 305: Software Security**

## Artemis Financial — Practices for Secure Software

### 1. Client and Software Requirements

Artemis Financial is a financial consulting company that provides individualized financial plans involving savings, retirement, investments, and insurance. The company wanted to modernize its public-facing web application while improving the protection of sensitive customer information. My responsibility was to enhance the existing application by implementing secure communication mechanisms and a checksum verification process to support data integrity.

### 2. Identifying Vulnerabilities and the Importance of Secure Coding

One area I handled well was using OWASP Dependency-Check to identify potential vulnerabilities in the application's third-party dependencies. I reviewed the scan results and recognized that successfully completing a build does not mean an application is free from vulnerabilities.

Secure coding is important because it helps protect sensitive information, reduce the risk of unauthorized access, and maintain customer trust. For a financial services company, strong software security also supports business continuity and reduces the potential impact of security incidents.

### 3. Challenges and Lessons from the Vulnerability Assessment

One of the more challenging aspects of the project was configuring and interpreting the OWASP Dependency-Check results. The scan identified 16 vulnerable dependencies and 295 reported vulnerabilities, which demonstrated how security issues can exist even when an application appears to function correctly.

This experience helped me better understand the importance of reviewing third-party libraries and distinguishing between successful execution and actual security readiness.

### 4. Increasing Layers of Security

I increased the application's security by implementing SHA-256 hashing through Java's MessageDigest class to generate a checksum for data-integrity verification. I also generated a self-signed digital certificate, configured a PKCS12 keystore, and enabled HTTPS communication on port 8443.

For future vulnerability assessments, I would continue using OWASP Dependency-Check, established guidance from NIST and OWASP, and manual code reviews. I would evaluate vulnerabilities based on their severity, affected components, and potential impact before choosing mitigation techniques such as dependency updates, configuration changes, or stronger security controls.

### 5. Functional Testing and Security Verification

After refactoring the application, I ran the Spring Boot server in Eclipse and accessed the HTTPS endpoint at `https://localhost:8443/hash`. I verified that the application displayed the expected SHA-256 checksum.

I also reviewed the Java code and application configuration and performed a secondary dependency scan. Although the application functioned successfully, the scan identified vulnerabilities requiring further review. This reinforced the importance of ongoing security testing rather than relying only on a successful build.

### 6. Resources, Tools, and Coding Practices

The primary tools I used were Eclipse IDE, Java, Spring Boot, Maven, Java Keytool, and OWASP Dependency-Check. I also used Java's MessageDigest class for SHA-256 hashing and an SSL/TLS configuration for secure communication.

I found NIST encryption standards, OWASP security guidance, manual code review, and dependency scanning especially helpful. These resources and practices will support future software development projects.

### 7. Portfolio Value for Future Employers

This project demonstrates my ability to work with an existing Java application, implement cryptographic hashing, configure HTTPS, generate a digital certificate, and perform software vulnerability testing.

I would show future employers my completed *Artemis Financial Practices for Secure Software Report* as evidence of my understanding of secure software development, technical troubleshooting, testing, and security documentation. The project also demonstrates my ability to identify areas that require further remediation and communicate those findings clearly.

## Portfolio Artifact

**Artemis Financial Practices for Secure Software Report — CS 305 Project Two**

This repository includes my completed report documenting the security improvements, functional testing, and vulnerability assessment performed for the Artemis Financial application.

